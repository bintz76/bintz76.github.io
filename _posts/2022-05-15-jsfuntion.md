---
layout: single
title:  "함수"
categories: javascript
published: true
---

# 함수

특정작업을 반복하는 코드를 작성해야 한다면  
코드 자체를 '어딘가'에 만들어 놓고 사용할 수 있지 않을까?

에서나온 그 '어딘가' = 함수

함수는
> function 함수명 (매개변수들) {  
    이 함수에서 실행할 코드들  
return 반환값
}

의 형태로 이루어져 있다.

매개변수: 함수의 바디에서 사용할 수 있는 변수

```js
function calculateAvg(price1,price2){ //상품가격을 input으로 받아서 평균으로 내보내다(output). 이렇게 받은 매개변수는 함수 안에서 변수처럼 사용하면 된다.
    const sum = price1+price2 //b라는 변수는 가격1과 2를 더해서 할당해준다.
    console.log(`두 상품의 합은 ${sum}입니다. `)
    const avg = sum/2 //다시 평균을 구해주는 c를 할당
    return avg //할당된 데이터를 반환한다.
}
```

이 함수에서 매개변수는 **price1**과 **price2**

---
함수정의가 완료되고 선언할떄는
> const 변수명 = 선언한 함수명(매개변수들)

```js
const priceA = 50000
const priceB = 20000
const avg1 = calculateAvg(priceA,priceB)

console.log(`두 상품의 평균은 ${avg1}입니다.`)

const priceC = 2000
const priceD =3000
const avg2 =calculateAvg(priceC,priceD)

console.log(`두 상품의 평균은 ${avg2}입니다.`)
```

## 예시문제

> 세 개의 물건가격을 매개변수로 전달받아 평균값을 리턴하는 함수를 정의하고, 그 함수를 호출해서 평균값을 출력해보자.

```js
function calculateAvg(a,b,c){
    const avg = (a+b+c) /3
    return avg
}

const price1 = 60000
const price2 = 100000
const price3 = 80000
const avg4 = calculateAvg(price1,price2,price3)

console.log(`세 상품의 가격의 평균은 ${avg4}입니다.`)
```

