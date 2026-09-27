# ACR Generator

[English](README.md) | [日本語](README.ja.md) | Français

ACR Generator est une application de bureau qui charge le JSON créé par [acrpng2json](https://github.com/acrossreport/acrpng2json) à partir d'une image PNG d'un document, et crée une définition de rapport ACR (AcrossReport) au format JSON.

## Fonctionnalités

- Vérification à l'écran du texte et des lignes lus par acrpng2json
- **Section** : ajout de sections (bandes) telles que l'en-tête, le détail et le pied de page au contenu chargé, puis enregistrement
- **Free Canvas** : vérification du résultat chargé sans sections et enregistrement tel quel. Cliquez sur un contrôle pour voir les valeurs lues
- Affichage de la grille et zoom (Ctrl + molette de la souris)
- Japonais / English / Français

Ouvrez le JSON enregistré dans AcrossReport Designer pour le finaliser. Le placement et le réglage des contrôles ainsi que le changement de format de papier se font dans Designer.

## Configuration requise

| OS | Statut |
|---|---|
| Windows x64 | Pris en charge (cette version) |
| macOS (Apple Silicon) | Prévu |
| macOS (Intel) | Prévu |
| Linux x64 | Prévu |

- Versions de Windows prises en charge : 【要確認】
- Le runtime .NET est inclus ; aucune installation séparée n'est nécessaire

## Téléchargement

Téléchargez le fichier correspondant à votre OS depuis les [Releases](https://github.com/acrossreport/acr-generator/releases).

- Windows x64 : `AcrGenerator-v0.0.1-win-x64.zip`

## Installation et lancement

1. Extrayez le fichier zip téléchargé dans le dossier de votre choix
2. Lancez `AcrGenerator.exe` dans le dossier extrait
3. Au premier lancement, l'écran d'enregistrement de la licence s'affiche. Saisissez votre adresse e-mail et votre clé de licence, puis cliquez sur « Authentifier », ou choisissez « Ignorer (avec filigrane) »

## Utilisation

1. Créez un JSON à partir d'une image PNG d'un document avec acrpng2json
2. Chargez ce JSON avec « Importer JSON » dans ACR Generator
3. Choisissez « Section » ou « FreeCanvas » à gauche de l'écran
   - Section : choisissez un type de bande, indiquez les positions de début et de fin (mm), puis cliquez sur « Enregistrer les sections »
   - Free Canvas : cliquez sur les contrôles pour vérifier les valeurs lues, puis cliquez sur « Enregistrer JSON »
4. Ouvrez le JSON enregistré dans AcrossReport Designer

Si le résultat de la lecture n'est pas satisfaisant, reprenez l'image PNG et recommencez à partir d'acrpng2json.

## Liens

- acrpng2json : https://github.com/acrossreport/acrpng2json
- Spécification ACR (modèle JSON) : https://github.com/acrossreport/acr-spec
- Site officiel : https://acrossreport.com

## Licence

Le code source de ce logiciel n'est pas public. Veuillez consulter le fichier [LICENSE](LICENSE) pour les conditions d'utilisation.

Vous pouvez utiliser le logiciel sans clé de licence en choisissant « Ignorer » sur l'écran d'enregistrement de la licence au démarrage (cet écran s'affiche à chaque lancement).

## Contact

across.support@gmail.com

---

© Across Systems Corporation
L'architecture d'instructions de dessin intermédiaires d'ACR fait l'objet d'une demande de brevet.
