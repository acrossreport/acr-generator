# ACR Generator

English | [日本語](README.ja.md) | [Français](README.fr.md)

ACR Generator is a desktop application that loads the JSON created by [acr-png2json](https://github.com/acrossreport/acr-png2json) from a PNG image of a business form, and creates an ACR (AcrossReport) report definition (JSON).

## Features

- Check the text and ruled lines read by acr-png2json on screen
- **Section**: add sections (bands) such as header, detail, and footer to the loaded content, then save
- **Free Canvas**: check the loaded result without sections and save it as is. Click a control to see the values that were read
- Grid display and zoom (Ctrl + mouse wheel)
- Japanese / English / Français

Open the saved JSON in AcrossReport Designer to finish it. Placing and configuring controls and changing the paper size are done in Designer.

## System Requirements

| OS | Status |
|---|---|
| Windows x64 | Supported |
| macOS (Apple Silicon) | Supported |
| macOS (Intel) | Supported |
| Linux x64 | Supported |

- Windows: Windows 11 or later
- macOS: macOS 14 (Sonoma) or later. The app is signed with a Developer ID and notarized by Apple
- Linux: a desktop environment is required. OpenSSL 3 (`libssl.so.3`) is required; it is included in Ubuntu 22.04 or later. Tested on Ubuntu 24.04 LTS
- The .NET runtime is included, so no separate installation is required

## Download

Download the file for your OS from [Releases](https://github.com/acrossreport/acr-generator/releases).

| OS | File |
|---|---|
| Windows x64 | `AcrGenerator-v0.0.2-win-x64.zip` |
| macOS (Apple Silicon) | `AcrGenerator-v0.0.2-osx-arm64.zip` |
| macOS (Intel) | `AcrGenerator-v0.0.2-osx-x64.zip` |
| Linux x64 | `AcrGenerator-v0.0.2-linux-x64.zip` |

## Installation and Launch

### Windows

1. Extract the downloaded zip to any folder
2. Run `AcrGenerator.exe` in the extracted `win-x64` folder

### macOS

1. Double-click the downloaded zip to extract `AcrGenerator.app`
2. Move `AcrGenerator.app` to the Applications folder (optional)
3. Double-click `AcrGenerator.app`. If macOS asks whether to open an app downloaded from the Internet, click "Open"

### Linux

1. Extract the downloaded zip to any folder
   ```
   unzip AcrGenerator-v0.0.2-linux-x64.zip
   ```
2. Run `AcrGenerator` in the extracted `linux-x64` folder
   ```
   ./linux-x64/AcrGenerator
   ```
   If it does not start because of missing execute permission, run `chmod +x linux-x64/AcrGenerator` first

### License registration (all OS)

On first launch, the license registration screen appears. Enter your email address and license key and click "Authenticate", or choose "Skip (with watermark)"

## Usage

1. Use acr-png2json to create JSON from a PNG image of a business form
2. Load that JSON with "Import PNG-JSON" in ACR Generator
3. Choose "Section" or "FreeCanvas" on the left side of the screen
   - Section: choose a band type, specify the start and end positions (mm), and click "Save Sections"
   - Free Canvas: click controls to check the values that were read, then click "Save JSON"
4. Open the saved JSON in AcrossReport Designer

If the recognition result is poor, retake the PNG image and start again from acr-png2json.

## Links

- acr-png2json: https://github.com/acrossreport/acr-png2json
- ACR specification (JSON template): https://github.com/acrossreport/acr-spec
- Official website: https://acrossreport.com

## License

The source code of this software is not publicly available. Please see [LICENSE](LICENSE) for the terms of use.

You can use the software without a license key by choosing "Skip" on the license registration screen at startup (the registration screen appears each time you launch the software).

## Contact

across.support@gmail.com

---

© Across Systems Corporation
The intermediate drawing instruction architecture of ACR is patent pending.
