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