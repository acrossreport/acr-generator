# ACR Generator

[English](README.md) | [日本語](README.ja.md) | Français

ACR Generator est une application de bureau permettant de créer des modèles de rapports ACR (AcrossReport) (`.acr`).

## Fonctionnalités

- **Deux modes de conception**
  - **Mode Section** : rapports composés de sections telles que l'en-tête, le détail et le pied de page (pour les documents à lignes de détail répétées, comme les bordereaux et les tickets de caisse)
  - **Free Canvas** : conception libre de toute la page, sans sections (pour les étiquettes, etc.)
- Les modèles créés dans l'un ou l'autre mode peuvent être produits par ACR en PDF, en PNG et sur imprimante
- 【要確認: acrpng2json の出力 JSON の取り込みに対応しているか】

## Configuration requise

| OS | Statut |
|---|---|
| Windows x64 | Pris en charge (cette version) |
| macOS (Apple Silicon) | Prévu |
| macOS (Intel) | Prévu |
| Linux x64 | Prévu |

- 【要確認: 対応する Windows のバージョン】
- 【要確認: .NET ランタイムの別途インストールが必要かどうか】

## Téléchargement

Téléchargez le fichier correspondant à votre OS depuis les [Releases](https://github.com/acrossreport/acr-generator/releases).

- Windows x64 : 【要確認: ファイル名】

## Installation et lancement

1. Placez le fichier téléchargé dans le dossier de votre choix 【要確認: 配布形式(単体 exe / zip)。zip の場合は « Extrayez le fichier zip téléchargé » に変更】
2. Lancez `AcrGenerator.exe`

## Utilisation

1. Créez un nouveau modèle et choisissez le mode Section ou Free Canvas 【要確認: 実際の画面上の操作】
2. Placez les contrôles (texte, lignes, images, codes-barres, etc.) 【要確認: 対応コントロールの種類】
3. Enregistrez-le en tant que fichier `.acr`

## Liens

- Spécification ACR (modèle JSON) : https://github.com/acrossreport/acr-spec
- Site officiel : https://acrossreport.com

## Licence

Le code source de ce logiciel n'est pas public. Veuillez consulter le fichier [LICENSE](LICENSE) pour les conditions d'utilisation.

【要確認: 無償利用の可否・登録の要否・ウォーターマークの有無】

## Contact

across.support@gmail.com

---

© Across Systems Corporation
L'architecture d'instructions de dessin intermédiaires d'ACR fait l'objet d'une demande de brevet.
