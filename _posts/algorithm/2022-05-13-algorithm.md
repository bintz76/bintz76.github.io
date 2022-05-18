---
layout: single
title:  "알고리즘 문제풀이 DAY1"
permalink: /category/알고리즘 문제/
categories: 알고리즘 문제

published: true
---

# 가운데 글자 가져오기 문제
단어 s의 가운데 글자를 반환하는 함수, solution을 만들어 보세요. 단어의 길이가 짝수라면 가운데 두글자를 반환하면 됩니다.

- 제한사항

s는 길이가 1 이상, 100이하인 스트링입니다.

---
# 풀이
s가 짝수 일때는 중간의 두글자, 홀 수 일때는 중간의 한글자가 반환되어야 한다.

```js
function solution(s) {
    var answer = '';
    
    if (s.length % 2 == 0){
        answer = s.substr(s.length/2-1,2);
    }else{
        answer =s.substr((s.length+1)/2-1,1);
    }
    return answer;

```
---
# 하나씩 뜯어보기
```js
 if (s.length % 2 == 0)
 ```
 짝수 값을 도출
 
 S의 길이만큼 2로나눈 나머지 = 짝수

 ```JS
  answer = s.substr(s.length/2-1,2);
  ```

 > substr ( start , length )

 > **문자열을 뽑아내는 함수**
 
 >  start로 시작위치를 정하고 length로 잘라낼 문자열의 길이를 정한다. 

컴퓨터는 0부터 숫자를 세기때문에 1의 값을 빼주고, 짝수기 때문에 2개의 글자를 반환해준다.!

```js
  }else{
        answer =s.substr((s.length+1)/2-1,1);
    }
    return answer;
```
아니면( 홀수이면)

마찬가지로 substr()함수를 쓰지만 홀수이기 때문에 lenth에 1을 더해준다.

---
# 없는 숫자 더하기 문제

0부터 9까지의 숫자 중 일부가 들어있는 정수 배열 numbers가 매개변수로 주어집니다. numbers에서 찾을 수 없는 0부터 9까지의 숫자를 모두 찾아 더한 수를 return 하도록 solution 함수를 완성해주세요.

- 제한사항

1 ≤ numbers의 길이 ≤ 9

0 ≤ numbers의 모든 원소 ≤ 9

numbers의 모든 원소는 서로 다릅니다.

---

# 풀이

i의 범위를 지정한 후 포함되지 않은 숫자를 더한다.

```js
function solution(numbers) {
    var answer = 0;
    for(i=1; i<10; i++){
        if(!numbers.includes(i))answer+=i;
    }
    return answer;
}
```

> includes(i) 함수 

>includes(i)는 배열에 i의 값을 포함하고 있는지의 여부를 반환한다.

포함되지 않은 숫자를 더하는 것이 목적이므로 
앞에 !를 붙여줬다.

! (not) 는 true를 false로, flase를  true로 바꿔서 리턴해준다. 
