# HTML

- HyperText Markup Language

# WEB

- 웹의 핵심적인 철학은 접근성(accessibility)
- 웹은 모든 운영체제에서 동작하고,
  웹페이지의 소스코드는 누구나 볼 수 있고,
  웹은 저작권이 없는 순수한 공공재입니다.

# HTML TAG

- 중첩해서 사용 가능

- <strong></strong> : 강조 표시(진하게)

- <u></u> : 밑줄 (underline)

- <br> : 줄바꿈

  - 쓰는 만큼 줄바꿈이 되기 때문에 원하는 간격을 줄 수 있음
  - 무엇인가를 설명하지 않는 태그들은 감싸야하는 컨텐츠가 없기 때문에 태그를 닫지 않는다는 규칙이 있음
  - ex. <br>, <meta>, <input> 등

- <p></p> : 단락 (paragraph) 그루핑

  - 단락 간격이 고정되어 시각적으로 자유도가 떨어짐
  - 하지만 CSS를 활용한다면 디자인을 자유롭게 변경 가능
    (단락의 경계를 분명이 하며 디자인을 변경할 수 있기 때문에 좋다.)

- <img>

  - '속성'(attribute) 필요
  - <img src="이미지의 주소"> _ src: source의 줄임말
    - src라는 속성을 통해 이미지를 불러옴

- <li></li> : 목차를 만들기 위한 테그 (list)

  - <li>태그는 항상 <ul> 태그를 필요로 함

- <ul></ul> : 목록을 다른 목록과 비교하기 위해 사용 (unordered list)

  - 순서 없는 리스트

- <ol></ol> : (ordered list)

  - 1, 2, 3 순서를 매겨줌

- <title></title> : 검색 엔진이 웹 페이지를 분석할 때 가장 중요하게 생각하는 태그

- <head></head> : 본문을 설명하는 정보

- <body></body> : 본문

- <html></html> : head와 body태그를 감싸는 하나의 태그

- <!doctype html> : 웹페이지가 HTML로 만들어졌다는 것을 표현하기 위해 사용

- <a href=""></a> : 링크 (a: anchor, href = HyperText Reference)

  - target="_blank": 링크 클릭 시 새 창에서 페이지가 열리게 하는 속성
  - title: 링크가 어떤 내용을 담고 있는지를 툴팁으로 보여주는 기능
