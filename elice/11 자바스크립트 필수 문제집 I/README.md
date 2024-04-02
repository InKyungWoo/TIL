- 어서와

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
  return "Hi, Elice";
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 여러 줄로 출력하기

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
  return "400\nbus\nlike";
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 따옴표 출력하기

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
  return '"It\'s all right."';
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 버스 좋다

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
    var num = 400;
    var str1 = "bus";
    var str2 = "like";
    var result = num + " " + str1 + " " + str2
  return result;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 숫자와 문자열

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
    var num1 = 1;
    var num2 = 2;
    var str1 = "1";
    var str2 = "2";
  return [num1 + num2, str1 + str2];
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- N줄 입력받기

```jsx
// solution 함수 안에 N줄에 걸쳐 주어지는 문자열을 배열로 만들어 출력하세요.
function solution(input) {
  var answer;
  answer = input.split('\n');
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 문자열 자르기

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution(str) {
  var answer = [];

  var str = str.split(' ');
  answer[0] = typeof str;
  answer[1] = str[0];
  
  return answer;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 용돈 압수

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution(money) {
    //console.log(money);
    var str = [];
    str = money.split("500원");
  return str;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 훈민정음

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution(hangul) {
    //console.log(hangul);
    var result = hangul[0] + hangul[47] + hangul[23];
  return result;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

- 함수 만들고 호출하기

```jsx
// solution 함수 안에서 지시사항을 수행해보세요.
function solution() {
    function add (x, y) {
        return x + y;
    }
  return add;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```