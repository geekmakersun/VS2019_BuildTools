# Visual Studio 2019 Build Tools 离线安装包

本项目是 Visual Studio 2019 Build Tools 的离线安装包布局，用于在无网络或受限网络环境下部署 Visual Studio 构建工具。

## 项目概述

- **版本**: Visual Studio 2019 (v16.11)
- **包含组件**: 
  - MSBuild 构建工具
  - .NET Framework 4.7.2 SDK
  - C++ 构建工具 (VC++ v14.29)
  - Windows 10 SDK (10.0.19041)
  - Python 开发工具
  - NuGet 包管理器
  - 代码分析工具
  - IntelliTrace 调试工具

- **文件统计**:
  - 总文件数: 597
  - 总大小: ~1.78 GB
  - 主要文件类型: .vsix, .cab, .msi, .exe

## 使用方法

### 本地安装

1. 确保系统已安装 [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework/net472) 或更高版本
2. 运行 `vs_BuildTools.exe` 启动安装程序
3. 选择需要的组件进行安装

### 网络部署

将整个目录复制到网络共享位置，其他用户可通过访问共享目录运行安装程序。

## Git LFS 说明

本项目使用 Git Large File Storage (LFS) 管理大文件，以下文件类型已配置 LFS 追踪：

- `.vsix` - Visual Studio 扩展包 (~1062 MB)
- `.cab` - Cabinet 压缩文件 (~434 MB)
- `.msi` - Windows 安装包 (~51 MB)
- `.exe` - 可执行文件 (~213 MB)
- `.msu` - Windows 更新包 (~5 MB)
- `.opc` - Open Packaging Convention 文件 (~47 MB)

克隆本仓库前请确保已安装 Git LFS：
```bash
git lfs install
```

## 系统要求

- **操作系统**: Windows 7 SP1 或更高版本 / Windows 10 / Windows Server 2012 R2 或更高版本
- **硬盘空间**: 至少 10 GB（安装需要额外空间）
- **内存**: 最少 2 GB，推荐 4 GB 或更高

## 许可证

本项目基于 MIT 许可证开源，详见 [LICENSE](LICENSE) 文件。

Visual Studio 2019 Build Tools 本身遵循 Microsoft 的许可协议，使用前请确保遵守相关许可条款。

## 参考资料

- [Visual Studio Build Tools 官方文档](https://docs.microsoft.com/visualstudio/install/use-command-line-parameters-to-install-visual-studio)
- [创建离线安装布局](https://docs.microsoft.com/visualstudio/install/create-an-offline-installation-of-visual-studio)
- [Git LFS 官方网站](https://git-lfs.github.com/)

## 贡献

本项目主要用于存档和分发 Visual Studio Build Tools 离线安装包，不接受代码贡献。

## 更新日志

- **2026-06-29**: 初始版本，包含 VS2019 Build Tools v16.11 组件