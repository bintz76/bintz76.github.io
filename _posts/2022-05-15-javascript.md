---
layout: single
title:  "자바스크립트 변수, 데이터 타입"
categories: javascript
---

# 변수 (Variable)

자바스크립트에서 변수를 선언할 때의 키워드는 let, const, var가 있다.

---

## let

```js
let name = 'lia'
console.log(name)

name = 'sunja kim'
console.log(name)
```

---

## const

```js
const name = 'lia'
console.log(name)
```
~~name = 'lia'~~

const는 let과 달리 한번 값을 할당하고 나면 재할당이 불가하다.

---

## var

var라는 키워드로도 변수 선언이 가능하지만 요즘엔 안쓴다고 한다.
~~(프로그래머스에는 쓰더라)~~

---

# 데이터 타입(Datatype)

## 숫자데이터

```js
console.log(10)

let age = 37
console.log(age)
```

숫자데이터는 따옴표나 큰따옴표로 묶어줄 필요가 **없다!!**

---

## 문자열 데이터

```js
let name = 'lia'
console.log(name)
```

이름이나 알파벳 같은 문자열 데이터. 작은따옴표('')나 큰따옴표("")로 묶어서 표현해야한다.

---
## Boolean 

참과 거짓을 나타내는 별도의 데이터 타입.

```js
let isman = true //'참'을 의미하는 Boolean데이터
let iswoman =false //'거짓'을 의미하는 Boolean데이터
```

---

## Null 과 Undefined

null은 텅텅비어 있는 값, undefined는 선언만 하고 출력되지 않은 값

```js
let name1 =null
console.log(name1) //null

let name2   //undefined
```

---
