## extend(), 객체 합치기
---

제이쿼리의 extend()는 다수의 객체를 하나의 객체로 합치는 merge 기능을 수행한다. <br>
**두 개 이상의 객체를 하나로 합치려는 경우 extend()를 사용** 하여 새로운 객체로 만들 수 있다. <br>

``` javaScript
$.extend(대상, 객체1, 객체2, 객체3, ..., 객체n)
```

<br>

---

### extend() 객체 예제
``` javaScript
var objA = { a: 1, b: 2 }
var objB = { c: 3, d: 4 }

var objC = new Object;
objC = $.extend({}, objA, objB);

console.log(objC);
```
위 객체 objC의 출력 결과는 아래와 같다.
```
a: 1
b: 2
c: 3
d: 4
```
