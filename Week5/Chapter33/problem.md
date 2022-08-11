# Chapter 33


<h5>1. 출력값을 예상 해보세요. </h5>

```js
const sym1 = Symbol.for('mySymbol');
const sym2 = Symbol.for('mySymbol');
const sym3 = Symbol('mySymbol');

console.log(Symbol.keyFor(sym1)); // 1.
console.log(Symbol.keyFor(sym2)); // 2.
console.log(Symbol.keyFor(sym3)); // 3.
console.log(sym1 === sym2); // 4.
console.log(sym2 === sym3); // 5.
```

<details>
  <summary>Solution</summary>
  <strong>1. mySymbol<br/>
  2. mySymbol<br/>
  3. undefined<br/>
  4. true<br/>
  5. false<br/></strong>
  <pre>
  Symbol.for 메소드
  > 검색에 성공하면 새로운 심벌 값을 생성하지 않고 검색된 심벌 값을 반환함.
  > 검색에 실패하면 인수로 전달된 키로 전역 심벌 레지스트리에 저장 후, 생성 된 심볼 값을 반환 
  Symbol.keyFor 메소드 
  > 전역 심볼 레지스트리에 저장된 심볼 값의 키를 추출
  </pre>
</ditails>

<br>