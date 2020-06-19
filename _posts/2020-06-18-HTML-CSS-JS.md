---
title:  "HTML, CSS, JS 내용 정리"
excerpt: "html, css, js 공부 내용 정리 "

categories:
  - 내용정리
  - 공부
tags:
  - html
  - css
  - js
date : "2020-06-18 16:40"
---

![](/assets/images/html5.png)

### HTML(Hyper Text Markup Language)은 페이지에 제목, 문단, 표, 이미지, 동영상 등을 정의하고 그 구조와 의미를 부여하는 **정적 언어** 웹의 구조를 담당한다.
### 온전히 튼튼한 구조(semantic)를 만드는 것에 집중해야하는 언어이다.
---
![](/assets/images/css3.png)

### CSS(Cascading Style Sheets)는 마크업 언어(HTML, XML 등)가 실제 표시되는 방법(색상, 크기, 폰트, 레이아웃 등)을 지정하여 콘텐츠 구조를 꾸며주는 **정적 언어**로 웹의 시각적인 표현을 담당한다.
### 예쁘게 만드는 디자인에 집중할 수 있다.
### 적당한 크기와 아름다운 색상, 원하는 위치를 지정하는데 집중할 수 있습니다.
---
![](/assets/images/javascript.png)

### JS(JavaScript)는 콘텐츠를 바꾸고 움직이는 등 페이지를 **동적**으로 꾸며주는 역할을 하는 프로그래밍 언어로 웹의 **동적 처리**를 담당한다.
### JS는 HTML과 CSS를 동원해서 HTML, CSS의 역할도 수행할 수 있지만, 실제 HTML, CSS만큼 잘하진 못하기 때문에(성능적으로) 되도록 동적 처리에만 집중해야 한다.

---

웹 페이지를 제작할 때 각 언어의 역할을 다른 언어가 완벽하게 대체하기 어렵기 때문에 다른 언어가 대체하지 않도록 주의 하며, 각 역할이 제대로 수행되도록 구조적, 기술적으로 코드를 최적화시킬 필요가 있다.

---

## 내가 사용하는 웹 개발 에디터
![](/assets/images/logo_vs_code.jpg)

[VSCODE주소](https://code.visualstudio.com/)

### VS Code(VisualStudio Code)는 마이크로소프트(MS)에서 만든 텍스트 에디터이다.
### 사용법이나 단축키 정보가 많아 가볍게 시작할 수 있고 확장 기능이 상당히 많아서 꾸준히 사용하는 에디터이다.

### 설치
---
자신의 운영체제(Windows, macOS, Linux)에 맞는 Stable 버전을 설치하세요.
별도 설정값을 무시하고 다음/다음을 눌러 진행하세요.

### 확장(Extensions)
---
![](/assets/images/vs_code_extensions_icon.jpg)

VS Code는 다양한 확장 기능을 제공하며 외부에서 다운로드 받아 사용할 수 있다.

내가 사용하는 확장 기능
- **Korean Language Pack for Visual Studio Code**
    - vscode 메뉴가 한국어 변경

- **Beautify**
    - 코드 가독성을 위해 코드 작성 스타일을 수정합니다.

- **Live Server**
    - 하단 상태 바(Status bar)에서 Go Live 선택 또는,
    HTML 화면에서 우클릭 > Open with Live Server 선택

- **Auto Rename Tag**
    - 태그 이름을 수정할 때 열린 태그와 닫힌 태그가 쌍으로 수정됩니다.
    각각 수정해야 하는 번거로움을 줄일 수 있습니다.


## HTML 문서의 범위
---

**index.html** 같은 HTML 파일을 HTML 문서라고 할 수 있다.

``` html
<!DOCTYPE html>
<html>
  <head>
    문서에 대한 정보를 담는다.
  </head>
  <body>
    문서의 구조, 내용, contents를 담는다.
  </body>
</html>
````

``` html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="author" content="쫑마토">
    <meta name="description" content="나의 블로그">
    <title>토마토 농장</title>
    <link rel="stylesheet" href="./css/main.css">
    <script src="./js/main.js"></script>
</head>
<body>
    <section>
      <h1></h1>
      <div>
        <ul>
          <li></li>
          <li></li>
        </ul>
      </div>
    </section>
</body>
</html>
```
## HTML
---
`<html>`는(은) HTML 문서의 전체 범위를 지정한다.
웹 브라우저가 해석 할 html 문서가 어디에서 시작하며, 어디에서 끝나는지 알려주는 태그이다.

## HEAD
---
html 문서의 정보를 지정한다.
웹 페이지의 제목, 웹 페이지 인코딩 방식, 외부 파일 위치, 세팅 값 등
화면을 구성하는 기본 설정 

## BODY
---
사용자가 화면을 통해서 볼 수 있는 컨텐츠 형태, 레이아웃, 로고, 헤더, 푸터, 네비게이션, 메뉴, 버튼, 등 모든 구조에 해당

## DOCTYPE(DTD, 버전 지정)
---
DOCTYPE은 마크업 언어에서 문서 형식을 정의한다.
HTML은 1, 2, 3, 4, X-, 5 버전이 있다
표준 모드는 HTML5이다.