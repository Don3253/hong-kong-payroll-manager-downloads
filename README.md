# 香港工资管家下载

这是香港工资管家的二进制发布仓库，只提供 Windows 安装程序和 SHA-256 校验文件，不包含底层源代码。

## 下载

[进入最新版下载页](https://github.com/Don3253/hong-kong-payroll-manager-downloads/releases/latest)

适用系统：Windows 10/11 x64。下载 `香港工资管家-安装程序-*.exe` 后运行安装；工资资料仅保存在当前 Windows 用户的本机应用数据目录。

## 校验文件

下载同版本 `.sha256` 文件后，可在 PowerShell 中核对：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath ".\香港工资管家-安装程序-1.1.0.exe"
```

输出必须与 `.sha256` 文件中的值完全一致。若不一致，请勿运行安装程序。

## 签名状态

`1.1.0` 当前未使用公众信任的 Windows Authenticode 证书签名，因此 Windows 可能显示“未知发布者”或 SmartScreen 提示。已提供 SHA-256 用于传输完整性核验。受信代码签名将在发布者完成证书机构身份验证后接入；不会使用自签名证书冒充可信发布者。

## 安全说明

- 本仓库不发布源码，源码仓库保持私有。
- 客户端软件无法从技术上保证绝对不可逆向；本版采用 ASAR、ASAR 完整性校验、Electron 安全熔丝、沙箱、关闭正式版开发者工具及远程调试等措施提高提取和篡改门槛。
- 工资与银行资料属于敏感数据。请从本仓库的 Release 页面下载、核对哈希，并启用 Windows 设备加密/BitLocker。
- IR56 文件是核对工作底稿，不是税务局正式申报文件；银行上传文件及法定计算在商用前应由专业人士复核。

Copyright © 2026 Don3253. All rights reserved. No source-code license is granted by this repository.
