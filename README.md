# 碧蓝档案：新生黎明 格式编辑支持扩展

## 语言切换 🌐
| 语言 | 文件 |
|------|------|
| 中文 | [README.md](README.md) |
| English | [README-en.md](README-Language/README-en.md) |
| 日本語 | [README-ja.md](README-Language/README-ja.md) |
| 한국어 | [README-ko.md](README-Language/README-ko.md) |

专门为SillyTavern的剧本《碧蓝档案：新生黎明》开发的STImage格式文件提供语法高亮的VSCode扩展。
兼容1.2版《碧蓝档案：新生黎明》新文本格式提供便捷编辑。
兼容Visual Studio Code、Trae CN等支持vsix安装的编辑器。

## 功能特性

- 为STImage格式的 `.stim` 文件提供语法高亮
- 支持多种文件格式：
  - 带引号和序号的角色表情格式（1.2新版本）
  - 不带引号和序号的背景图格式
- 自定义颜色主题，清晰区分不同元素
- 专为《碧蓝档案：新生黎明》剧本资源编辑优化

## 安装方法

### 方法1：从本地安装

1. 打开VSCode/Trae CN
2. 按 `Ctrl+Shift+P` 打开命令面板
3. 输入 "Extensions: Install from VSIX..."
4. 选择 `ba-stimage-editingsupport.vsix` 文件

### 方法2：开发模式安装

1. 在编辑器中打开 `ba-stimage-editingsupport` 文件夹
2. 按 `F5` 启动扩展开发主机
3. 在新打开的窗口中，扩展会自动加载

### 方法3：VSCode Trae CN特有简单图形化安装方式

1. 打开VSCode/Trae CN
2. 点击扩展图标
3. 点击扩展界面的右上角 ⋯ (更多) → 从 VSIX 安装...
4. 选择 `ba-stimage-editingsupport.vsix` 文件


## 使用说明

1. 安装扩展后，打开任意 `.stim` 文件
2. 点击右下角的语言模式选择器
3. 选择 **"STImage"** 语言模式
4. 文件将自动应用语法高亮
5. 必须搭配内置的主题 **"STImage Theme"** 才能正常显示

## 文件格式支持

扩展支持以下格式的语法高亮：

### 格式1（带引号和序号）- 1.2版新格式

```
<"星野_正常":"01"|https://xxxx.xxxxxx.xxx/xxxxx.png>
<"梦前辈_笑A":"00"|https://xxxx.xxxxxx.xxx/xxxxx.png>
```

### 格式2（不带引号和序号）- 背景图格式

```
<基沃托斯城市_正常|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
<阿拜多斯会议室_夜晚|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
```

### 分隔线

```
———————————————————————————————————————
```

## 颜色说明

| 元素 | 颜色 | 说明 |
|------|------|------|
| 角色名称（带引号） | 水蓝色 | 如：星野_正常 |
| 背景名称（不带引号） | 紫色 | 如：基沃托斯城市_正常 |
| 表情编号 | 粉色 | 如：01 |
| URL链接 | 编辑器默认 | 带下划线的链接样式 |
| 分隔符 | 灰色 | `< > : \|` |
| 分隔线 | 绿色 | —————— |

## 开发

如需修改颜色或语法规则，编辑以下文件：

- `themes/stimage-theme.json` - 颜色主题配置
- `syntaxes/stimage.tmLanguage.json` - 语法规则定义
- `package.json` - 扩展配置

## 开发者

**暮落夜月**

[![哔哩哔哩](https://img.shields.io/badge/Bilibili-暮落夜月-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/175546011)
[![Github](https://img.shields.io/badge/Github-SunsetNightMoon-181717?style=flat-square&logo=github)](https://github.com/SunsetNightMoon)

## 剧本开发者

**二次元绝缘体**

[![哔哩哔哩](https://img.shields.io/badge/Bilibili-二次元绝缘体-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/6009407)

## 免责声明

本扩展仅为特定STImage格式（`.stim`）文件提供语法高亮功能，不涉及《碧蓝档案》游戏本体或任何相关美术资源。

本扩展的开发与NEXON Games、MX studio、Yostar Pictures均无关联，未使用其任何美术资源。

《碧蓝档案》及其相关资源版权归NEXON Games、MX studio、Yostar Pictures所有。

## 开发说明

本项目在开发过程中使用了AI工具。

## 修改声明

根据 GPL v3 要求：
- 本项目为开源软件，可自由修改和分发
- 修改后的版本必须：
  1. 明确标注为修改版本
  2. 注明修改日期和内容
  3. 保留所有原始许可证声明
- 完整条款请参阅 [GPL v3 许可证](LICENSE)

## 许可证

[GPL v3](LICENSE)