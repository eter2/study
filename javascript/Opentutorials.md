# JavaScript란? #
* 사용자와 상호 작용하는 웹페이지를 만들기 위한 기술.

# 수업의 목적 #
코드를 이해해봅시다.
```html
<input type="button" value="night" onclick="
document.querySelector('body').style.background.color='black';
document.querySelector('body').style.color='white';>">

<input type="button" value="day" onclick="
document.querySelector('body').style.background.color='white';
document.querySelector('body').style.color='black';>">
```
* `input`, `type=button`, `value="night"`는 html 문서에서 다뤘던 내용.
* `onclick`이라고 하는 속성의 값으로는 자바스크립트가 와야한다. `onclick` 속성이 위치하고 있는 버튼을 클릭했을 때 자바스크립트가 실행된다.
    * 버튼을 클릭했을 때 `body` 태그에 `style` 속성이 추가된다.

# HTML과 JavaScript의 만남1 (script태그) #
* 시작과 끝을 선언해주어야 하는 `<script>` 태그를 이용한다.

```html
<script>
    document.write(‘hello world’);
</script>

```
```html
<body>
    hello world
</body>
```

두 가지를 출력했을 때 같은 결과값이 나온다.

```html
<script>
    document.write(1+1);
</script>
```

```html
<body>
    1+1
</body>
```

자바스크립트는 결과값인 2가 출력되지만 html은 1+1이 그대로 출력된다.

# HTML과 JavaScript의 만남2 (이벤트) #
웹 브라우저 위에서 일어나는 일들을 이벤트라고 한다.

```html
<input type="button" value="hello" onclick="alert('hello')">
<input type="text" onchange="alert('changed')">
<input type="text" onkeydown="alert('key down')">
```

* 여러가지 사건들 중, 기념할만한 몇 가지 (onclick, onchange etc...) 를 정의해놓고 있다. 이를 이용해 사용자와 상호작용하는 웹페이지를 만들 수 있다.

# HTML과 JavaScript의 만남 3 (콘솔) #
파일을 만들지 않고 자바스크립트를 실행해야할 때, 개발자 도구의 `console`을 이용하자.
* 콘솔에서 실행하는 자바스크립트는 웹페이지에 삽입되어 있는 것처럼 동작한다. 즉, 현재 웹페이지를 대상으로 실행되는 것이다.

```js
alert('문자열' .length)
```
`문자열`의 문자 개수를 세어주는 코드이다.
