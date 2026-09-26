# ACR Generator

English | [日本語](README.ja.md) | [Français](README.fr.md)

ACR Generator is a desktop application for creating ACR (AcrossReport) report templates (`.acr`).

## Features

- **Two design modes**
  - **Section mode**: reports built from sections such as header, detail, and footer (for forms with repeating detail rows, such as slips and receipts)
  - **Free Canvas**: design the entire page freely without sections (for labels, etc.)
- Templates created in either mode can be output by ACR to PDF, PNG, and printers
- 【要確認: acrpng2json の出力 JSON の取り込みに対応しているか】

## System Requirements

| OS | Status |
|---|---|
| Windows x64 | Supported (this release) |
| macOS (Apple Silicon) | Planned |
| macOS (Intel) | Planned |
| Linux x64 | Planned |

- 【要確認: 対応する Windows のバージョン】
- 【要確認: .NET ランタイムの別途インストールが必要かどうか】

## Download

Download the file for your OS from [Releases](https://github.com/acrossreport/acr-generator/releases).

- Windows x64: 【要確認: ファイル名】

## Installation and Launch

1. Place the downloaded file in any folder 【要確認: 配布形式(単体 exe / zip)。zip の場合は "Extract the downloaded zip" に変更】
2. Run `AcrGenerator.exe`

## Usage

1. Create a new template and choose Section mode or Free Canvas 【要確認: 実際の画面上の操作】
2. Place controls (text, lines, images, barcodes, etc.) 【要確認: 対応コントロールの種類】
3. Save as an `.acr` file

## Links

- ACR specification (JSON template): https://github.com/acrossreport/acr-spec
- Official website: https://acrossreport.com

## License

The source code of this software is not publicly available. Please see [LICENSE](LICENSE) for the terms of use.

【要確認: 無償利用の可否・登録の要否・ウォーターマークの有無】

## Contact

across.support@gmail.com

---

© Across Systems Corporation
The intermediate drawing instruction architecture of ACR is patent pending.
