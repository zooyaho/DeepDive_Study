# Chapter 48

<pre>1. 모듈은 공개가 필요한 자산에 한정하여 명시적으로 선택적 공개가 가능한데, 이를 [   1   ]라고 하고
모듈 사용자는 모듈이 공개한 자산 중 일부 또는 전체를 선택해 자신의 스코프 내로 불러들여 재사용할 수 있는데 이를 [   2   ]라한다.</pre>

<details>
  <summary>Solution</summary>
<strong>1. export<br>
2. import</strong>
</details>

<br>

<pre>2. 다음 코드를 보고 출력값을 예상하세요.</pre>

```html
<script type="module" src="foo.mjs"></script>
```

```js
// foo.mjs
var x = "foo";
console.log(x); // 1. ?
console.log(window.x); // 2. ?
```

<details>
  <summary>Solution</summary>
<strong>1. foo<br>
2. undefined</strong>
<pre>x 변수는 전역 변수가 아니며 window 객체의 프로퍼티도 아니다.</pre>
</details>

<br>
