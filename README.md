# HTML

> HyperText Markup Language

- 웹 페이지를 만드는 마크업 언어
- 기본적으로 웹 페이지에서 다른 페이지로 이동할 수 있는 HyperLink를 지원하도록 설계 되었고 이 덕분에 페이지 안에서 클릭만으로 다른 페이지로의 이동이 가능



## HTML Basic Tag

> 특정 기능을 지원하는 태그 문법 (중첩해서 사용 가능)

1. `<html>` 

   - head와 body태그를 감싸는 하나의 태그

   - 웹 페이지의 시작과 끝

2. `<head>`

   - 웹 페이지의 정보, 문서에서 사용할 외부 파일들을 링크할 때 사용
   - 본문을 설명하는 정보

3. `<body>`

   - 브라우저에 실제 표시되는 내용 (본문)

4. `<title>`

   - 문서의 제목
   - 웹브라우저의 제목 표시줄에 표시

5. `<meta>`

   - 문자 인코딩 및 문서 키워드의 요약 정보

6. `<div>`

   - 컨텐츠들을 묶는 용도로 사용 (상자 같은 느낌)
   - block Type
     - div를 붙이면 줄바꿈

7. `<span>`

   - 컨텐츠들을 묶는 용도로 사용
   - inline Type
     - span을 여러개 붙여도 줄바꿈이 되지 않는다. 

8. `<a>`

   - a: anchor - 웹 페이지나 외부 사이트로 연결
   - `<a href="연결할 경로">이름</a>`
     - href: HyperText Reference
   - 하이퍼링크를 통해 페이지 간 이동이 가능

9. `<script>`

   - 코드 삽입
   - 보통 자바스크립트 코드를 넣을 때 사용
     - `<script type="text/JavaScript">document.write("자바스크립트 코드 추가");</script>`

10. `<link>`

    - 외부 파일을 연결할 때 사용 (CSS, JS 등)
    - `<link rel="stylesheet" type="text/css" href="index.css"/>`

11. `<img>`

    - 속성(attribute) 필요
    - `<img src="이미지 주소">`
      - src: source - src라는 속성을 통해 이미지를 불러옴

12. `<p>`

    - p: paragraph - 단락, 앞뒤로 빈 줄이 생기며 단락이 생김

13. `<li>`

    - list - 목차를 만들기 위한 태그
    - `<ul>` 태그를 필요로 함

14. `<ul>`

    - 순서가 없는 리스트 항목 묶음
    - 목록을 다른 목록과 비교하기 위해 사용

15. `<ol>`

    - 순서가 있는 리스트 항목 묶음

16. `<style>`

    - head 안에서 스타일 정보 정의

17. `<br>`

    - 줄바꿈 - 쓰는 만큼 줄바꿈이 되기 때문에 원하는 간격 설정 가능
    - 닫는 태그가 없음

18. `<h>`

    - h1~h6
    - 제목 태그

19. `<input>`

    - form의 요소 중 하나로, 사용자가 정보를 입력할 때 사용
    - `<input type="유형" 속성="속성값">`

20. `<form>`

    - GET, POST 방식으로 내용 전송 가능

21. `<button>`

    - form 요소 중 하나로 페이지에 버튼을 넣고 form을 전송하거나 reset할 때 사용



## HTML Sementic Tag

> 사용자가 이해하기 쉽도록 태그 이름만 보고도 역할이나 위치를 알 수 있도록 만든 태그

1. `<header>`
   - 제목 - 사이트의 제목, 로고 등이 위치
2. `<nav>`
   - 목차 - 다른 페이지로 갈 수 있는 링크들이 위치
3. `<section>`
   - 보여주고자 하는 주요 내용이 위치
4. `<aside>`
   - 본문 외의 내용이 위치
5. `<footer>`
   - 저작권 / 제작자 정보가 위치


---

# CSS

> Cascading Style Sheets

- 웹 페이지를 표현하기 위한 스타일 규칙을 모아 놓은 문서
- HTML 문서를 시각적으로 꾸미는 용도로 사용

- ('선택자(selector)' + '선언(declaration)' + '속성(property)') 으로 구성

- css 파일을 만든 후 html파일의 `<head>`  부분에 파일 경로를 추가해 사용한다.
  - `<link rel="stylesheet" type="text/css" href="css/index.css" >`



## Selector

> 특정 요소를 선택하여 스타일링 하기 위해 필요



### 기본 선택자

1. 클래스(class) 선택자
   - 마침표(.) 문자로 시작, 해당 클래스가 적용된 모든 항목 선택
