# jQuery

자바스크립트로 DOM을 조작할 수는 있지만, 문제가 있다.

1. DOM 함수 동작이 브라우저마다 다를 수 있다.
2. DOM 함수를 사용하기 불편하다. (사용친화적인 인터페이스를 제공하지 않는다. )
   <br />

jQuery는 2006년에 나온 라이브러리로 브라우저 사이의 불일치를 부드럽게 메꿔준다.
따라서 프로그래머가 브라우저 간의 차이를 다룰 필요가 없다. 그리고 더 쉬운 DOM 조작 인터페이스를 제공한다.
<br />

```html
<!-- 1. jQuery 라이브러리 import -->
<script
  type="text/javascript"
  ,
  src="https://code.jquery.com/jquery-3.2.1.min.js"
></script>

<!-- 2. 실제 코드  -->
<script>
  $(function () {
    $('big').css('background', 'green');
  });
</script>
```

<br />

1. 첫 번째 `<script>` 엘리먼트는 jQuery 라이브러리를 임포트한다.
2. 두 번째 `<script>` 엘리먼트에는 실제 코드가 담겨있다.
   - `$('big')`는 실렉터.
   - `.css('background', 'green')`는 실렉터로 선택한 원소에 대해 수행할 액션
     <br />

이렇게 jQuery를 사용하면 자바스크립트로 더 쉽게 DOM을 변경할 수 있다. 현재는 jQuery 외에도 상이한 자바스크립트 라이브러리가 많다.
