---
layout: post
title:  "알고리즘 문제풀이 DAY1"
---

# 3번 문제
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






