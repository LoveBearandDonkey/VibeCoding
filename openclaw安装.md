# OpenClaw 安装指南

## 什么是 OpenClaw？

OpenClaw 是一个跨平台的游戏引擎，用于开发类似 Commander Keen 的 2D 平台游戏。它是 Claw 游戏引擎的开源实现。

## 安装方法

### 方法一：从源码编译

#### 1. 安装依赖

**Windows:**
```bash
# 安装 Visual Studio 2019 或更高版本
# 安装 CMake 3.10+
# 安装 Git
```

**Linux:**
```bash
sudo apt-get update
sudo apt-get install build-essential cmake git libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev
```

**macOS:**
```bash
# 安装 Xcode 命令行工具
xcode-select --install

# 安装 Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 安装依赖
brew install cmake git sdl2 sdl2_image sdl2_mixer
```

#### 2. 克隆源码

```bash
git clone https://github.com/OpenClaw/OpenClaw.git
cd OpenClaw
```

#### 3. 编译

**Windows:**
```bash
mkdir build
cd build
cmake ..
# 打开生成的 .sln 文件并编译
```

**Linux/macOS:**
```bash
mkdir build
cd build
cmake ..
make -j4
```

### 方法二：下载预编译版本

1. 访问 [OpenClaw GitHub 发布页](https://github.com/OpenClaw/OpenClaw/releases)
2. 下载对应平台的预编译包
3. 解压并运行

## 配置游戏数据

1. 你需要获取 Claw 游戏的原始数据文件
2. 将数据文件复制到 OpenClaw 的 `data` 目录
3. 运行 OpenClaw 即可开始游戏

## 常见问题

### 找不到游戏数据
- 确保你已正确放置 Claw 游戏的数据文件到 `data` 目录

### 编译错误
- 检查是否安装了所有依赖
- 确保使用的是兼容的编译器版本

### 运行时错误
- 检查 SDL2 相关库是否正确安装
- 确认游戏数据文件完整

## 资源链接

- [OpenClaw GitHub 仓库](https://github.com/OpenClaw/OpenClaw)
- [OpenClaw 官方网站](https://openclaw.github.io/)
- [SDL2 官方网站](https://www.libsdl.org/)

## 系统要求

- **Windows:** Windows 7 或更高版本
- **Linux:** 支持 SDL2 的 Linux 发行版
- **macOS:** macOS 10.10 或更高版本
- **硬件:** 1 GHz CPU, 512 MB RAM, 支持 OpenGL 2.0 的显卡
