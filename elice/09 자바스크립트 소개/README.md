- [[이론1] 자바스크립트 소개](#---1-----------)
- [[이론2] 자바스크립트의 변수](#---2------------)
- [[이론3] 데이터 타입](#---3--------)
- [[이론4] 프로퍼티와 메서드](#---4-----------)


### [이론1] 자바스크립트 소개

- HTML: 웹사이트의 구조
- CSS: 웹사이트를 꾸며줌
- JavaScript: 동적인 웹사이트 (사용자와의 인터랙션)
> 💡 이미지 슬라이드 효과, 팝업 효과 등의 기능을 포함한 동적인 웹사이트 제작 시 사용되는 프로그래밍 언어 


<img width="763" alt="스크린샷 2024-04-01 오후 4 38 55" src="https://github.com/InKyungWoo/TIL/assets/102344718/b257e70b-844f-4fe3-9faf-195a22b0130a">

→ 범용적인 프로그래밍 언어! 

<br>

### [이론2] 자바스크립트의 변수

- **변수 선언 및 데이터 저장**
    - `변수` : 데이터를 담는 공간
    - `변수 선언` : 데이터를 담을 공간을 생성하는 것
    - `변수 초기화` : 생성된 변수에 데이터를 전달하는 것

```jsx
var fruit;          // 변수 선언
fruit = "apple"     // 변수 초기화

var fruit = "apple"; // 변수 선언 및 초기화
```

- **데이터 변경**

```jsx
var fruit = "apple";

fruit = "banana";
```

fruit 라는 변수의 데이터를 apple → banana로 변경, (또 다른 변수를 선언할 필요는 X)

- **데이터 확인 방법**

```jsx
var fruit = "apple";

console.log(fruit);   // apple 출력됨
```

- **변수 생성 시 주의사항**

```jsx
// 변수 명은 숫자로 시작할 수 없음
var 1str;

// 변수명은 최대한 자세하게 작성
var randomNumber;

// 의미가 불명확한 단어들의 조합은 피하기
var tmax;
var timeMax;
```

- **자바스크립트 사용 방법**

```jsx
<body>
	<script src="index.js"></script>
</body>
```

→ `<script> 태그 안에 src의 속성값으로 js 파일을 입력 후 html 파일과 연동`

```jsx
document.write();     // 웹 화면에 출력
document.writeln();   // 출력값 사이에 공백 넣기
```

<br>

### [이론3] 데이터 타입

<img width="747" alt="스크린샷 2024-04-01 오후 4 39 19" src="https://github.com/InKyungWoo/TIL/assets/102344718/5a33bf4d-eca6-4c34-8701-279ad14fb209">


1. **문자열**
- “” , ‘’ 안에 작성된 데이터
- `“He’s a boy”;`, `‘He\’s a boy’;`

2. **숫자**
- 별도의 기호 없이 입력 (정수, 음수, 실수 등)

3. **함수**
- 함수 생성: function 키워드를 사용하여 생성
- 함수 호출: 함수 안에 있는 코드를 실행시키겠다는 의미

```jsx
var func1 = function() {
	console.log("Func1";)
}  //함수 생성

func1();  //함수 호출
```

```jsx
function func1() {
	console.log("Func1";)
}  //함수 생성

func1();  //함수 호출
```

<img width="759" alt="스크린샷 2024-04-01 오후 4 39 52" src="https://github.com/InKyungWoo/TIL/assets/102344718/67927424-7cd6-4e7d-8143-b833553e2834">

4. **배열**
- 비슷한 성격을 갖고 있는 데이터를 하나의 변수 안에서 관리

```jsx
var fruit = ["사과", "배", "수박"];

console.log(fruit);     //["사과", "배", "수박"]
console.log(fruit[0]);  // "사과"
```

- **배열 데이터 변경하기**

```jsx
var fruit = ["사과", "배", "수박"];
fruit[0] = "포도";

console.log(fruit);   //["포도", "배", "수박"]
```

5. **객체**
   
<img width="766" alt="스크린샷 2024-04-01 오후 4 40 13" src="https://github.com/InKyungWoo/TIL/assets/102344718/cbdd6feb-6c53-4e66-992b-07761844442b">

```jsx
var student = {
	name : "inkyung",
	age : 20,
	skills : ["js", "html", "CSS"],
	sum : function(num1, num2) {
		return num1 + num2;
	}
}

console.log(student.name);     // inkyung 출력
console.log(student['name']);  // inkyung 출력

student.name = "minju";        // name 프로퍼티의 데이터 변경
console.log(student.name);     // minju 출력
```

6. **불린**
- 참 또는 거짓 데이터가 들어가 있는 상태

```jsx
var t = true;
var f = false;
```

7. **undefined**
- 변수 안에 데이터를 입력하지 않은 상태 `데이터 없음`

```jsx
var unde;
```

8. **null**
- 임의로 변수 안에 빈 데이터를 삽입한 상태 `빈 데이터를 지정`

```jsx
var empty = null;
```

<br>

### [이론4] 프로퍼티와 메서드

- **문자열 프로퍼티와 메서드**

```jsx
var str1 = "Hello World";
 
str1.length;        // 문자열 길이 11
str1.charAt(0);     // 문자 H 추출
str1. split(" ");   // 공백 기준으로 문자 나눈 후 배열로 출력 [Hello, World]
```

- **배열 프로퍼티와  메서드**

```jsx
var fruit = ["js", "html", "CSS"];

fruit.length;            // 데이터 개수

fruit.push("python");    // 배열 뒤에 데이터 삽입 ["js", "html", "CSS", "python"]
fruit.unshift("java");   // 배열 앞에 데이터 삽입 ["java", "js", "html", "CSS", "python"]

fruit.pop();    // 배열 뒤의 데이터 제거 ["java", "js", "html", "CSS"]
fruit.shift();  // 배열 앞의 데이터 제거 ["js", "html", "CSS", "python"]
```

- **math 라이브러리의 수학 연산 메서드**

```jsx
Math.abs(-3);      // 절대값 -> 3
Math.ceil(0.3);    // 올림 -> 1
Math.floor(10.9);  // 내림 -> 10
Math.random();     // 임의의 숫자 출력
```

- **문자를 숫자로 변환하는 메서드**

```jsx
parseInt("20.6");    // 정수 형태의 20 변환
parseFloat("20.6");  // 실수 형태의 20.6 변환
```

> 참고
> 

[String - JavaScript | MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String)
