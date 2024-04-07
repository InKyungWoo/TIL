### [이론1] 연산자

- **산술 연산자**

```jsx
console.log(20 + 10)   // 30
console.log(20 - 10)   // 10
console.log(20 * 10)   // 200
console.log(20 / 10)   // 2
console.log(20 % 10)   // 0 -> 나머지 연산자
```

- 문자열도 산술 연산자 사용 가능
    - 덧셈만 문자열 이어 붙이기, 나머지는 숫자 처럼 연산됨

```jsx
console.log("20" + "10")   // 2010
console.log("20" - "10")   // 10  -> 숫자처럼 연산 됨
console.log("20" * "10")   // 200
console.log("20" / "10")   // 2
console.log("20" % "10")   // 0
```

- **증감 연산자**

```jsx
var num = 10;

console.log(++num);   // num+1 후 num 출력 -> 11
console.log(--num);   // num+1 후 num 출력 -> 9

console.log(num++);   // num 출력 후 +1 -> 10 (실제로는 11)
console.log(num--);   // num 출력 후 -1 -> 10 (실제로는 9)
```

- **비교 연산자**

```jsx
console.log(10 == 20);   // 값이 같다 -> False
console.log(10 === 20);  // 데이터 타입 & 값이 같다
console.log(10 != 20);   // 값이 같지 않다 -> True

console.log(10 > 20);
console.log(10 >= 20);
console.log(10 < 20);
console.log(10 <= 20);
```

- `**==` 와 `===` 의 차이**

```jsx
console.log(10 == "10");    //true
console.log(10 === "10");   //false
```

- **논리 연산자**

```jsx
/* AND 연산자 -> 앞 뒤 조건 모두 참일때만 true */
console.log(10 === 10 && 20 === 30);    //false

/* OR 연산자 -> 둘 중 하나만 참이면 true */
console.log(10 === 10 && 20 === 30);    //true
```

### [이론2] 조건문

주어진 조건에 따라 결과값을 출력하는 구문

조건에는 비교 연산자, 논리 연산자 사용

- **if문**
    - `if ( 조건 ) { 수행할 명령 }`
- **if ~ else문**
    - 조건이 true면 if문, false면 else문 실행

```jsx
var a = 20;
var b = 40;

if (a > b) {
	console.log("a는 b보다 크다");
} else {
	console.log("a는 b보다 작거나 같다");
}
```

- **else if문**
    - 여러개의 조건문을 생성
    - 위에서부터 순서대로 비교하면서 조건이 만족되면 명령 수행하고 끝남

```jsx
var a = 20;
var b = 40;
var c = 60;

if (a > b) { console.log("a는 b보다 크다");
} else if (b > c) { console.log("b는 c보다 크다");
} else if (a < c) { console.log("a는 c보다 작다");
} else if (b < c) { console.log("b는 c보다 작다");
} else {console.log("모든 조건을 만족하지 않는다.");
} 

// -> a는 c보다 작다
```

- **중첩 if문**

```jsx
var a = 20;
var b = 40;

if (a != b) {
	if (a > b) { console.log("a는 b보다 크다"); }
	else { console.log("a는 b보다 작다"); }
} else { console.log("a와 b는 같다"); }
```

### [이론3] 반복문

- **for문**
    - `for ( 초기화한 변수값; 조건; 증감표시 ) { 수행문 }`

```jsx
for (var i = 0; i < 10; i++) {
	console.log(i);
}
```

- **while문**
    - `while ( 조건 ) { 수행문 }`

```jsx
var num = 0;

while (num < 10) {
	console.log(num);
	num++;
}
```

- **do ~ while문**
    - `do { 수행문 } while ( 조건);`
    - while의 조건과 관계 없이, do의 명령을 무조건 실행부터 한다!

```jsx
var i = 12;

do {
	console.log(i);
	i++;
} whle (i < 10);
```

### [이론4] 자바스크립트 활용

- 주사위 게임

```jsx
var dice = Math.floor( Math.random() * 6 ) + 1;
```

- 소수 출력하기

```jsx
function isPrime(n) {
	var divisor = 2;              // 2부터 나누기 시작
	while (n > divisor) {         // n이 나누는 수보다 클 때까지
		if (n % divisor ===0) {     // 나누어 떨어지면 
			return false;
		} else {
			divisor++;                // 나누어 떨어지지 않으면 ++1  
		}
	} return true;
}
```

- 문자열 거꾸로 출력하기
    - 인덱스는 문자열 길이 -1

```jsx
function reverse(str) {
	var reverStr = '';        // 빈 문자열
	for (var i = str.length -1; i >= 0; i--) {
		reverStr = reverStr + str.charAt(i);       // i번째 문자를 빈 문자열에 추가
	} return reverStr;
}

console.log(reverse('Hello');    //olleH
```

---

### [실습]

- 구구단 만들기

```jsx
function timesTable(n) {
    for(var i = 1; i < 10; i++) {
        document.write(n,  " x ",  i, " = ", n * i, "<br>");
    }
}

timesTable(2); // 2단만 출력
timesTable(3); // 3단만 출력
```

```jsx
// 2단부터 9단까지 출력하는 반복문을 완성시켜 보세요.
for(var n = 2; n < 10; n ++) {
    for (var i = 1; i < 10; i++) {
        document.write(n, " x ", i, " = ", n * i, "<br>");
    }    
}
```