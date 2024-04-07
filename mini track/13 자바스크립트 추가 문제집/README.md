### 1. 샌드위치 만들기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
	// input = 햄과치즈
  let sandwich = "빵 " + input + " 빵";
  return sandwich;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 2. 두 수의 곱 구하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(a, b) {
  var a; var b;
  return a * b;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 3. 홀수, 짝수 판단하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num) {
  //console.log(num);
  if (num % 2 == 0) {
      return num + ':"짝수"';
  } else {
      return num + ':"홀수"';
  }
  return;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 4. 삼각형의 각도 구하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(angle) {

  //angle 변수에 어떤 값이 들어오는지 확인해보세요!
  console.log(angle);
  let angle1 = parseInt(angle.split(" ")[0]);
  let angle2 = parseInt(angle.split(" ")[1]);
  let answer;

  if (angle1 + angle2 >= 180) {
      answer = 0;
  } else {
      answer = 180 - angle1 - angle2;
  }
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

### 5. 가장 큰 자릿수 숫자 구하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(number) {
  console.log(number);
  let digit = parseInt(String(number).charAt(0));
  
  return digit;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 6. 배수 판별기 

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num) {
  var answer = [];
  
  if (num % 2 == 0) { answer.push(2 + "의 배수입니다."); }
  if (num % 3 == 0) { answer.push(3 + "의 배수입니다."); }
  if (num % 5 == 0) { answer.push(5 + "의 배수입니다."); }
  if (num % 7 == 0) { answer.push(7 + "의 배수입니다."); }

  answer = answer.join("\n");
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 7. In the Middle

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  //console.log(input.split(" "));
  let answer = parseInt(input.split(" ")[1]);
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 8. 3,6,9!

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  //console.log(input);
  if ((input+1) % 3 == 0) {
      return "짝!";
  } else {
      return input + 1
  }
  return;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 9. 말썽쟁이 도도새

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  const index = input.indexOf("웩");
  //console.log(index);
  return index;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 10. 주문내용 계산하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution() {

  var americano = 3500;
  var cafe_latte = 3800;
  var milk_tea = 4200;

  var price1 = americano * 2 + milk_tea;
  var price2 = (cafe_latte * 2 + milk_tea * 2) * 0.9;

  return price1 + price2; 
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 11. 엘리스 토끼의 수학 숙제


> 💡 1부터 매개변수 **`num`** 까지의 합의 제곱과 제곱의 합의 차이를 출력하세요.
> - 합의 제곱 수식<br>
>  (1 + 2 + 3 + ・・・ 8 + 9 + N)^2 <br>
> - 제곱의 합 수식 <br>
>    1^2 + 2^2 + 3^2 + ・・・ 8^2 + 9^2 + N^2
    

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num) {
  //console.log(num);
  var sum1 = 0; var squreSum = 0;

  // 합의  제곱 구하기
  for (i=1; i<=num; i++) {
      sum1 += i;
  }
  var sumSqure = sum1 * sum1;

  // 제곱의 합 구하기
  for (i=1; i<=num; i++) {
      squreSum += i * i;
  }
  
  var answer = sumSqure - squreSum;
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 12. 구슬 꾸러미


> 💡 `input`  매개변수로부터 구슬 꾸러미의 무게를 입력받고 꾸러미를 만드는 데 사용되는 최소 구슬의 수를 출력하세요.
- (1 ≤ *input* ≤ 10,000)
- 만약 무게에 맞추어 꾸러미를 만들 수 없는 경우에는 **`1`**을 출력하세요.

```jsx

```
<br>

### 13. 렌터카

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(hour, price, defaultPrice, defaultHour, defaultCost) {
  var H = hour; //엘리스 토끼가 이용할 시간
  var A = price; //모자장수 렌터카의 시간당 비용 
  var B = defaultPrice; //코더랜드 렌터카 기본요금
  var C = defaultHour; //코더랜드 렌터카 기본시간
  var D = defaultCost; //코더랜드 렌터카 기본시간 이후 시간당 부과 요금

  cost1 = hour * price;
  cost2 = defaultPrice + (hour - defaultHour) * defaultCost;
  var min_cost;

  if (cost1 < cost2) {
      min_cost = cost1;
  } else {
      min_cost = cost2;
  }
  // 최소비용을 return 하세요.
  return min_cost;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 14. 마천루 🌟

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  var line = "";
  for (let i=1; i <= input; i++) {
      if (i <= 5) {
          for (let j=1; j <= i; j++) {
              line += "*";
          }
      } else {
          for (let j=1; j <= 5; j++) {
              line += "*";
          }
      }
      if (i !== input) {
          line += "\n";
      }
  }
  return line;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<Br>

### 15. 문자열 앞뒤 검사하기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(str) {
  var palindrome = [];
  for (let i = 0; i < str.length/2 ; i++) {
      //console.log(str[i]);
      //console.log(str[(str.length-1) - i]);
      var result = (str[i] == str[(str.length)-1 - i]);
      if (result) {
          palindrome.push("Same");
      } else {
          palindrome.push("Different");
      }
  }
  return palindrome.join("\n");
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 16. 수타박수 

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
  //console.log(input[1]);
  var total = 0;
  for (let i = 0; i < input.length; i++) {
      if (input[i] == "아메리카노") {
          total += 4100;
      } else if (input[i] == "카페라떼") {
          total += 4600;
      } else {
          total += 5100;
      }
  }
  return total;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<Br>

### 17. 반쪽짜리 피라미드 🌟

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(num) {
  //console.log(num);
  let line = "";
  for (let i=1; i <= num; i++) {
      for (let j=num-1; j >= i; j--) {
          line += " ";
      }
      for (let k=1; k<=i; k++) {
          line += "*";
      }
      // 맨 마지막줄 제외 줄바꿈 
      if (i !== num) {
          line += "\n";
      }
  } 
  return line;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 18. 좋아하는 숫자만 골라내기 🌟

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
    var num_tuple = ['2', '3', '5', '6', '7', '8', '9'];
    var result = [];
    
    for (let i = 0; i < input.length; i++) {
        if (num_tuple.includes(input[i])) {
            if (result.length < 5) {
                result.push(input[i]);
            } else {
                break;
            }
        }
    }
    return result;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 19. 잘린 피라미드 만들기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(a, b) {
    result = "";
    if (b > 15) {b = 15;}   // 최대 크기 제한
    
    if (a >= b) {
        result = "오류";
    } else {
        for (let i = a; i <= b; i++) {
            for (let j = 1; j <= i; j++) {
                result += "*";
            }
            // 현재 줄이 마지막 줄이 아니라면 줄바꿈 추가
            if (i !== b) {
                result += "\n";
            }
        }
    }
    return result;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<Br>

### 20. 겹치는 구간 찾기

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
    const range = input.split("\n");
    const A_start = Number(range[0]);
    const A_end = Number(range[1]);
    const B_start = Number(range[2]);
    const B_end = Number(range[3]);

    // 겹치는 구간 시작점, 끝점 찾기
    var min; var max; var answer = [];
    if (A_start <= B_start) {
        min = B_start;
    } else {
        min = A_start;
    }
    if (A_end <= B_end) {
        max = A_end;
    } else {
        max = B_end;
    }
    
    if (max < min) {
        return "X";     // 안겹치는 경우
    } else {
        answer.push(min);
        answer.push(max);
    }
    return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 21. 8은 특별해!

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution() {
    var cnt = 0;
    for (let i = 1; i <= 10000; i++) {
        var num = String(i);
        for (let j = 0; j < num.length; j++) {
            if (num[j] == "8") {
                cnt += 1;
            }
        }
    }
    return cnt;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 22. 끼리끼리

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(input) {
    var red_pocket = [];
    var blue_pocket = []
    var total_pocket = [];

    var card = input.split(" ");
    for (let i = 0; i < card.length; i++) {
        if (card[i] >= 0) {
            red_pocket.push(card[i])
        } else {
            blue_pocket.push(card[i]);
        }
    }
    total_pocket.push(red_pocket);
    total_pocket.push(blue_pocket);

    return total_pocket;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### 23. 암호문 해석하기

```jsx
// 암호의 알파벳을 키로, 대응하는 원문의 알파벳을 값으로 저장한 딕셔너리입니다.
var signal1 = {'a': 'n', 'b': 'd', 'c': 'a', 'd': 'b', 'e': 'e', 'f': 'l', 'g': 'j', 'h': 'o', 'i': 'z', 'j': 'u', 'k': 'y', 'l': 'v', 'm': 'w', 'n': 'q', 'o': 'x', 'p': 'r', 'q': 'p', 'r': 'f', 's': 'g', 't': 't', 'u': 'm', 'v': 'h', 'w': 'i', 'x': 'c', 'y': 'k', 'z': 's'}

var signal2 = {'a': 'z', 'b': 'y', 'c': 'x', 'd': 'w', 'e': 'v', 'f': 'u', 'g': 't', 'h': 's', 'i': 'r', 'j': 'q', 'k': 'p', 'l': 'o', 'm': 'n', 'n': 'm', 'o': 'l', 'p': 'k', 'q': 'j', 'r': 'i', 's': 'h', 't': 'g', 'u': 'f', 'v': 'e', 'w': 'd', 'x': 'c', 'y': 'b', 'z': 'a'}

// 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(code) {
    var code = code.split(" ");
    var code_num = code[0];
    var code_char = code[1];

    var answer = "";
    for (let i = 0; i < code_num.length; i++) {
        if (code_num[i] == 0) {
            answer += signal1[code_char[i]]
        } else {
            answer += signal2[code_char[i]]
        }
    }
    
    return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
// input = 01011 eowxvqp
```
<Br>

### 24. 겹치는 구간의 길이

```jsx
 // 지시사항을 참고하여 solution 함수 안에 코드를 작성하세요. 
function solution(a, b) {
    // 선분을 파싱하여 중심점과 길이 추출
    const aParts = a.split(',');
    const a_center = Number(aParts[0]);
    const a_length = Number(aParts[1]);

    const bParts = b.split(',');
    const b_center = Number(bParts[0]);
    const b_length = Number(bParts[1]);

    // 시작점과 끝점 계산
    const a_start = a_center - (a_length / 2);
    const a_end = a_center + (a_length / 2);
    const b_start = b_center - (b_length / 2);
    const b_end = b_center + (b_length / 2);

    // 겹치는 구간 시작점과 끝점 찾기
    const range_start = Math.max(a_start, b_start);
    const range_end = Math.min(a_end, b_end);
    
    if (range_end < range_start) {
        return 0;
    } else {
        return range_end - range_start;
    }
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```