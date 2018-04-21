문제 1

두 수를 입력받아 큰 수를 반환하는 함수를 작성하세요.

두 수 x, y

```js
function maxNum(x, y) {

    if ( x > y ) {
	return x;
	} else {
	  return y;
	}
}

maxNum(19, 9);

```

   

   

문제 2

세 수를 입력받아 그 곱이 양수이면 true, 0 혹은 음수이면 false, 둘 다 아니면 에러를 발생시키는 함수를 작성하세요.

에러를 발생시키는 코드는 다음과 같습니다.

+throw new Error('입력값이 잘못되었습니다.');

```js
function multiNum(x, y, z) {

  if ( x * y * z > 0 ) {
	return true;
	} else if ( x * y * z < 0 ) {
	return false;
	} else {
	throw new Error('입력값이 잘못되었습니다.');
	}
}

multiNum(3, 6, 9);

multiNum(3, -10, 9);

```

   

   

문제 3

세 수 min, max, input을 입력받아, 다음과 같이 동작하는 함수를 작성하세요.

min보다 input이 작으면, min을 반환합니다.

max보다 input이 크면, max를 반환합니다.

아니면 input을 반환합니다.

예:

```js
function limit( min, max, input ) {

  if ( min > input) {
	return min;
	} else if ( max < input ) {
		return max;
	} else {
		return input;
	}
}

limit(3, 7, 5);
limit(3, 7, 11);
limit(3, 7, 0);

```

   

   

문제 4

어떤 정수가 짝수인지 홀수인지 출력하는 함수를 작성하세요.

이를 이용해서, 1부터 20까지의 수가 각각 짝수인지 홀수인지 출력하는 프로그램을 작성하세요.

```js
function evenOrOdd(num) {
	if ( num % 2 === 0 ) {
		console.log('짝수 입니다');
	} else if ( num % 3 === 0) {
		console.log('홀수 입니다');
	}
}
evenOrOdd(15);
evenOrOdd(48);

```

   

   

문제 5

100 이하의 자연수 중 3과 5의 공배수를 모두 출력하는 프로그램을 작성하세요.

```js
function printNum(num){
if (num % 3 === 0 && num % 5 === 0) {
	console.log(num);
	}
}

let i = 0;
while (i <= 100) {
	printNum(i);
	i++;
	}

```

   

   

문제 6

자연수를 입력받아, 그 수의 모든 약수를 출력하는 함수를 작성하세요.

```js
function divisor(num) {
   for (let i = 0; i <= num; i++ ){
		if (num % i === 0) {
		console.log(i);
		}
	}
}

divisor(18);

6의 약수

1,2,3,6

```

   

​     

문제 7

2 이상의 자연수를 입력받아, 그 수가 소수인지 아닌지를 판별하는 함수를 작성하세요.

```js
function primeNum(num) {
	for (let i = 0; i >= 2; i++) {
		if (i % num === 0 && i % num === 1) {
			console.log( '${num} 은 소수입니다.' );
			} else {console.log('${num} 은 소수가 아닙니다.');
			}
		}
	}

primeNum(3);


2= 1,2

3= 1,3

5= 1,5

7= 1,7

11=1,11

```



