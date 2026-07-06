<p align="center">
  <a href="https://veiltranslate.com">
    <img src="https://veiltranslate.com/logo-mark.png" alt="Veil Translate 标志" width="112">
  </a>
</p>

<h1 align="center">Veil Translate</h1>

<p align="center">
  <a href="./README.md">English</a> ·
  <a href="./README.zh-CN.md">中文</a> ·
  <a href="./README.ko.md">한국어</a> ·
  <a href="./README.ja.md">日本語</a>
</p>

## 中文

**面向保密文档的隐私安全 AI 文档翻译。**

Veil Translate 帮你翻译 Word、Excel、PowerPoint 文件，同时减少敏感实体暴露。文档会在浏览器本地解析，被识别并确认的敏感值会替换为稳定占位符，只有打码文本会发送给你选择的翻译服务；译文返回后，文件会在本地还原并尽量保留原版式。

官网：[veiltranslate.com](https://veiltranslate.com)

### 功能

- 翻译 `.docx`、`.xlsx`、`.pptx` 文件，并保留文档结构与版式。
- 在浏览器内完成解析、敏感实体识别、打码、映射表存储与还原。
- 由浏览器直连你选择的 OpenAI 兼容端点，只发送打码文本和你自己的 API Key。
- 支持简体中文、繁体中文、英语、日语、韩语、法语、德语、西班牙语、俄语。
- 支持一次最多 10 个文件批量翻译，并打包下载 ZIP。
- 支持本地术语库，让指定术语在模型返回后还原为固定译法。

### 工作流程

1. 浏览器读取文档，并提取可翻译文本段。
2. 姓名、证件号、手机号、邮箱、机构名、银行卡样式号码、术语等候选项会进入复核。
3. 你确认的值会替换为 `⟦NAME_1⟧` 或 `⟦TERM_1⟧` 这样的稳定占位符。
4. 浏览器把打码文本发送到你配置的 OpenAI 兼容翻译服务。
5. 翻译完成后，Veil Translate 会检查占位符完整性，在本地还原确认过的值，并写回文档格式。

### 安全边界

Veil Translate 保护的是翻译前被识别并确认的敏感实体。未被打码的其余正文仍会以明文发送给你选择的翻译服务。本产品不是“加密后翻译”。

这个公开仓库只用于放置网站外链所需的产品介绍材料。它不包含应用源码、用户数据、API Key、保密样本文档或实现秘密。
