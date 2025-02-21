# 연산자의 이해

Swift에서 연산자(operator) 는 값에 대한 연산을 수행하는 특별한 기호 또는 키워드입니다. Swift는 기본 제공 연산자뿐만 아니라 사용자 정의 연산자도 지원합니다.
## 산술 연산자 (Arithmetic Operators)

|연산자|설명|예제|
|:------|:---|:---|
|+|덧셈|let sum = 10 + 5|
|-|뺄셈|let diff = 10 - 5|
|*|곱셈|let product = 10 * 5|
|/|나눗셈|let quotient = 10 / 5|
|%|나머지 연산|let remainder = 10 % 3|

**예시코드**
```swift
let a = 10
let b = 3
print("덧셈: \(a + b), 뺄셈: \(a-b)")
print("곱셈: \(a * b), 나눗셈: \(a / b), 나머지: \(a % b)")

//13
//7
//30
//3
//1
```
## 비교 연산자 (Comparison Operators)

|연산자|설명|예제|
|:------|:---|:---|
|==|값이 같은지 비교|a == b|
|!=|값이 다른지 비교|a != b|
|>|왼쪽 값이 더 큰지 비교|a > b|
|<|오른쪽 값이 더 큰지 비교|a < b|
|>=|왼쪽 값이 크거나 같은지 비교|a >= b|
|<=|오른쪽 값이 크거나 같은지 비교|a <= b|

**예시코드**
```swift
let score1 = 85
let score2 = 90
print("점수 비교: \(score1 > score2)")

//False
```

## 논리 연산자 (Logical Operators)

|연산자|설명|예제|
|:------|:---|:---|
|&&|AND (둘 다 참이어야 참)| true && false -> false|
|!|NOT (참을 거짓으로, 거짓을 참으로)|!true -> false|
| &#124;&#124;|OR (둘 중 하나가 참이면 참)|true  &#124;&#124; false -> true|

**예시코드**

```swift
let isRainy = true
let isCold = false
print("비 오고 춥나요? \(isRainy && isCold)")
print("비 오거나 춥나요? \(isRainy || isCold)")

//False
//True
```

## 할당 연산자 (Assignment Operators)

|연산자|설명|예제|
|:------|:---|:---|
|=|값 할당|var x = 10|
|+=|더한 후 할당|x += 5 // x = x +5|
|-=|뺀 후 할당|x -= 5 // x = x -5|
|*=|곱한 후 할당|x *= 2 // x = x * 2|
|/=|나눈 후 할당|x /= 2 //x= x / 2|

**예시코드**

```swift
var number = 10
number += 5
print("현재 값: \(number)")

//15
```
이를 바탕으로 실습을 해보았다.

**실습1**

```swift
let num1 = 12
let num2 = 7

let sum = num1 + num2
let difference = num1 - num2
let product = num1 * num2
let quotient = num1 / num2
let remainder = num1 % num2

print("덧셈: \(sum), 뺄셈: \(difference)")
print("곱셈: \(product), 나눗셈: \(quotient), 나머지: \(remainder)")

//덧셈: 19
//뺄셈: 5
//곱셈: 84
//나눗셈: 1
//나머지: 5
```

**실습2**

```swift
let height1 = 170
let height2 = 165

print("키비교: \(height1 > height2)")
print("같은 키인가요? \(height1 == height2)")

//키비교: true
//같은 키인가요? false
```

**실습3**

```swift
let isSunny = true
let isWeekend = false

let goOutside = isSunny && isWeekend
let stayHome = !isSunny

print("외출할까요? \(goOutside)")
print("집에 있을까요? \(stayHome)")

//외출할까요? false
//집에 있을까요? false
```

**실습4**

```swift
var points = 50

points += 10
print("현재 점수: \(points)")

points *= 2
print("현재 점수: \(points)")

//현재 점수: 60
//현재 점수: 120
```

**실습5**

```swift
let score = 85

if score >= 90 {
    print("A 등급입니다!")
} else if score >= 80 {
    print("B 등급입니다!")
} else if score >= 70 {
    print("C 등급입니다!")
} else {
    print("더 노력하세요!")
}

//B 등급입니다!
```
Swift 연산자 학습 고찰
이번 실습을 통해 Swift의 다양한 연산자에 대해 학습하고, 실제 코드로 적용해보는 경험을 할 수 있었다. 연산자는 프로그래밍에서 가장 기본적인 개념이지만, 단순한 계산을 넘어서 논리적인 흐름을 만들고, 변수의 값을 효율적으로 조작하는 데 필수적이라는 점을 다시 한번 깨닫게 되었다.

1. 주요 학습 내용

- 산술 연산자를 통해 기본적인 계산을 수행하는 방법을 익혔다.
- 비교 연산자를 활용하여 값의 크기를 비교하고 조건문과 함께 사용할 수 있음을 확인했다.
- 논리 연산자를 통해 여러 조건을 조합하여 논리적인 흐름을 제어할 수 있었다.
- 할당 연산자를 사용하여 변수 값을 간결하게 갱신하는 방법을 실습했다.
2. 실습을 통해 느낀 점
각 연산자의 개념을 이해하는 것보다, 실제로 코드를 작성하면서 어떤 상황에서 어떤 연산자를 사용하는 것이 적절한지 고민하는 과정이 더 중요하다는 것을 깨달았다. 예를 들어, 논리 연산자를 활용하여 조건문을 단순하게 표현하거나, 할당 연산자를 사용해 코드의 가독성을 높이는 것이 중요했다.

또한, 연산자 우선순위(Precedence)를 고려하지 않으면 예상과 다른 결과가 나올 수도 있기 때문에, 연산자의 실행 순서를 명확히 이해하고 괄호를 적절히 사용하는 것이 필요하다고 생각했다.

3. 보완할 점 및 추가 학습 필요성
연산자의 기본적인 활용법을 익혔지만, 아직 비트 연산자(Bitwise Operators), 삼항 연산자(Ternary Operator), 사용자 정의 연산자(Custom Operator) 등 심화적인 내용이 더 있다는 점을 알게 되었다. 

4. 실제 활용 가능성
Swift 연산자는 단순한 계산뿐만 아니라, UI 개발, 데이터 처리, 알고리즘 구현 등 다양한 프로그래밍 영역에서 필수적으로 활용된다. 예를 들어,

- 조건문과 논리 연산자를 활용하여 앱의 UI 상태를 동적으로 변경할 수 있다.
- 산술 및 비교 연산자를 사용하여 게임 개발에서 캐릭터의 체력, 점수 등을 관리할 수 있다.
- 할당 연산자를 적절히 사용하면 가독성이 높은 코드를 작성할 수 있다.
이러한 점에서 Swift 연산자는 단순한 문법이 아니라, 실제 개발에서 효율적인 코드 작성에 중요한 요소라는 점을 다시금 확인할 수 있었다.

5. 결론
이번 학습을 통해 Swift 연산자의 개념을 확실히 이해하고, 이를 활용한 간단한 프로그램을 작성할 수 있는 능력을 키울 수 있었다. 하지만, 단순한 문법 암기를 넘어 실무에서 어떻게 활용할지 고민해보는 것이 중요하며, 보다 심화된 연산자 개념을 익혀서 코드 최적화 및 가독성을 높이는 방향으로 나아가야겠다고 생각한다.
