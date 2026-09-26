# ACR Generator

[English](README.md) | 日本語 | [Français](README.fr.md)

ACR Generator は、ACR(AcrossReport)の帳票テンプレート(`.acr`)を作成するデスクトップアプリケーションです。

## 特長

- **2つのデザインモード**
  - **セクション型**: ヘッダー・明細・フッターなどのセクションで構成する帳票(伝票・レシートなど、明細を繰り返す帳票向け)
  - **Free Canvas**: セクションを使わず、紙面全体を自由にデザインする方式(ラベルなど向け)
- どちらのモードで作成したテンプレートも、ACR で PDF・PNG・プリンタへ出力できます
- 【要確認: acrpng2json の出力 JSON の取り込みに対応しているか】

## 動作環境

| OS | 状況 |
|---|---|
| Windows x64 | 対応(本リリース) |
| macOS(Apple Silicon) | 対応予定 |
| macOS(Intel) | 対応予定 |
| Linux x64 | 対応予定 |

- 【要確認: 対応する Windows のバージョン】
- 【要確認: .NET ランタイムの別途インストールが必要かどうか】

## ダウンロード

[Releases](https://github.com/acrossreport/acr-generator/releases) から、お使いの OS 用のファイルをダウンロードしてください。

- Windows x64: 【要確認: ファイル名】

## インストールと起動

1. ダウンロードしたファイルを任意のフォルダに置きます 【要確認: 配布形式(単体 exe / zip)。zip の場合は「展開します」に変更】
2. `AcrGenerator.exe` を実行します

## 使い方

1. 新規作成で、セクション型または Free Canvas を選びます 【要確認: 実際の画面上の操作】
2. コントロール(テキスト・線・画像・バーコードなど)を配置します 【要確認: 対応コントロールの種類】
3. `.acr` ファイルとして保存します

## 関連リンク

- ACR 仕様(JSON テンプレート): https://github.com/acrossreport/acr-spec
- 公式サイト: https://acrossreport.com

## ライセンス

本ソフトウェアのソースコードは公開していません。利用条件は [LICENSE](LICENSE) をご確認ください。

【要確認: 無償利用の可否・登録の要否・ウォーターマークの有無】

## お問い合わせ

across.support@gmail.com

---

© Across Systems Corporation
ACR の中間描画命令アーキテクチャは特許出願中です。
