# ACR Generator

[English](README.md) | 日本語 | [Français](README.fr.md)

ACR Generator は、[acrpng2json](https://github.com/acrossreport/acrpng2json) が帳票の PNG 画像から作成した JSON を読み込み、ACR(AcrossReport)の帳票定義(JSON)を作成するデスクトップアプリケーションです。

## 特長

- acrpng2json が読み取った文字・罫線を画面で確認できます
- **セクション**:読み込んだ内容に、ヘッダー・明細・フッターなどのセクション(帯)を付けて保存します
- **Free Canvas**:セクションを付けずに読み込み結果を確認し、そのまま保存します。部品をクリックすると、読み取った値を確認できます
- グリッド表示、ズーム(Ctrl + マウスホイール)
- 日本語 / English / Français

保存した JSON は AcrossReport Designer で開いて仕上げます。部品の配置・設定や用紙サイズの変更は Designer で行います。

## 動作環境

| OS | 状況 |
|---|---|
| Windows x64 | 対応(本リリース) |
| macOS(Apple Silicon) | 対応予定 |
| macOS(Intel) | 対応予定 |
| Linux x64 | 対応予定 |

- 対応する Windows のバージョン:【要確認】
- .NET ランタイムを同梱しているため、別途インストールは不要です

## ダウンロード

[Releases](https://github.com/acrossreport/acr-generator/releases) から、お使いの OS 用のファイルをダウンロードしてください。

- Windows x64:`AcrGenerator-v0.0.1-win-x64.zip`

## インストールと起動

1. ダウンロードした zip を任意のフォルダに展開します
2. 展開したフォルダの中の `AcrGenerator.exe` を実行します
3. 初回起動時にライセンス登録画面が表示されます。メールアドレスとライセンスキーを入力して「認証する」を押すか、「スキップ(ウォーターマーク付き)」を選びます

## 使い方

1. acrpng2json で、帳票の PNG 画像から JSON を作成します
2. ACR Generator の「PNG-JSON読込」で、その JSON を読み込みます
3. 画面左で「セクション」または「Free Canvas」を選びます
   - セクション:帯の種類を選び、開始位置・終了位置(mm)を指定して「セクション保存」
   - Free Canvas:部品をクリックして読み取った値を確認し、「JSON保存」
4. 保存した JSON を AcrossReport Designer で開きます

読み取り結果がよくない場合は、PNG 画像を撮り直して acrpng2json からやり直してください。

## 関連リンク

- acrpng2json:https://github.com/acrossreport/acrpng2json
- ACR 仕様(JSON テンプレート):https://github.com/acrossreport/acr-spec
- 公式サイト:https://acrossreport.com

## ライセンス

本ソフトウェアのソースコードは公開していません。利用条件は [LICENSE](LICENSE) をご確認ください。

【要確認: 無償利用の可否・登録の要否・ウォーターマークの対象】

## お問い合わせ

across.support@gmail.com

---

© Across Systems Corporation
ACR の中間描画命令アーキテクチャは特許出願中です。
