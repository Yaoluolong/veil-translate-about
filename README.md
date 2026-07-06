<p align="center">
  <a href="https://veiltranslate.com">
    <img src="https://veiltranslate.com/logo-mark.png" alt="Veil Translate logo" width="112">
  </a>
</p>

<h1 align="center">Veil Translate</h1>

<p align="center">
  <a href="#english">English</a> ·
  <a href="#chinese">中文</a> ·
  <a href="#korean">한국어</a> ·
  <a href="#japanese">日本語</a>
</p>

<a id="english"></a>

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

<a id="chinese"></a>

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

<a id="korean"></a>

## 한국어

**기밀 문서를 위한 개인정보 보호형 AI 문서 번역 도구입니다.**

Veil Translate는 Word, Excel, PowerPoint 파일을 번역하면서 민감한 항목의 노출을 줄입니다. 문서는 브라우저 안에서 파싱되고, 감지된 민감 값은 안정적인 자리표시자로 바뀝니다. 선택한 번역 제공업체에는 마스킹된 텍스트만 전송되며, 번역된 파일은 브라우저에서 원래 레이아웃에 맞게 복원됩니다.

공식 웹사이트: [veiltranslate.com](https://veiltranslate.com)

### 주요 기능

- `.docx`, `.xlsx`, `.pptx` 파일을 문서 구조와 레이아웃을 유지한 채 번역합니다.
- 파싱, 민감 항목 감지, 마스킹, 매핑 테이블 저장, 복원을 브라우저 안에서 처리합니다.
- 브라우저가 사용자가 선택한 OpenAI 호환 엔드포인트로 직접 연결하며, 마스킹된 텍스트와 사용자의 API Key만 전송합니다.
- 중국어 간체, 중국어 번체, 영어, 일본어, 한국어, 프랑스어, 독일어, 스페인어, 러시아어를 지원합니다.
- 최대 10개 파일의 일괄 번역과 ZIP 다운로드를 지원합니다.
- 로컬 용어집을 통해 지정한 용어를 모델 응답 후 고정 번역어로 복원할 수 있습니다.

### 작동 방식

1. 브라우저가 문서를 읽고 번역 가능한 텍스트 구간을 추출합니다.
2. 이름, 신분증 번호, 전화번호, 이메일, 조직명, 은행 번호 형식의 값, 용어집 항목이 검토 대상으로 표시됩니다.
3. 사용자가 확인한 값은 `⟦NAME_1⟧` 또는 `⟦TERM_1⟧` 같은 안정적인 자리표시자로 바뀝니다.
4. 브라우저가 마스킹된 텍스트를 사용자가 설정한 OpenAI 호환 번역 서비스로 보냅니다.
5. 번역 후 Veil Translate는 자리표시자의 무결성을 확인하고, 확인된 값을 브라우저에서 복원한 뒤 문서 형식으로 다시 씁니다.

### 안전 경계

Veil Translate는 번역 전에 감지되고 사용자가 확인한 민감 항목을 보호합니다. 마스킹되지 않은 나머지 본문은 사용자가 선택한 번역 서비스로 평문 전송됩니다. 이 제품은 암호화 번역이 아닙니다.

이 공개 저장소는 웹사이트 외부 링크에 사용할 제품 소개 자료만 담고 있습니다. 애플리케이션 소스 코드, 사용자 데이터, API Key, 기밀 샘플 문서, 구현 비밀은 포함하지 않습니다.

<a id="japanese"></a>

## 日本語

**機密文書向けのプライバシー保護型 AI 文書翻訳ツールです。**

Veil Translate は、Word、Excel、PowerPoint ファイルを翻訳しながら、機密性の高いエンティティの露出を減らします。文書はブラウザ内で解析され、検出された機密値は安定したプレースホルダーに置き換えられます。選択した翻訳プロバイダーにはマスク済みテキストだけが送信され、翻訳後のファイルはブラウザ内で元のレイアウトに沿って復元されます。

公式サイト：[veiltranslate.com](https://veiltranslate.com)

### 主な機能

- `.docx`、`.xlsx`、`.pptx` ファイルを文書構造とレイアウトを保ったまま翻訳します。
- 解析、機密エンティティ検出、マスキング、対応表の保存、復元をブラウザ内で処理します。
- ブラウザが選択された OpenAI 互換エンドポイントへ直接接続し、マスク済みテキストとユーザー自身の API Key だけを送信します。
- 簡体字中国語、繁体字中国語、英語、日本語、韓国語、フランス語、ドイツ語、スペイン語、ロシア語に対応します。
- 最大 10 ファイルの一括翻訳と ZIP ダウンロードに対応します。
- ローカル用語集により、指定した用語をモデル応答後に固定訳語として復元できます。

### 仕組み

1. ブラウザが文書を読み込み、翻訳可能なテキスト区間を抽出します。
2. 氏名、ID、電話番号、メールアドレス、組織名、銀行番号のような値、用語集項目が確認対象として表示されます。
3. ユーザーが確認した値は `⟦NAME_1⟧` や `⟦TERM_1⟧` のような安定したプレースホルダーに置き換えられます。
4. ブラウザがマスク済みテキストを、ユーザーが設定した OpenAI 互換翻訳サービスへ送信します。
5. 翻訳後、Veil Translate はプレースホルダーの完全性を確認し、確認済みの値をブラウザ内で復元して文書形式へ書き戻します。

### 安全上の境界

Veil Translate が保護するのは、翻訳前に検出され、ユーザーが確認した機密エンティティです。マスクされていない残りの本文は、ユーザーが選択した翻訳サービスへ平文で送信されます。この製品は暗号化翻訳ではありません。

この公開リポジトリは、ウェブサイトからリンクするための製品紹介資料だけを置く場所です。アプリケーションのソースコード、ユーザーデータ、API Key、機密サンプル文書、実装上の秘密は含まれていません。
