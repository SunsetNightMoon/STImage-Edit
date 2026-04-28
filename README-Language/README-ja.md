---
title: STImage Edit Support - 日本語
language: Japanese
---

# STImage Edit Support

SillyTavernのシナリオ「ブルーアーカイブ：新生黎明」で使用されるSTImage形式ファイルの構文強調表示を提供するVSCode拡張機能です。
「ブルーアーカイブ：新生黎明」1.2版の新しいテキスト形式に対応し、編集を便利にします。
Visual Studio Code、Trae CNなどのvsixインストールに対応したエディターで使用可能です。

## 言語切り替え 🌐
| 言語 | ファイル |
|------|----------|
| 中文 | [README.md](../README.md) |
| English | [README-en.md](README-en.md) |
| 日本語 | [README-ja.md](README-ja.md) |
| 한국어 | [README-ko.md](README-ko.md) |

## 機能

- STImage形式の `.stim` ファイルの構文強調表示
- 複数のファイル形式をサポート：
  - 引用符と番号付きのキャラクター表情形式（1.2版）
  - 引用符と番号なしの背景画像形式
- 要素を明確に区別するカスタムカラーテーマ
- 「ブルーアーカイブ：新生黎明」シナリオリソースの編集に最適化

## インストール方法

### 方法1：ローカルファイルからインストール

1. VSCode/Trae CNを開く
2. `Ctrl+Shift+P` を押してコマンドパレットを開く
3. 「Extensions: Install from VSIX...」と入力
4. `STImage-Edit-1.4.1.vsix` ファイルを選択

### 方法2：開発モードでインストール

1. エディターで `ba-stimage-editingsupport` フォルダを開く
2. `F5` を押して拡張機能開発ホストを起動
3. 新しいウィンドウで拡張機能が自動的に読み込まれる

### 方法3：VSCode Trae CN専用の簡単なグラフィカルインストール方法

1. VSCode/Trae CNを開く
2. 拡張機能アイコンをクリック
3. 拡張機能画面の右上 ⋯ (その他) → VSIXからインストール...
4. `STImage-Edit-1.4.1.vsix` ファイルを選択


## 使用方法

1. 拡張機能をインストール後、任意の `.stim` ファイルを開く
2. 右下の言語モードセレクターをクリック
3. **「STImage」** 言語モードを選択
4. ファイルに自動的に構文強調表示が適用される
5. 正常に表示するには組み込みの **「STImage Theme」** を使用する必要があります

## ファイル形式サポート

拡張機能は以下の形式の構文強調表示をサポートします：

### 形式1（引用符と番号付き）- 1.2版新形式

```
<"星野_正常":"01"|https://xxxx.xxxxxx.xxx/xxxxx.png>
<"夢先輩_笑A":"00"|https://xxxx.xxxxxx.xxx/xxxxx.png>
```

### 形式2（引用符と番号なし）- 背景画像形式

```
<基沃托斯城市_正常|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
<阿拜多斯会议室_夜晚|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
```

### 区切り線

```
———————————————————————————————————————
```

## 色の説明

| 要素 | 色 | 説明 |
|------|------|------|
| キャラクター名（引用符付き） | 水色 | 例：星野_正常 |
| 背景名（引用符なし） | 紫色 | 例：基沃托斯城市_正常 |
| 表情番号 | ピンク | 例：01 |
| URLリンク | エディターデフォルト | 下線付きリンクスタイル |
| 区切り文字 | 灰色 | `< > : \|` |
| 区切り線 | 緑色 | —————— |

## 開発

色または構文規則を変更するには、以下のファイルを編集します：

- `themes/stimage-theme.json` - カラーテーマ設定
- `syntaxes/stimage.tmLanguage.json` - 構文規則定義
- `package.json` - 拡張機能設定

## 開発者

**暮落夜月**

[![Bilibili](https://img.shields.io/badge/Bilibili-暮落夜月-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/175546011)
[![Github](https://img.shields.io/badge/Github-SunsetNightMoon-181717?style=flat-square&logo=github)](https://github.com/SunsetNightMoon)

## シナリオ開発者

**二次元绝缘体**

[![Bilibili](https://img.shields.io/badge/Bilibili-二次元绝缘体-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/6009407)

## 免責事項

この拡張機能は特定のSTImage形式（`.stim`）ファイルの構文強調表示機能のみを提供し、「ブルーアーカイブ」ゲーム本体または関連する美術リソースには関係ありません。

この拡張機能の開発はNEXON Games、MX studio、Yostar Picturesとは関係ありません。それらの美術リソースは使用していません。

「ブルーアーカイブ」および関連リソースの著作権はNEXON Games、MX studio、Yostar Picturesに帰属します。

## 開発について

このプロジェクトは開発中にAIツールを使用しました。

## 改変声明

GPL v3の要件に従い：
- このプロジェクトはオープンソースソフトウェアであり、自由に改変および配布可能です
- 改変したバージョンは以下の条件を満たす必要があります：
  1. 改変バージョンであることを明確に表示
  2. 改変日時および内容を明記
  3. すべての元のライセンス声明を保持
- 完全な条項は [GPL v3 ライセンス](../LICENSE) を参照してください

## ライセンス

[GPL v3](../LICENSE)
