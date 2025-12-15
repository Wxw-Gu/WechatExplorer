# WechatExplorer

MAC系统 获取微信聊天记录 AI一键生成群聊总结
它支持查看解密后的微信数据库内容，提供聊天记录搜索、导出以及 AI 智能总结功能。

## 📸 预览

<div style="display: flex; justify-content: space-between;">
  <img src="./public/WX20251215-155324.png" alt="预览图1" width="48%" />
  <img src="./public/WX20251215-155524.png" alt="预览图2" width="48%" />
</div>

## ✨ 功能特性

- **聊天记录查看**: 浏览微信好友和群聊的聊天记录。
- **全局搜索**: 快速搜索聊天内容。
- **AI 智能总结**: 集成 DeepSeek AI，一键总结群聊精华内容，生成话题报告。
- **图片生成**: 将 AI 总结的内容生成精美图片，方便分享。
- **数据导出**: 支持导出聊天记录为 CSV 文件（今日、昨日、近7天或全部）。
- **安全隐私**: 所有数据仅在本地处理，AI 功能需自行配置 API Key。

## 🛠️ 技术栈

- **Electron**: 跨平台桌面应用框架
- **React**: 用于构建用户界面
- **TypeScript**: 提供类型安全
- **Vite**: 极速构建工具
- **Better-SQLite3**: 高性能 SQLite 数据库操作
- **OpenAI SDK**: 用于调用 DeepSeek API

## 🚀 快速开始

### 前置要求

- 微信<=4.0 需要获取自己微信本地数据库的密码， 获取方式参考： [Mac 导出微信聊天记录](https://blog.vcvit.me/2024/08/02/mac-export-wechat-chat-records/)
- 如果无法获取本地数据库密码 则无法使用当前项目
- Node.js (推荐 v16+)
- pnpm (推荐) 或 npm
- 解密后的微信数据库文件 (`.db`) 和对应的密钥
- [DeepSeek API Key](https://www.deepseek.com/) (用于 AI 总结功能)

### 安装

```bash
# 克隆项目
git clone https://github.com/your-username/WechatExplorer.git

# 进入目录
cd WechatExplorer

# 安装依赖
pnpm install
```

### 配置

复制 `.env.example` 文件为 `.env`，并填写相关配置（可选，也可以在应用内设置）：

```bash
cp .env.example .env
```

### 开发模式运行

```bash
pnpm dev
```

### 打包构建

```bash
# Windows
pnpm build:win

# macOS
pnpm build:mac

# Linux
pnpm build:linux
```

## ⚠️ 免责声明

本项目仅供学习和研究使用。请勿用于非法用途。开发者不对使用本项目造成的任何后果负责。请遵守相关法律法规和微信使用协议。

## 📄 许可证

[MIT](./LICENSE) License

## 🔗 参考

- [WechatMessageExplorer](https://github.com/svcvit/WechatMessageExplorer)
