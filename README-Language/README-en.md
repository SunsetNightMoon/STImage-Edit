---
title: STImage Edit Support - English
language: English
---

# STImage Edit Support

A VSCode extension providing syntax highlighting for STImage format files used in the SillyTavern scenario "Blue Archive: New Dawn".
Compatible with version 1.2 of "Blue Archive: New Dawn" new text format for convenient editing.
Compatible with Visual Studio Code, Trae CN and other editors supporting vsix installation.

## Language Switch 🌐
| Language | File |
|----------|------|
| 中文 | [README.md](../README.md) |
| English | [README-en.md](README-en.md) |
| 日本語 | [README-ja.md](README-ja.md) |
| 한국어 | [README-ko.md](README-ko.md) |

## Features

- Syntax highlighting for STImage format `.stim` files
- Supports multiple file formats:
  - Character expression format with quotes and numbers (version 1.2)
  - Background image format without quotes and numbers
- Custom color theme for clear element distinction
- Optimized for editing "Blue Archive: New Dawn" scenario resources

## Installation

### Method 1: Install from local file

1. Open VSCode/Trae CN
2. Press `Ctrl+Shift+P` to open command palette
3. Type "Extensions: Install from VSIX..."
4. Select `STImage-Edit-1.4.1.vsix` file

### Method 2: Development mode

1. Open the `ba-stimage-editingsupport` folder in editor
2. Press `F5` to launch Extension Development Host
3. Extension will load automatically in new window

### Method 3: VSCode Trae CN simple graphical installation

1. Open VSCode/Trae CN
2. Click the Extensions icon
3. Click ⋯ (More) in the top-right corner → Install from VSIX...
4. Select `STImage-Edit-1.4.1.vsix` file


## Usage

1. After installing the extension, open any `.stim` file
2. Click the language selector in the bottom-right corner
3. Select **"STImage"** language mode
4. Syntax highlighting will be applied automatically
5. Must use the built-in **"STImage Theme"** for proper display

## File Format Support

The extension supports syntax highlighting for the following formats:

### Format 1 (with quotes and numbers) - Version 1.2

```
<"星野_正常":"01"|https://xxxx.xxxxxx.xxx/xxxxx.png>
<"梦前辈_笑A":"00"|https://xxxx.xxxxxx.xxx/xxxxx.png>
```

### Format 2 (without quotes and numbers) - Background format

```
<基沃托斯城市_正常|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
<阿拜多斯会议室_夜晚|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
```

### Divider Line

```
———————————————————————————————————————
```

## Color Reference

| Element | Color | Description |
|---------|-------|-------------|
| Character Name (quoted) | Light Blue | e.g., 星野_正常 |
| Background Name (unquoted) | Purple | e.g., 基沃托斯城市_正常 |
| Expression Number | Pink | e.g., 01 |
| URL Link | Editor Default | Underlined link style |
| Delimiters | Gray | `< > : \|` |
| Divider Line | Green | —————— |

## Development

To modify colors or syntax rules, edit the following files:

- `themes/stimage-theme.json` - Color theme configuration
- `syntaxes/stimage.tmLanguage.json` - Syntax rule definitions
- `package.json` - Extension configuration

## Developer

**暮落夜月**

[![Bilibili](https://img.shields.io/badge/Bilibili-暮落夜月-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/175546011)
[![Github](https://img.shields.io/badge/Github-SunsetNightMoon-181717?style=flat-square&logo=github)](https://github.com/SunsetNightMoon)

## Scenario Developer

**二次元绝缘体**

[![Bilibili](https://img.shields.io/badge/Bilibili-二次元绝缘体-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/6009407)

## Disclaimer

This extension only provides syntax highlighting for the specific STImage format (`.stim`) files and does not involve the "Blue Archive" game itself or any related art resources.

The development of this extension is not affiliated with NEXON Games, MX studio, or Yostar Pictures, and no art resources from them were used.

"Blue Archive" and its related resources are copyrighted by NEXON Games, MX studio, and Yostar Pictures.

## Development Notes

This project used AI tools during development.

## Modification Notice

According to GPL v3 requirements:
- This project is open source software and can be freely modified and distributed
- Modified versions must:
  1. Be clearly marked as modified versions
  2. Include modification date and content
  3. Retain all original license notices
- See the [GPL v3 License](../LICENSE) for complete terms

## License

[GPL v3](../LICENSE)
