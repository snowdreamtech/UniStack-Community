# UniStack Community Registry

[English](README.md) | [简体中文](README.zh-CN.md)
Welcome to the **UniStack Community Registry**! This repository serves as the central index and package registry for the open-source community ecosystem of UniStack.

## 📦 What is this?

This registry allows developers to share their custom UniStack packages with the community. When a user runs `unistack install author/package`, the `unistack` CLI queries this registry's generated SQLite index to resolve and download the package.

## 🚀 How to Contribute a Package

We welcome contributions from the community! To ensure security and prevent naming collisions, we enforce strict namespace rules.

### Namespace Rules
- All community packages **MUST** use a namespace prefix (e.g., `your-username/package-name`).
- Root-level namespaces (e.g., just `package-name`) are strictly reserved for official Core UniStack packages and are prohibited in this community registry.
- Your package files should be placed under the directory structure: `packages/[first_letter_of_namespace]/[namespace]/[package_name]/`.

### Submission Process
1. Fork this repository.
2. Create your package structure following the namespace rules.
3. Include a valid `package.yml` and any installation scripts.
4. Open a Pull Request! Our CI will automatically validate your YAML format, namespace, and run a Sandbox Installation Test.

For detailed instructions, please read our [Contributing Guide](CONTRIBUTING.md).

## ⚖️ License & Agreements

By contributing to this repository, you agree that your contributions will be licensed under the [MIT License](LICENSE) (or the license specified in your package). 
All contributors are required to sign our [Contributor License Agreement (CLA)](CLA.md) upon opening their first Pull Request.
