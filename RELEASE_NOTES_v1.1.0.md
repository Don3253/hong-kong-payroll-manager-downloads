# 香港工资管家 1.1.0

## 本次更新

- 更新全套品牌 Logo、Windows 多尺寸图标和网页图标。
- 升级 Electron 与 PDF 组件并修复全部已知 npm 依赖漏洞。
- 加固 Electron sandbox、context isolation、IPC 来源验证、外部链接白名单和本地服务安全响应头。
- 启用 ASAR 完整性、OnlyLoadAppFromAsar 及多项 Electron 安全熔丝；正式版关闭开发者工具与远程调试入口。
- 修复随月份变化失效的自动化测试。

## 验证

- 152/152 项自动化测试通过。
- 核心代码行覆盖率 94.37%。
- npm 生产及完整依赖审计：0 个已知漏洞。
- 打包版启动、Logo、导航及三语即时切换测试通过。
- 安装程序 SHA-256：`6B5EADEEB710FC40FCD5646BBCA5D0AD5B45ADA13BE65E3027D71B97682D3299`。

## 重要提示

本版本尚未使用公众信任的 Authenticode 证书签名。请从本仓库下载并核对 SHA-256；Windows 可能显示未知发布者提示。
