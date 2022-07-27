## JSON

`JavaScript Object Notation`의 축약어로 데이터를 저장하거나 전송할 때 많이 사용되는 경량의 데이터 교환 형식이다.

Javascript에서 객체를 만들 때 사용하는 표현식을 의미한다. 
JSON 표현식은 사람과 기계 모두 이해하기 쉬우며 용량이 작아서, 최근에는 JSON이 XML을 대체해서 데이터 전송 등에 많이 사용한다.
JSON은 데이터 포맷일 뿐이며 어떠한 통신 방법도, 프로그래밍 문법도 아닌 단순히 데이터를 표시하는 표현 방법일 뿐이다.

<br/>

<div align="center">

![](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FB1wJV%2FbtqSTImOlsB%2FzpskLu4DwKd8uqa7bgzw0k%2Fimg.png)

</div>

<br/>

JSON 형식은 자바스크립트 객체와 마찬가지로 `key/value`가 존재할 수 있으며 key 값이나 문자열은 항상 쌍따옴표를 이용하여 표기한다.
객체, 배열 등의 표기를 사용할 수 있으며, 일반 JS 객체처럼 원하는 만큼 중첩시켜 사용할 수 있다. JSON 형식으로는 null, number, string, array, object, boolean을 사용할 수 있다.

<br/>

AJAX는 단순히 데이터만이 아니라 JS 그 자체도 전달할 수 있다. JSON 데이터를 받았는데 단순 데이터가 아니라 JS를 받아 그게 실행 될 수 있다.
이러한 이유로 순수하게 데이터만 추출하기 위한 JSON 관련 라이브러리를 따로 사용하기도 한다.

<br/>

- `JSON.parse(JSON 형식의 텍스트)` JSON 형식의 텍스트를 자바스크립트 객체로 변환
- `JSON.stringify(JSON 형식(문자열)으로 변환할 값)` 자바스크립트 객체를 JSON 텍스트롤 변환

<br></br>

### XML과 JSON의 차이점

둘 다 데이터를 저장하고 전달하기 위해 고안되었다. 기계 뿐만 아니라 사람도 쉽게 읽을 수 있으며, 계층적인 데이터 구조를 가진다.

XML은 데이터 저장, 전달시 사용되는 마크업 언어이다. ML DOM(Document Object Model)을 이용하여 해당 문서에 접근후 XML 파서를 통해 파싱된다.
JSON은 데이터를 저장하고 전달하는 메타언어이다. 자바스크립트의 표준 함수인 eval()함수로 파싱된다.

XML은 스키마를 사용하여 데이터의 무결성을 검증할 수 있지만, 배열을 사용할 수 없고 데이터를 읽고 쓰는 것이 JSON에 비해 느리다.
JSON은 문자열을 전송받은 후에 해당 문자열을 바로 파싱하므로, XML보다 빠른 속도를 가지고 있다. 하지만 개발자가 문자열 데이터의 무결성을 검증해야 한다.


JSON은 HTML과 JavaScript가 연동된 빠른 응답이 필요한 웹 환경에서 많이 사용되고, XML은 스키마를 사용하여 데이터의 무결성을 검증할 필요가 있을 때 많이 사용된다.

<br></br>

### 참고

- [JSON이란 무엇일까?](https://usefultoknow.tistory.com/entry/JSON%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)