## 项目简介

ChatMemOllama 是一个个人微信公众号聊天机器人，结合了本地 AI 模型（由 Ollama 提供）和 mem0 记忆管理功能。该项目旨在提供一个智能、个性化的聊天体验。
注意！使用mem0的版本仅为早期测试版，速度慢且设计不科学(仅依靠mem0不科学)，请先使用旧版
请等待后续更新 欢迎提交pr
目前测试加入tool calling让ai调用函数执行，已经实现让ai使用搜索引擎(未发布)

## 功能特性

- **本地 AI 模型**：使用 Ollama 提供的本地 AI 模型进行对话。
- **记忆管理**：通过 mem0 管理用户的聊天记忆，提供更连贯的对话体验。
- **多用户支持**：支持多个用户同时进行对话（测试版存在逻辑问题）。
- **快速响应**：尽量在 5 秒内回复用户，超时情况下会提示用户等待。

## 安装与使用

### 环境要求

- Python 3.7+
- Flask
- FastAPI
- WeChatPy
- Ollama

### 安装步骤

1. 克隆仓库：
    ```bash
    git clone https://github.com/yourusername/ChatMemOllama.git
    cd ChatMemOllama
    ```

2. 安装依赖：
    ```bash
    pip install -r requirements.txt
    ```

3. 配置环境变量：
    ```bash
    export WECHAT_TOKEN='your_wechat_token'
    export APPID='your_appid'
    export APPSECRET='your_appsecret'
    export EncodingAESKey='your_encoding_aes_key'
    ```

4. 运行应用：
    ```bash
    python justchat.py
    ```

## 贡献指南

欢迎任何形式的贡献！请确保在提交 PR 之前阅读以下指南：

1. Fork 仓库并创建一个新的分支。
2. 提交您的修改并推送到您的分支。
3. 创建一个 Pull Request 并描述您的更改。

## 许可证

本项目基于 Apache 2.0 许可证进行分发。详情请参阅 [LICENSE](./LICENSE) 文件。

## 联系方式

如有任何问题或建议，请通过 email 联系我：lightjunction.me@gmail.com
