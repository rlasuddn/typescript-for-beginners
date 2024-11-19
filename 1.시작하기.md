# TypeScript 사용 이유

TypeScript는 다음과 같은 이유로 사용됩니다:

1. **타입 안정성**: 변수와 함수의 타입을 명확히 정의하여 예기치 않은 동작을 방지합니다.
2. **코드의 버그 감소**: 코드 작성 중 발생할 수 있는 오류를 사전에 발견하여 유지보수를 용이하게 만듭니다.
3. **런타임 에러 감소**: 실행 중 발생할 수 있는 오류를 컴파일 단계에서 차단합니다.
4. **생산성 증가**: 강력한 IDE 지원으로 코드 자동 완성, 리팩토링, 타입 체크를 통해 개발 속도가 향상됩니다.

---

## JavaScript의 단점

JavaScript는 유연성이 높아 코드 작성 시 에러를 명확히 보여주지 않는 경우가 많습니다.

```javascript
;[1, 2, 3, 4] + false // 결과: '1,2,3,4false'

function divide(a, b) {
    return a / b
}

divide(6, 3) // 결과: 2
divide("xxxxxxxx") // 결과: NaN
```

런타임 에러: 런타임 에러는 코드가 실행될 때만 발생하는 에러입니다.
TypeScript는 코드 실행 전에 타입과 구조를 확인하여 오류를 미리 알려줍니다.

```javascript
const kevin = { age: 17 }
kevin.hello() // TypeError: kevin.hello is not a function
```

브라우저: JavaScript만 이해하므로, TypeScript로 작성된 코드는 JavaScript로 컴파일됩니다.
Node.js: JavaScript와 TypeScript 모두를 이해할 수 있습니다.

TypeScript는 변수의 타입을 자동으로 추론합니다.
let a = 'hello'; // TypeScript는 a를 string으로 추론합니다.

필요한 경우 명시적으로 타입을 지정할 수 있습니다.

```typescript
let a: string = "hello"
```

TypeScript는 주로 타입 추론을 사용하지만, 타입 추론이 어려운 경우 개발자가 직접 명시합니다.

```typescript
let numbers: number[] = []
numbers.push(1) // 정상 동작

numbers.push("hello") // 오류: 'string' 타입은 'number' 타입에 할당할 수 없습니다.
```
