# Copilot Default Python Environment | Copilot 默认 Python 环境

[![EN](https://img.shields.io/badge/lang-English-blue)](#english) &nbsp; [![中文](https://img.shields.io/badge/lang-中文-red)](#中文)

---

<a id="english"></a>

## 🇬🇧 English

Set a default Python virtual environment for GitHub Copilot, so that Copilot automatically uses your specified conda/virtualenv environment in every new conversation.

### Features

- 🐍 **Set Default Python Environment**: Choose a conda environment or manually specify a Python interpreter path
- 📌 **Status Bar Display**: Show the current default environment in the VS Code bottom status bar
- 🔄 **Quick Switch**: Click the status bar or use the command palette to quickly switch environments
- 🚀 **Auto Activation**: Automatically set the Python interpreter path when VS Code starts
- 🔗 **Copilot Integration**: Sync with `python.defaultInterpreterPath` to ensure Copilot uses the correct environment

### Usage

#### 1. Set Default Environment

- Press `Ctrl+Shift+P` to open the command palette
- Search for **"Copilot: Set Default Python Environment"**
- Select your conda environment from the list, or manually enter a path

#### 2. View Current Environment

- Click the environment name in the bottom status bar
- Or run the command **"Copilot: Show Current Default Python Environment"**

#### 3. Configure via Settings

In `settings.json`:

```json
{
  "copilotDefaultEnv.pythonEnvironment": "YOUR_ENV_NAME",
  "copilotDefaultEnv.environmentType": "conda",
  "copilotDefaultEnv.autoActivate": true
}
```

### Installation

1. Place this folder into the VS Code extensions directory:
   - Windows: `%USERPROFILE%\.vscode\extensions\ygj.copilot-default-env-1.0.0`
2. Restart VS Code
3. Run `npm install && npm run compile` to compile the extension

### Requirements

- VS Code 1.85.0+
- Conda (optional, for automatic environment discovery)

---

<a id="中文"></a>

## 🇨🇳 中文

为 GitHub Copilot 设置默认 Python 虚拟环境，让 Copilot 在每次新对话中自动使用你指定的 conda/virtualenv 环境。

### 功能

- 🐍 **设置默认 Python 环境**: 选择 conda 环境或手动指定 Python 解释器路径
- 📌 **状态栏显示**: 在 VS Code 底部状态栏显示当前默认环境
- 🔄 **快速切换**: 点击状态栏或使用命令面板快速切换环境
- 🚀 **自动激活**: 启动 VS Code 时自动设置 Python 解释器路径
- 🔗 **Copilot 集成**: 与 `python.defaultInterpreterPath` 同步，确保 Copilot 使用正确的环境

### 使用方式

#### 1. 设置默认环境

- 按 `Ctrl+Shift+P` 打开命令面板
- 搜索 **"Copilot: 设置默认 Python 环境"**
- 在列表中选择你的 conda 环境，或手动输入路径

#### 2. 查看当前环境

- 点击底部状态栏的环境名称
- 或执行命令 **"Copilot: 显示当前默认 Python 环境"**

#### 3. 通过设置配置

在 `settings.json` 中:

```json
{
  "copilotDefaultEnv.pythonEnvironment": "你的环境名",
  "copilotDefaultEnv.environmentType": "conda",
  "copilotDefaultEnv.autoActivate": true
}
```

### 安装

1. 将此文件夹放到 VS Code 扩展目录:
   - Windows: `%USERPROFILE%\.vscode\extensions\ygj.copilot-default-env-1.0.0`
2. 重启 VS Code
3. 运行 `npm install && npm run compile` 编译扩展

### 要求

- VS Code 1.85.0+
- Conda（可选，用于自动发现环境）