2. 아이디(id) 선택자
   - 우물정(#) 문자로 시작, 해당 아이디가 적용된 모든 항목 선택
   - 일반적으로 하나의 아이디는 하나의 문서에서 1번만 사용(Unique)



### 적용 우선순위(Cascading Order)

1. 중요도
   - !important
2. 우선순위
   - 인라인 > id 선택자 > class. tjsxorwk > 요소 선택자
3. 소스 순서



### 결합자 (Combinators)

1. 자손 결합자

   - `div span{}`

   - selector A 하위 모든 selector B 요소

2. 자식 결합자

   - `div > span{}`

   - selector A 바로 아래의 selector B 요소

3. 일반 형제 결합자

   - `p ~ span{}`

   - selector A의 형제 요소 중 뒤에 위치하는 selector B 요소를 모두 선택

4. 인접 형제 결합자

   - `p + span{}`

   - selector A의 형제 요소 중 바로 뒤에 위치하는 selector B 요소 선택



## CSS 속성

### font

> 페이지에서 사용할 폰트의 종류를 외부에서 받아올 수 있다.

- `<font-size>` : 글자 크기
- `<font-weight>` : 글자 두께

- `<font-style>` : 글꼴의 스타일
- `<font-family>` : 글꼴



### box model

> 태그를 통해 요소를 만들 때마다 새로운 box가 생기고 그 박스에 style을 주어서 문서를 꾸밀 수 있다.

- width
  - 내용을 표시하는 영역에서 가로 길이

- height
  - 내용을 표시하는 영역에서 세로 길이
- box-sizing
  - 기본적으로 모든 요소의 box-sizing은 content-box 기준 (padding 제외, 순수 contents영역만을 box로 지정)
  -  `box-sizing` 속성을 통해서 `border-box`를 지정하면 테두리를 width와 height를 계산하는 기준으로 변경할 수 있다.

- padding
  - 내용과 border 사이의 영역을 나타내고 안쪽 여백 역할을 담당

- border
  - 내용에 패딩을 더한 영역의 경계를 나타내며 margin과 padding의 경계가 되기도 한다. (테두리 역할)

- margin
  - border 부터 box model의 maximum 범위 까지를 나타내는 영역 (바깥 여백 영역 역할)
  - 외부 요소와의 거리를 조절하는 용도로 사용



### display

> 요소를 어떻게 보여줄지를 결정

1. `none`

   - 요소를 아예 보여주지 않고 지워버린다.

2. `block`

   - 줄바꿈이 일어나는 요소

   - 화면 크기 전체의 가로영역을 전부다 차지
   - width, height을 지정할 수 있지만 여전히 다음 요소는 개행되어 나타난다.
   - 대표적으로 `div`, `p`, `h`, `li` 태그

3. `inline` 

   - block 과 달리 줄 바꿈이 되지 않고, width와 height를 지정할 수 없다
   - content 너비만큼 가로 폭을 차지
   - block 요소 안에 들어갈 수 있다.
   - 대표적으로 `span` `a` `strong` `i` 태그

4. `inline-block`

   - block과 inline의 중간 단계
   -  width와 height는 지정할 수 있지만 개행은 되지 않는다.





### position

> 문서 상에서 요소를 배치하는 방법을 지정

- static
  - 모든 태그의 기본 값(기준 위치)
- relative
  - 상대 위치
  - 자기 자신의 static 위치를 기준으로 이동
- absolute
  - 절대 위치
  - 요소를 일반적인 문서 흐름에서 제거 후 레이아웃에 공간을 차지하지 않음
  - static이 아닌 가장 가까이 있는 부모/조상 요소를 기준으로 이동 (없는 경우 body에 붙음)
- fixed
  - 고정 위치
  - 요소를 일반적인 문서 흐름에서제거 후 레이아웃에 공간을 차지하지 않음
  - 부모 요소와 관게 없이 viewport를 기준으로 이동
  - 스크롤 시에도 항상 같은 곳에 위치





### flex

> flexible-box를 사용할 수 있는 display 속성
>
> 각각의 요소들을 item으로 보고 item들을 효과적을 정렬하고 배치할 수 있도록 도와준다.

#### container

1. flex-direction
   - 안에 있는 Item들을 정렬할 때 어떤 순서로 정렬할 지, 가로로 정렬할지 세로로 정렬할지를 선택
   - 정방향 가로정렬이 기본값
2. felx-wrap
   - flex는 기본적으로 item을 한줄에 정렬(기본값 = no-wrap)
     - 중간에 끊고 줄바꿈을 하고 싶다면 flex-wrap을 사용
3. justify-content
   - 메인 축을 중심으로 아이템들을 여백과 함께 정렬하는 방식을 지정
   - flex-start가 기본 값
   - 중앙 정렬을 원할 경우 `center`나 `space-around`등을 사용
4. align-content
   - flex-wrap 을 사용해서 item이 여러 줄로 존재하고 있을 때, 여백과 함께 정렬하는 방식을 지정할 수 있다. 
   - 기본값은 flex-start
   - 한 줄 밖에 없을 때는 justify-content와 똑같다.
5. align-items
   - container 안에서 items들의 세로정렬하는데 사용



---

# WEB

- 웹의 핵심적인 철학은 접근성(accessibility)
- 웹은 모든 운영체제에서 동작하고, 웹페이지의 소스코드는 누구나 볼 수 있고, 웹은 저작권이 없는 순수한 공공재입니다.




# 세계 최초의 웹사이트

http://info.cern.ch/



# 클라이언트와 서버

- 고객을 영어로는 클라이언트(client)라고 합니다.
  - 요청하는 컴퓨터 = 클라이언트 컴퓨터
  - 웹 브라우저 (웹 클라이언트)
- 사업자를 영어로는 서버(server)라고 합니다.
  - 응답하는 컴퓨터 = 서버 컴퓨터
  - 웹 서버

- client는 server에 request를 보내고
- server은 client에게 그에 맞는 response를 보내준다.

웹 브라우저

- HTML 문서와 그림, 멀티미디어 파일등 월드 와이드 웹을 기반으로 한 인터넷의 컨텐츠를 검색 및 열람하기 위한 응용 프로그램의 총칭.

웹 서버

- 웹 호스팅 업체를 활용
- ex. github의 pages 기능
- https://opentutorials.org/course/3084/18891



