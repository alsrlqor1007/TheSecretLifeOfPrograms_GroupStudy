# HTML 문서

### HTML이란?
하이퍼 텍스트 마크업 언어(Hyper Text Markup Language)로 웹페이지 표시를 위해 개발된 마크업 언어  
꺽쇠 괄호(<,>)로 둘러싸인 태그로 되어있는 HTML 엘리먼트 형태로 작성  

### HTML의 구성요소
- **여는 태그**  
엘리먼트의 이름과 열고 닫는 꺽쇠 괄호로 구성  ex) `<p>`, `<title>`  
엘리먼트가 시작되는 부분부터 효과가 적용  
- **닫는 태그**  
엘리먼트의 이름 앞에 슬래시(/)가 포함 ex) `</p>`, `</title>`  
엘리먼트 효과가 종료  
- **내용**  
엘리먼트의 내용으로 단순 텍스트  
- **엘리먼트**  
여는 태그, 닫는 태그, 내용을 통틀어 요소(element)라고 한다.  

### 블록 레벨 요소 vs 인라인 요소
- **블록 레벨 요소**  
웹 상에 하나의 블록을 만드는 엘리먼트 ex)`<p>...</p>`  
앞 뒤 엘리먼트 사이의 새로운 줄을 만든다  
인라인 엘리먼트 내부에 만들 수 없지만 다른 블록 레벨 엘리먼트 내부에는 만들 수 있다  
- **인라인 요소**  
항상 블록 레벨 엘리먼트 내에 포함되어 있다  
단어같은 작은 부분에 대해서만 적용될 수 있다  
새로운 줄을 만들지 않는다  
ex) `<a>...</a>`,`<em>...</em>`,`<strong>...</strong>`


### 속성(attributes)
해당 엘리먼트에 실제로 표시되지는 않지만 추가적인 내용을 담고 싶을 때 사용  
속성 이름에 따라 미리 정의도니 동작이 있는 경우도 있다  
ex) `<a href='https://roadgram.net'>링크</a>`,`<input type='text'>text</input>`


### 참고자료
- [위키백과 - HTML](https://ko.wikipedia.org/wiki/HTML)
- [MDN - HTML 시작하기](https://developer.mozilla.org/ko/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
