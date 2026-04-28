---
title: STImage Edit Support - 한국어
language: Korean
---

# STImage Edit Support

SillyTavern 시나리오 《블루 아카이브: 새로운 새벽》에서 사용되는 STImage 형식 파일에 대한 구문 강조 표시를 제공하는 VSCode 확장 프로그램입니다.
《블루 아카이브: 새로운 새벽》1.2버전의 새로운 텍스트 형식과 호환되어 편집을 용이하게 합니다.
Visual Studio Code, Trae CN 등 vsix 설치를 지원하는 에디터와 호환됩니다.

## 언어 전환 🌐
| 언어 | 파일 |
|------|------|
| 中文 | [README.md](../README.md) |
| English | [README-en.md](README-en.md) |
| 日本語 | [README-ja.md](README-ja.md) |
| 한국어 | [README-ko.md](README-ko.md) |

## 기능

- STImage 형식의 `.stim` 파일에 대한 구문 강조 표시
- 다양한 파일 형식 지원:
  - 따옴표와 번호가 있는 캐릭터 표정 형식(1.2버전)
  - 따옴표와 번호가 없는 배경 이미지 형식
- 요소를 명확하게 구분하는 맞춤 색상 테마
- 《블루 아카이브: 새로운 새벽》시나리오 리소스 편집에 최적화

## 설치 방법

### 방법1: 로컬 파일에서 설치

1. VSCode/Trae CN을 엽니다
2. `Ctrl+Shift+P`를 눌러 명령 팔레트를 엽니다
3. "Extensions: Install from VSIX..."를 입력합니다
4. `STImage-Edit-1.4.1.vsix` 파일을 선택합니다

### 방법2: 개발 모드로 설치

1. 에디터에서 `ba-stimage-editingsupport` 폴더를 엽니다
2. `F5`를 눌러 확장 프로그램 개발 호스트를 시작합니다
3. 새 창에서 확장 프로그램이 자동으로 로드됩니다

### 방법3: VSCode Trae CN 특유의 간단한 그래픽 설치 방법

1. VSCode/Trae CN을 엽니다
2. 확장 프로그램 아이콘을 클릭합니다
3. 확장 프로그램 인터페이스의 오른쪽 상단 ⋯(더 보기) → VSIX에서 설치...
4. `STImage-Edit-1.4.1.vsix` 파일을 선택합니다


## 사용 방법

1. 확장 프로그램을 설치한 후,任意の `.stim` 파일을 엽니다
2. 오른쪽 하단의 언어 모드 선택기를 클릭합니다
3. **"STImage"** 언어 모드를 선택합니다
4. 파일에 자동으로 구문 강조 표시가 적용됩니다
5. 정상적으로 표시하려면 내장된 **"STImage Theme"**를 사용해야 합니다

## 파일 형식 지원

확장 프로그램은 다음 형식의 구문 강조 표시를 지원합니다:

### 형식1(따옴표와 번호 포함) - 1.2버전 새 형식

```
<"星野_正常":"01"|https://xxxx.xxxxxx.xxx/xxxxx.png>
<"夢先輩_笑A":"00"|https://xxxx.xxxxxx.xxx/xxxxx.png>
```

### 형식2(따옴표와 번호 없음) - 배경 이미지 형식

```
<基沃托斯城市_正常|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
<阿拜多斯会议室_夜晚|https://xxxx.xxxxxx.xxx/xxxxx.jpg>
```

### 구분선

```
———————————————————————————————————————
```

## 색상 설명

| 요소 | 색상 | 설명 |
|------|------|------|
| 캐릭터 이름(따옴표 포함) | 수색 | 예:星野_正常 |
| 배경 이름(따옴표 없음) | 보라색 | 예:基沃托斯城市_正常 |
| 표정 번호 | 분홍색 | 예:01 |
| URL 링크 | 에디터 기본값 | 밑줄이 있는 링크 스타일 |
| 구분 기호 | 회색 | `< > : \|` |
| 구분선 | 녹색 | —————— |

## 개발

색상 또는 구문 규칙을 수정하려면 다음 파일을 편집합니다:

- `themes/stimage-theme.json` - 색상 테마 구성
- `syntaxes/stimage.tmLanguage.json` - 구문 규칙 정의
- `package.json` - 확장 프로그램 구성

## 개발자

**暮落夜月**

[![Bilibili](https://img.shields.io/badge/Bilibili-暮落夜月-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/175546011)
[![Github](https://img.shields.io/badge/Github-SunsetNightMoon-181717?style=flat-square&logo=github)](https://github.com/SunsetNightMoon)

## 시나리오 개발자

**二次元绝缘体**

[![Bilibili](https://img.shields.io/badge/Bilibili-二次元绝缘体-00A1D6?style=flat-square&logo=bilibili)](https://space.bilibili.com/6009407)

## 면책 조항

이 확장 프로그램은 특정 STImage 형식(`.stim`) 파일에 대한 구문 강조 표시 기능만 제공하며, 《블루 아카이브》게임 자체 또는 관련 예술 자원과는 무관합니다.

이 확장 프로그램의 개발은 NEXON Games, MX studio, Yostar Pictures와 관련이 없으며, 이들의 예술 자원을 사용하지 않았습니다.

《블루 아카이브》및 관련 자원의 저작권은 NEXON Games, MX studio, Yostar Pictures에 있습니다.

## 개발 설명

이 프로젝트는 개발 과정에서 AI 도구를 사용했습니다.

## 수정 선언

GPL v3 요구 사항에 따라:
- 이 프로젝트는 오픈 소스 소프트웨어로, 자유롭게 수정 및 배포할 수 있습니다
- 수정된 버전은 다음을 충족해야 합니다:
  1. 수정 버전임을 명확하게 표시
  2. 수정 날짜 및 내용 명시
  3. 모든 원래 라이선스 선언 유지
- 전체 조항은 [GPL v3 라이선스](../LICENSE)를 참조하십시오

## 라이선스

[GPL v3](../LICENSE)
