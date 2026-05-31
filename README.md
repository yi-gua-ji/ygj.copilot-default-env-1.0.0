# Copilot Default Python Environment

为 GitHub Copilot 设置默认 Python 虚拟环境，让 Copilot 在每次新对话中自动使用你指定的 conda/virtualenv 环境。

## 功能

- 🐍 **设置默认 Python 环境**: 选择 conda 环境或手动指定 Python 解释器路径
- 📌 **状态栏显示**: 在 VS Code 底部状态栏显示当前默认环境
- 🔄 **快速切换**: 点击状态栏或使用命令面板快速切换环境
- 🚀 **自动激活**: 启动 VS Code 时自动设置 Python 解释器路径
- 🔗 **Copilot 集成**: 与 `python.defaultInterpreterPath` 同步，确保 Copilot 使用正确的环境

## 使用方式

### 1. 设置默认环境

- 按 `Ctrl+Shift+P` 打开命令面板
- 搜索 **"Copilot: 设置默认 Python 环境"**
- 在列表中选择你的 conda 环境，或手动输入路径

### 2. 查看当前环境

- 点击底部状态栏的环境名称
- 或执行命令 **"Copilot: 显示当前默认 Python 环境"**

### 3. 通过设置配置

在 `settings.json` 中:

```json
{
  "copilotDefaultEnv.pythonEnvironment": "venv1",
  "copilotDefaultEnv.environmentType": "conda",
  "copilotDefaultEnv.autoActivate": true
}
```

## 安装

1. 将此文件夹放到 VS Code 扩展目录:
   - Windows: `%USERPROFILE%\.vscode\extensions\copilot-default-env`
2. 重启 VS Code
3. 运行 `npm install && npm run compile` 编译扩展

## 要求

- VS Code 1.85.0+
- Conda（可选，用于自动发现环境）
