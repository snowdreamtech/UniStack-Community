# UniStack Community Registry (社区注册表)

[English](README.md) | [简体中文](README.zh-CN.md)

欢迎来到 **UniStack Community Registry**！本仓库是 UniStack 开源社区生态系统的中央索引和包注册表。

## 📦 这是什么？

该注册表允许开发者与社区分享他们自定义的 UniStack 包。当用户运行 `unistack install author/package` 时，`unistack` 命令行工具会查询本仓库生成的 SQLite 索引，以解析并下载相应的包。

## 🚀 如何贡献包

我们非常欢迎来自社区的贡献！为了确保安全性并防止命名冲突，我们实施了严格的命名空间规则。

### 命名空间规则
- 所有社区包 **必须** 使用命名空间前缀（例如：`your-username/package-name`）。
- 根级别命名空间（例如：只有 `package-name`）严格保留给官方的 Core UniStack 核心包，本社区注册表中严禁使用。
- 您的包文件应放置在以下目录结构下：`packages/[命名空间的首字母]/[命名空间]/[包名]/`。

### 提交流程
1. Fork 本仓库。
2. 按照命名空间规则创建您的包结构。
3. 包含一个有效的 `package.yml` 文件和任何必要的安装脚本。
4. 开启一个 Pull Request！我们的 CI 会自动验证您的 YAML 格式、命名空间，并运行沙盒安装测试。

有关详细指引，请阅读我们的[贡献指南](CONTRIBUTING.md)。

## ⚖️ 许可与协议

通过向本仓库提交贡献，即表示您同意您的贡献将在 [MIT 许可证](LICENSE)（或您包中指定的许可证）下分发。
所有贡献者在开启第一个 Pull Request 时，都必须签署我们的[贡献者许可协议 (CLA)](CLA.md)。
