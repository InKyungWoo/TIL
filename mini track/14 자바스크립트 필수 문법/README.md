## TOC

[- 템플릿 리터럴](#템플릿-리터럴템플릿-리터럴) <br>
[- Split 메서드](#split-메서드) <br>
[- Sort 메서드](#sort-메서드) <br>
[- 아스키 코드](#ascii아스키-코드) <br>
[- Join 메서드](#join-메서드) <br>

<br>

### 템플릿 리터럴

- Javascript의 기능 중 하나로 문자열을 표현하는 새로운 방식, 백틱```` 으로 감싼다
- 문자열 내에 변수를 쉽게 삽입할 수 있는 `${  }` 표현식을 사용할 수 있다

```jsx
let name = "철수";
let age = 30;

let greeting = `안녕하세요, 제 이름은 ${이름}이고, 나이는 ${나이}살입니다.`;

console.log(greeting);  // "안녕하세요, 제 이름은 철수이고, 나이는 30살입니다." 출력
```

```jsx
// 줄바꿈 문자 없이 여러 줄 작성 가능
let multiLineString = `이것은
여러 줄에 걸친
문자열입니다.`;

console.log(multiLineString);
```

```jsx
// 지시사항을 참고하여 solution 함수 안에 코드를 작성하고 출력값을 return 하세요.
function solution(person) {
  //console.log(person);

  let person = {
	  name: '홍길동',
	  age: 30
  };
  let greeting = `안녕하세요, 제 이름은 ${name}이고, 나이는 ${age}살입니다.`;
  
  return greeting;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### Split() 메서드

- `split()` : 길이가 1인 배열 반환
- `split(separator)` : separator 기준으로 문자열을 나눠서 반환
- `split(separator, limit)` : 반환되는 배열의 최대 크기를 정해줌

```jsx
// 지시사항을 참고하여 solution 함수 안에 코드를 작성하고 출력값을 return 하세요.
function solution(word) {
	// word는 010-1234-5678
  const splits = word.split("-");
  return splits;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
//['010', '1234', '5678']
```
<br>

### Sort() 메서드

- 배열의 요소를 문자열로 변환 후, 문자열의 [유니코드](https://ko.wikipedia.org/wiki/%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C) 포인트 순서에 따라 정렬

```jsx
let arr = [40, 100, 1, 5, 25, 10];
arr.sort();
console.log(arr); // [1, 10, 100, 25, 40, 5]
```

- 그래서 비교함수를 함께 사용
    - 두 개의 인자를 받아, 양수를 반환하면 인자 두 개의 위치를 바꾸고, 음수나 0을 반환하면 위치를 그대로 유지

```jsx
// 오름차순 정렬

let arr = [40, 100, 1, 5, 25, 10];
arr.sort(function(a, b) {
  return a - b;
});
console.log(arr); // [1, 5, 10, 25, 40, 100]
```

```jsx
// 내림차순 정렬

let arr = [40, 100, 1, 5, 25, 10];
arr.sort(function(a, b) {
  return b - a;
});
console.log(arr); // [100, 40, 25, 10, 5, 1]
```

```jsx
// 지시사항을 참고하여 solution 함수 안에 코드를 작성하고 출력값을 return 하세요.
function solution(numbers) {
  //console.log(numbers);  -> [30, 20, 60, 50, 10]
  numbers.sort(function(a,b) {
      return a - b;
  });
  return numbers;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```
<br>

### **ASCII(아스키) 코드**

- Javascript에서 문자끼리 비교 연산을 수행할 때, 아스키 코드 값을 통해 비교할 수 있음

```jsx
const result = 'A' > 'B';
console.log(result);
// false
```

```jsx
// 지시사항을 참고하여 solution 함수 안에 코드를 작성하고 출력값을 return 하세요.
function solution(str1, str2) {
    if (str1 > str2) {
        return str1
    } else if (str1 < str2) {
        return str2
    } else {return "같음"};
    return;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```

### Join() 메서드

- 배열의 모든 요소를 연결하여 하나의 문자열로 만든다
- `arr.join(separator)` : 배열의 각 요소 사이에 추가되는 구분자. 이 인수가 생략되면 구분자는 쉼표(,)가 되고 마지막 요소 뒤에는 추가되지 않는다

```jsx
// 지시사항을 참고하여 solution 함수 안에 코드를 작성하고 출력값을 return 하세요.
function solution(words) {
  //console.log(words);
  let str = words.join(" ");
  return str;
}

// 실행 혹은 제출을 위한 코드입니다. 지우거나 수정하지 말아주세요.
module.exports = solution;
```