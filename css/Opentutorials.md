# CSS #
'**C**ascading **S**tyle **S**heets'의 약자. HTML 문서를 꾸밀 때 사용하는 언어.

# 사용법 #
* inline은 별도의 우선순위를 갖지만, internal과 external은 우선순위가 동등함.
1. `<style>`태그를 문서의 `<head>`안에 작성.
    ```html
    <head>
        <title> </title>
        <style>
         선택자 {
               속성: 속성값;
            }
      </style>
    </head>
    ```
1. 문자마다 스타일 속성을 사용.
    ```html
    <a href="http://www.github.com" style="color:red" target="_blank">GitHub</a>
    ```

1. 스타일 시트를 연결.
    ```html
    <head>
    <title> </title>
    <link rel="stylesheet" href="example.css">
    </head>
    ````

# 기본 형태 #
```css
선택자 {
    속성: 속성값;
}
```
* `{}`를 이용해 시작과 끝을 표시하고, 하나의 속성값이 끝났음을 `;(세미콜론)`을 이용해 표시해준다.
* `속성: 속성값;` 전체를 선언이라고 한다.
* 선택자 앞에 `#`(id), `.`(class), 아무것도 붙이지 않은 선택자 순으로 먼저 표현된다.
    * `#`는 `id`를 정의한다. `id`는 한 번만 지정해야 한다.
    * `.`는 `class`을 정의한다.
    * `class`와 `id`는 특정 요소들을 하나로 묶는데 이용한다.

# 구조 #

## 박스모델 ##
문서의 요소는 사각형 박스로 나타난다. 가장 바깥쪽부터 다음과 같은 네 가지 영억으로 구분된다.
* margin
* border
* padding
* content

**block level과 inline**
* block level element는 화면 전체를 사용한다.
* inline element는 자기 자신만을 둘러싼다.

## 그리드 ##
일정 수의 격자로 나누고 배치하는 방법.