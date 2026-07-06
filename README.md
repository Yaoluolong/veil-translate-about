<p align="center">
  <a href="https://veiltranslate.com">
    <img src="https://veiltranslate.com/logo-mark.png" alt="Veil Translate logo" width="112">
  </a>
</p>

<h1 align="center">Veil Translate</h1>

<p align="center">
  <a href="./README.md">English</a> ·
  <a href="./README.zh-CN.md">中文</a> ·
  <a href="./README.ko.md">한국어</a> ·
  <a href="./README.ja.md">日本語</a>
</p>

## English

**Privacy-safe AI document translation for confidential files.**

Veil Translate helps you translate Word, Excel, and PowerPoint files while reducing the exposure of sensitive entities. Documents are parsed in your browser, detected sensitive values are replaced with stable placeholders, only the masked text is sent to the translation provider you choose, and the translated file is restored locally with its original layout.

Official website: [veiltranslate.com](https://veiltranslate.com)

### What It Does

- Translates `.docx`, `.xlsx`, and `.pptx` files while preserving document structure and layout.
- Runs parsing, sensitive-entity detection, masking, mapping-table storage, and restoration in the browser.
- Sends only masked text plus your own API key directly from your browser to the selected OpenAI-compatible endpoint.
- Supports Simplified Chinese, Traditional Chinese, English, Japanese, Korean, French, German, Spanish, and Russian.
- Supports batch translation of up to 10 files with ZIP download.
- Includes a local terminology glossary so selected terms can be replaced with fixed translations after the model returns.

### How It Works

1. Your browser reads the document and extracts translatable text segments.
2. Detected names, IDs, phone numbers, emails, organizations, bank-like numbers, and glossary terms are shown for review.
3. Confirmed values are replaced with stable placeholders such as `⟦NAME_1⟧` or `⟦TERM_1⟧`.
4. The browser sends the masked text to the OpenAI-compatible provider you configure.
5. After translation, Veil Translate checks placeholder integrity, restores confirmed values locally, and writes the result back into the document format.

### Safety Boundary

Veil Translate protects the sensitive entities that are detected and confirmed before translation. The remaining non-masked text is still sent as plain text to the translation provider you choose. This is not encrypted translation.

This public repository is intentionally limited to product introduction material for website linking. It does not contain the application source code, user data, API keys, sample confidential documents, or implementation secrets.
