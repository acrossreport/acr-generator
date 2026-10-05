# ACR Generator

[English](README.md) | 日本語 | [Français](README.fr.md)

ACR Generator は、[acr-png2json](https://github.com/acrossreport/acr-png2json) が帳票の PNG 画像から作成した JSON を読み込み、ACR(AcrossReport)の帳票定義(JSON)を作成するデスクトップアプリケーションです。

## 特長

- acr-png2json が読み取った文字・罫線を画面で確認できます
- **セクション**:読み込んだ内容に、ヘッダー・明細・フッターなどのセクション(帯)を付けて保存します
- **Free Canvas**:セクションを付けずに読み込み結果を確認し、そのまま保存します。部品をクリックすると、読み取った値を確認できます
- グリッド表示、ズーム(Ctrl + マウスホイール)
- 日本語 / English / Français

保存した JSON は AcrossReport Designer で開いて仕上げます。部品の配置・設定や用紙サイズの変更は Designer で行います。

## 動作環境

| OS | 状況 |
|---|---|
| Windows x64 | 対応 |
| macOS(Apple Silicon) | 対応 |
| macOS(Intel) | 対応 |
| Linux x64 | 対応 |

- Windows:Windows 11 以上
- macOS:macOS 14(Sonoma)以上。Developer ID で署名し、Apple の公証を受けています
- Linux:デスクトップ環境が必要です。OpenSSL 3(`libssl.so.3`)が必要で、Ubuntu 22.04 以上には標準で入っています。Ubuntu 24.04 LTS で動作を確認しています
- .NET ランタイムを同梱しているため、別途インストールは不要です

## ダウンロード

[Releases](https://github.com/acrossreport/acr-generator/releases) から、お使いの OS 用のファイルをダウンロードしてください。

| OS | ファイル |
|---|---|
| Windows x64 | `AcrGenerator-v0.0.2-win-x64.zip` |
| macOS(Apple Silicon) | `AcrGenerator-v0.0.2-osx-arm64.zip` |
| macOS(Intel) | `AcrGenerator-v0.0.2-osx-x64.zip` |
| Linux x64 | `AcrGenerator-v0.0.2-linux-x64.zip` |

## インストールと起動

### Windows

1. ダウンロードした zip を任意のフォルダに展開します
2. 展開した `win-x64` フォルダの中の `AcrGenerator.exe` を実行します

### macOS

1. ダウンロードした zip をダブルクリックして、`AcrGenerator.app` を取り出します
2. `AcrGenerator.app` を「アプリケーション」フォルダに移します(任意)
3. `AcrGenerator.app` をダブルクリックします。「インターネットからダウンロードされたアプリケーションです。開いてもよろしいですか?」と表示された場合は「開く」を押します

### Linux

1. ダウンロードした zip を任意のフォルダに展開します
   ```
   unzip AcrGenerator-v0.0.2-linux-x64.zip
   ```
2. 展開した `linux-x64` フォルダの中の `AcrGenerator` を実行します
   ```
   ./linux-x64/AcrGenerator
   ```
   実行権限がなく起動しない場合は、先に `chmod +x linux-x64/AcrGenerator` を実行してください

### ライセンス登録(全 OS 共通)

初回起動時にライセンス登録画面が表示されます。メールアドレスとライセンスキーを入力して「認証する」を押すか、「スキップ(ウォーターマーク付き)」を選びます

## 使い方

1. acr-png2json で、帳票の PNG 画像から JSON を作成します
2. ACR Generator の「PNG-JSON読込」で、その JSON を読み込みます
3. 画面左で「セクション」または「Free Canvas」を選びます
   - セクション:帯の種類を選び、開始位置・終了位置(mm)を指定して「セクション保存」
   - Free Canvas:部品をクリックして読み取った値を確認し、「JSON保存」
4. 保存した JSON を AcrossReport Designer で開きます

読み取り結果がよくない場合は、PNG 画像を撮り直して acr-png2json からやり直してください。

## 関連リンク

- acr-png2json:https://github.com/acrossreport/acr-png2json
- ACR 仕様(JSON テンプレート):https://github.com/acrossreport/acr-spec
- 公式サイト:https://acrossreport.com

## ライセンス

本ソフトウェアのソースコードは公開していません。利用条件は [LICENSE](LICENSE) をご確認ください。

ライセンスキーがなくても、起動時のライセンス登録画面で「スキップ」を選べば利用できます(登録画面は起動のたびに表示されます)。

## お問い合わせ

across.support@gmail.com

---

© Across Systems Corporation
ACR の中間描画命令アーキテクチャは特許出願中です。
