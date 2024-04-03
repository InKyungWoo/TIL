- 집에 가는 길

```jsx
/*
 *  solution 함수 안에 코드를 작성해주세요.
 *  money에 입력된 금액에 따라 결과를 출력합니다.
 *  조건문을 이용해 문제를 해결할 수 있습니다.
 */
function solution(money) {
  var answer;

  if (money >= 1000) {
      answer = "택시";
  } else if (money >= 500) {
      answer = "버스";
  } else if (money >= 300) {
      answer = "지하철";
  } else {
      answer = "도보";
  }
 
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 조건에 맞는 암호

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  // 숫자 입력받기
  var num = input.split(" ");  
  var a = num[0]; var b = num[1]; var c = num[2]; var d = num[3];
  
  var answer;
  //조건에 따라 answer값 return
  if (a <= b && a <= d && b >= c && c < 6) {
      answer = true;
  } else if (a == b && a == c && a == d) {
      answer = true;
  } else {
      answer = false;
  }

  // 다른 방법
  // answer = (a <= b && a <= d && b >= c && c < 6) || (a == b && a == c && a == d);

  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 약수 찾기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  var answer = [];

  for (var i = 1; i <= input; i ++) {
      if (input % i == 0) {
          answer.push(i);
      }
  }

  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;

```

<aside>
💡 let 함수

---

```jsx
for (let i = 1; i <= input; i++)
```

for문에서 let을 사용하지 않으면 변수 i가 전역 변수로 선언되어 현재 스코프 밖에서도 접근할 수 있게 됩니다. 이는 변수 충돌이 발생할 수 있고 의도하지 않은 변수 값 변경 등의 문제가 발생할 수 있습니다.

따라서 let을 사용하여 변수 i를 블록 범위로 제한하는 것이 좋습니다. 이렇게 하면 for문 내에서만 변수 i에 접근할 수 있고, for문이 끝나면 변수 i는 사라지게 됩니다. 이는 코드의 가독성을 높이고 변수 관리를 효율적으로 할 수 있게 도와줍니다

</aside>

- 3, 6, 9 게임  🌟

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  var answer = [];
  
  for (var i = 1; i <= 30; i++) {
      var one_digit = (i % 10);
      var ten_digit = Math.floor(i/10);  
      
      // 일의 자리가 3, 6, 9 일때
      if (one_digit == 3 || one_digit == 6 || one_digit == 9) {
          answer.push("짝!");
      // 십의 자리가 3, 6, 9 일 때
      } else if (ten_digit == 3 || ten_digit == 6 || ten_digit == 9) {
          answer.push("짝!");
      } else {
          answer.push(i);
      }
  }
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 해설코드 💡

```jsx
function solution() {
  var answer = [];

  for (var i = 1; i <= 30; i++) {
      if ((i % 10) % 3 == 0 && i % 10 != 0) {
        answer.push("짝!");
      } else if (Math.floor((i / 10) % 3) == 0 && Math.floor(i / 10) != 0) {
        answer.push("짝!");
      } else {
        answer.push(i);
      }
  }

  return answer;
}
```

- 숫자 출력

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num) {
  var answer = [];
  //console.log(num);
  
  for (var i =1; i <= num; i++) {
      answer.push(i);
  }
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 노동요

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(s) {
  var answer = "";
  
  for (let i=0; i <= s.length-1; i++) {
      //console.log(s[i]);
      if (s[i] == " ") {
          answer += "링디기디기\n";
      } else if (s[i] == ".") {
          answer += "딩딩딩\n";
      } else {
          answer += "링딩동 ";
      }
  }
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 음식 가격 계산하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution() {
  var korean = 7000;
  var chinese = 6000;
  var western = 8500;
  var discount_korean = 7000 * 0.9;
  var total_price = discount_korean * 55 + chinese * 43 + western * 52;

  return { korean, chinese, western, discount_korean, total_price };
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 변수 비교하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution() {
  var a = 10; var b = 10;
  var case1 = (a == b);
  var case2 = (a === b);

  var b = "10";
  var case3 = (a == b);
  var case4 = (a === b);

  return {case1, case2, case3, case4}; 
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 변수 다루기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num, string) {
  num += 204;
  string += 'elice!';

  return {num, string}; 
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 소수의 합 구하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution() {
  //var answer = [];
  var sum = 0;
  
  for (var num = 1; num <= 200; num++) {
      // 1은 제외
      for (var i = 2; i <= num; i++) {
          if (num % i === 0) {
              break;
          }
      }
      // 나누어 떨어졌을 때 '나누는 수 === 자기 자신' -> 소수
      if (num === i) {
          //answer.push(num);
          sum += num;
      }
  }
  return sum; 
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```