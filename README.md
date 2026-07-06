# Veil Translate

**Privacy-safe AI document translation for confidential files.**

Veil Translate helps you translate Word, Excel, and PowerPoint files while reducing the exposure of sensitive entities. Documents are parsed in your browser, detected sensitive values are replaced with stable placeholders, only the masked text is sent to the translation provider you choose, and the translated file is restored locally with its original layout.

Official website: [veiltranslate.com](https://veiltranslate.com)

> Safety boundary: Veil Translate protects the sensitive entities that are detected and confirmed before translation. The remaining non-masked text is still sent as plain text to the translation provider you choose. This is not "encrypted translation".

## What It Does

- Translates `.docx`, `.xlsx`, and `.pptx` files while preserving document structure and layout.
- Runs parsing, sensitive-entity detection, masking, mapping-table storage, and restoration in the browser.
- Sends only masked text plus your own API key directly from your browser to the selected OpenAI-compatible endpoint.
- Supports Simplified Chinese, Traditional Chinese, English, Japanese, Korean, French, German, Spanish, and Russian.
- Supports batch translation of up to 10 files with ZIP download.
- Includes a local terminology glossary so selected terms can be replaced with fixed translations after the model returns.

## How It Works

1. **Local parsing**
   Your browser reads the document and extracts translatable text segments. The original file does not need to be uploaded to a Veil Translate server.

2. **Review and masking**
   Detected names, IDs, phone numbers, emails, organizations, bank-like numbers, and glossary terms are shown for review. Confirmed values are replaced with stable placeholders such as `⟦NAME_1⟧` or `⟦TERM_1⟧`.

3. **Browser-direct translation**
   The browser sends the masked text to the OpenAI-compatible provider you configure. Your API key is carried only in the request from your browser to that provider.

4. **Local restoration**
   After translation, Veil Translate checks placeholder integrity, restores confirmed sensitive values or glossary translations locally, and writes the result back into the document format.

## Product Principles

- No server-side translation proxy.
- No upload of original documents to a Veil Translate application server.
- No server-side handling of plaintext sensitive data, passwords, derived keys, or API keys.
- Stable placeholders for reversible pseudonymization; WebCrypto is used only for local encrypted storage.
- Clear user-facing boundary: masked entities are protected, but non-masked body text still leaves the browser as plain text.

## 中文简介

**Veil Translate 是一个面向保密文档的匿名化 AI 翻译工具。**

它在浏览器本地解析 Word / Excel / PowerPoint 文件，先把你确认过的姓名、证件号、手机号、邮箱、机构名、术语等敏感实体替换成稳定占位符，再由浏览器直连你选择的 OpenAI 兼容翻译端点。译文返回后，占位符会在本地还原，并尽量保留原文档版式。

官网：[veiltranslate.com](https://veiltranslate.com)

安全边界：Veil Translate 保护的是被识别并确认的敏感实体；去除这些实体后的正文仍会以明文发送给你选择的翻译服务。本产品不应被理解为“加密后翻译”。

## Repository Scope

This public repository is intentionally limited to product introduction material for website linking. It does not contain the application source code, user data, API keys, sample confidential documents, or implementation secrets.
