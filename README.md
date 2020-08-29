# 코드숨 모던 자바스크립트 정주행 스터디 질문모음집

https://ko.javascript.info/

## 3.1 Chrome으로 디버깅하기

* 디버깅을 할 줄 안다면 개발할 때 어떤 이점이 있을까요?
* 실행 추적에서 step, step over, step into, step out의 차이
* 브레이크포인트는 코드 작성할 때 잡아줄 수 있다? 없다?
* 중단점을 설정하기는 귀찮은데 해당 줄에서 실행을 재개하고 싶을 때 아주 유용한 옵션은?
* 디버깅을 유용하게 사용 해 본 사례가 있다면 공유 부탁드립니다. 전 안써봐서...
* Chrome 개발자 도구에서 자신이 사용하는 유용한 기능이 있다면?
* 여러분들은 디버깅 툴을 이용하는지, console.log로만 하고 있는지, 자바스크립트 도구 call stack 부분을 본적이 있는지요~

## 3.2 코딩 스타일

* 가독성이 좋고 이해하기 쉬운 코드를 만들려면 무엇을 해야할까요? 에러를 피하려면 어떻게 해야할까요?
* 정의한 함수의 끝에 세미콜론을 붙이는가?
* 호출부를 먼저 쓰고 헬퍼 함수를 나중에 두는 방식의 장점은?
* 문자열을 여러 줄로 쉽게 나눌 때, 어떤 걸 사용하면 좋을까요?
* 중첩레벨을 줄이는 자신만의 방법이 있다면?
* Linter를 왜 사용할까요?

## 3.3 주석

* 좋은 주석이란 무엇인가요?
* 주석에 들어가면 좋지 않은 내용은 무엇인가?
* 좋은 주석과 나쁜 주석을 설명해주세요
* 주석에 들어가면 좋지 않은 내용에는 어떤게 있을까요?
* (책의 설명과 상관없이 자신이 생각했을 떄) 좋은 주석이란?
* 주석에 들어가면 좋은 내용 과 주석에 들어가면 좋지 않은 내용 예로 뭐가 있을까요?

## 3.4 닌자 코드

* 유사한 뜻을 가진 단어 여러개를 같은걸 나타내는데 섞어서 사용하면 어떤 일이 발생하나요?
* 닌자코드를 작성해본 경험이 있는가?
* 닌자코드는 좋은 걸까요 나쁜 걸까요
* 닌자 코드 예시 중 가장 생각나는 예시는?
* 가장 찔렸던 구절이 있다면?
* 약어를 사용하여 코드의 양을 줄이면 좋은 방법인가요? O,X

## 3.5 테스트 자동화와 Mocha

* 테스트는 왜 해야할까요?
* BDD란 무엇인가?
* 테스트 자동화의 장점은?
* before와 beforeEach의 차이는?
* BDD와 TDD의 차이는?
* 테스트는 왜 할까요?

## 3.6 폴리필

* 바벨의 역할은 무엇인가요?
* 폴리필은 어떨 때 사용하는가?
* js 엔진에 구현이 누락된 새로운 기능을 쓸수 있게 해주는 스크립트의 명칭은?
* 모던 자바스크립트 코드를 구 표준을 준수하는 코드로 바꿔주는 역할을 하는 것은?
* babel과 polyfill의 차이는 무엇인가요 ?
* 폴리필과 트랜스파일러의 차이는?
* 바벨을 왜 사용할까요?
* 자료구조와 자료형

## 4.1 객체

* 객체의 프로퍼티 이름에 제약사항이 있는가?
* const로 선언된 객체는 값을 변경할 수 있다? 없다?
* Object는 모든 프로퍼티에 대해서 객체가 추가한 순서 그대로 정렬된다.[O/X]
* 점 표기법과 대괄호 표기법의 가장 큰 차이점은 무엇일까요?
* 정수 프로퍼티를 사용할 때의 장단점은 무엇일까?
* 대괄호 표기법은 언제 사용하면 좋은가?(2가지)

## 4.2 참조에 의한 객체 복사

* 참조에 의해 저장되고 복사된다는 것은 무슨 의미인가요? 원시 타입이랑 무엇이 다른가요?
* 깊은 복사를 하기위해서는 어떻게 하면 되는가?
* 똑같은 내용의 객체를 서로 다른 변수로 선언한 뒤 비교 연산자로 비교하면 true? false?

```js
let a = {};
let b = {};
alert( a == b ); // 결과는?
```

* 리액트에서 중첩된 객체를 복사할 때 사용하는 라이브러리는 무엇이 있을까요?
* `Object.assign`을 활용하여 객체를 복사하는 코드를 작성해본다면?

```js
const array1 = [1,2,3];
const arrayCopy = array1;
1) array1 === arrayCopy ?
arrayCopy.push(4);
2) array1's values
arrayCopy = [...arrayCopy];
3) arrayCopy's values

const date = new Date();
const date2 = date;
date.setHours(10);
4) date.getHours()
5) date2.getHours()

// 각 답을 말하시오.(5문제)
```

## 4.3 가비지 컬렉션

* 도달가능성이란 무엇인가요?
* 가비지 컬렉션을 더 빠르게 하는 최적화 기법은 무엇이 있는가?
* 가비지 컬렉션은 개발자가 제어할 수 있다? 없다?
* (이 파트는 제가 아직 이해를 못해서 질문은 못만들겠어요ㅠ)
* 가비지 컬렉션은 어떤 기준으로 메모리를 관리하나요?
* (상상해본다면?!) 우리가 선언한 것들 (원시값, 객체, 함수) 중 몇 퍼센트는 계속 유지되고 몇 퍼센트가 가비지 컬렉션이 될까?
* 전역 객체의 변수와 전역 변수의 차이는 무엇인가요?

## 4.4 메서드와 'this'

* this를 사용할 때 주의할 점은 무엇인가요?
* 화살표 함수가 유용한 경우는 언제인가?
* 화살표 함수에서의 this는 무엇을 의미할까?
* 메서드 내부에서의 this 와 화살표 함수 내부에서의 this의 차이는?
* this의 과제 첫번째 문제가 이해되지 않습니다 ㅠ
* `this` 사용시, 화살표함수를 쓰면 좋은 경우를 설명해보기
* 1) 엄격모드일 때, this와 아닐 때 this는 어떻게 바인딩 되는가요? 2) 함수와 메서드의 차이가 무엇일까요?

## 4.5 'new' 연산자와 생성자 함수

* new로 실행한 함수로 그냥 실행한 함수가 동작이 어떻게 다른가요?
* 생성자함수의 관례
* 생성자 함수에서 기본으로 반환되는 값은?
* 생성자 함수의 2가지 관례는?
* 생성자 함수를 썼을 때 일어나는 일(알고리즘?)을 설명해본다면?
* 1) new 연산자를 사용하는 이유는 무엇일까요? 2) new 연산자를 이용하여 함수를 호출하면 어떤 동작을 하게 되나요?

## 4.6 옵셔널 체이닝 '?.'

* 옵셔넌 체이닝의 세가지 사용법에 대해 설명해주세요
* 옵셔널 체이닝은 왜 필요한가?
* 옵셔널 체이닝이 등장한 이유는?
* ?. 은 쓰기 뿐만 아니라 읽기나 삭제하기에는 사용할 수 있다. [O/X]
* 옵셔널 체이닝이 필요한 경우를 설명해본다면?
* 언제 사용하면 좋을까요?

## 4.7 심볼형

* 심볼형은 언제 사용하는가?
* Object.assign을 이용한 복사는 심볼형 데이터를 복사 한다? 안한다?
* 심볼은 문자형으로 자동 형 변환된다. [O/X]
* 숨김프로퍼티의 특징은?
* 1) 심볼형을 왜 사용할까요? 2) 동일한 심볼값을 만드는 방법과 전역 심볼을 만드는 방법은 무엇인가요?

## 4.8 객체를 원시형으로 변환하기

* hint의 세가지 종류는?
* alert 함수같이 문자열을 기대하는 연산을 수행할 때는(객체-문자형 변환), hint가 string이다. [O/X]
* 객체를 primitive type으로 변환할 때, hint가 될수 있는 세 가지를 나열해본다면?

```js
let obj = {
    toString() {
        return "3";
    }
};

console.log(obj + obj * obj + 2);
// 의 값은 무엇이 나올까요?
```

## 5.1 원시값의 메서드

* 원시값과 객체의 차이는 무엇인가요?
* 원시값이 객체처럼 사용되는 과정
* 원시형에 프로퍼티를 추가했을 때 엄격모드 / 비 엄격모드의 차이점
* 자바스크립트의 원시형 타입 7가지는?
* 1) 원시값 무엇이 있는지 말해주세요. 2) 원시값의 메서드가 객체의 메서드보다 좋을 땐 언제일까요?

## 5.2 숫자형

* 왜 0.1 + 0.2 는 0.3이 아니라 0.3000000000004 일까요?
* n진법 문자형으로 변환하는 메서드
* object.is 와 ===의 차이
* 정밀도 손실 개념을 설명해주세요
* isFinite(' ') 의 결과값은?
* isFinite('') 의 결과값은?

## 5.3 문자열

* Single quotes 나 Double quotes대신에 Back tick( ` )을 쓰면 좋은 경우가 어떤 경우가 * 있을까요?
* 특정 언어에 적합한 비교 기준 사용해 문자열을 비교하려면 어떤 메서드를 써야 하는가?
* substring, substr 차이
* 백틱을 이용한 문자열의 특징 두가지를 설명해주세요
* 문자열의 특정 위치를 접근할 때, [] 로 접근하는 방법과 charAt() 을 사용하여 접근하는 방법이 있습니다. 만약 찾고자하는 자리가 없는 자리일 경우 각각 무엇을 반환할까요?

## 5.4 배열

* 객체로도 똑같이 동작하게 만들 수 있지만 배열을 써야하는 이유는 무엇일까요?
* 배열을 복사하게 되면 shallow copy가 되는가 deep copy가 되는가?
* 배열을 객체처럼 쓰지 말아야하는 이유
* 자바스크립트에서 배열 요소는 같은 자료형만 허용한다? 아니다?
* 배열은 특별한 종류의 객체이다? O , X

## 5.5 배열과 메서드

```js
let arr = [ 1, 2, 15 ];
arr.sort();

// 의 결과가 1, 15, 2인 이유는 무엇인가요?
```
* forEach 내부 함수에서 첫번째, 두번째, 세번째 매개변수가 각각 무슨 역할을 하는가?
* includes와 indexOf/lastIndexOf의 차이
* 기존 배열을 변형시키는 배열 메서드를 하나만 설명해주세요
* slice는 새로운 배열을 반환하나요? O, X
* 객체와 배열을 typeof 로 비교할 경우 둘다 객체로 나옵니다. 그럼 어떻게 구분할 수 있을까요?

## 5.6 iterable 객체

* iterable 객체란 무엇인가요?
* iterable은 무엇인가?
* iterable 객체와 유사배열의 차이
* 문자열을 배열로 만들 수 있는 방법 중 split() 을 이용한 방법 말고 또 뭐가 있을까요?

## 5.7 맵과 셋

* 객체와 맵의 차이는 무엇인가요?
* 셋은 언제 사용되나요?
* 맵과 객체의 차이점
* 맵과 셋의 차이
* 일반 객체와 맵의 차이점은?
* 맵의 키로 객체를 키로 사용할 수 있나요?

## 5.8 위크맵과 위크셋

* 위크맵과 위크셋을 어디에 활용할 수 있을까요?
* 맵과 위크맵, 셋과 위크셋의 차이점
* 순환참조 안되는이유
* 위크맵, 위크셋은 구성 요소 전체를 대상으로 하는 메서드를 지원한다? 안한다?
* 위크맵과 맵의 차이점은 무엇일까요?

5.9 Object.keys, values, entries

* Object.keys, values, entries 각각 무슨 일을 하는지 설명해주세요
* Object의 메서드인 keys, value, entries에 대해서 설명
* 해당 메소드들을 적용할 수 있는 자료구조의 종류
* 객체에 배열 전용 메서드를 적용하는 방법은?
* map.keys 와 Object.keys // 즉, 맵과 객체의 반환값 차이는 뭘까요?

## 5.10 구조 분해 할당

* 디스트럭처링을 이용해서 함수에 객체를 전달할 때, 그냥 변수를 펼쳐서 전달하는 것과 객체로 전달했을 때 * 어떤 장점이 있을까요?
* 기본값을 사용해도 괜찮을 경우 인자로 무엇을 넘겨주면 되는가?
* 함수 매개변수를 구조 분해할 때 기본값을 설정해주는 두가지 방법은?
* [guest, admin] = [admin, guest] 는 뭘 하는건가요?

5.11 Date 객체와 날짜

* YYYY-MM-DDTHH:mm:ss.sssZ 각 문자열이 무엇을 나타내는지 설명해주세요
* Date 객체에 자동고침이란?
* Date 객체를 만들지 않고도 시차를 측정할 방법과 장점
* Date 객체에서 날짜나 시간만 따로 저장하는 것은 가능하다? 불가능하다?
* getDay() 의 0 은 뭘 나타낸걸까요?
* 전날을 알고 싶을 경우 어떻게 하면 될까요?

## 5.12 JSON과 메서드

* JSON.parse의 reviver는 무엇인가요? 언제 사용하나요?
* JSON.stringify(value[, replacer, space]) 에서 replacer의 용도
* JSON.stringify를 사용할 때 주의하셔야 할 점
* reviver 개념에 대해 설명해주세요
* JSON.stringify() 를 이용하여 문자열로 변하는 메서드를 사용했을 때, 무시되는 프로퍼티 3가지가 무엇이 있을까요?

## 6.1 재귀와 스택

* 재귀 호출이 어떻게 동작하는지 내부 동작 설명
* 실행 컨텍스트란?
* 재귀적 자료 구조의 예시를 들어주세요
* 재귀의 장점은 무엇입니까!!!ㅣ

## 6.2 나머지 매개변수와 전개 문법

* 나머지 매개변수가 중간에 있어도 상관 없는가?
* arguments의 특징, arguments로 배열 메소드를 사용하기 위한 방법
* 나머지 매개변수와 전개 문법의 사용 패턴에 대해 설명해주세요
* 전개 문법은 어떤 객체에만 사용할 수 있나요?

## 6.3 변수의 유효범위와 클로저

* 클로저란 무엇인가?
* 클로저란?
* 클로저에 대해 설명해주세요
* 클로저란 무엇인가요?

## 6.4 오래된 'var'

* 호이스팅이란?
* 즉시 실행 함수 표현식를 사용했던 이유
* var를 권장하지 않는 이유는?
* var 키워드를 이용할 경우 일어나는 현상은 무엇이 있을까요?

## 6.5 전역 객체

* 표준화 시도를 하고있는 전역 객체 이름은?
* 모던 자바스크립트에서 전역변수를 사용할때 권장되는 방식
* 전역 객체를 가급적 사용하지 않는 이유는?
* 전역 객체의 보편적인 이름은 무엇일까요? 표준 스펙이도 들어있습니다.
* 전역 변수는 다른 곳에서도 자유롭게 쓸 수 있게 하기 위해서 자주 사용하는게 좋다 O, X

## 6.6 객체로서의 함수와 기명 함수 표현식

* 기명 함수 표현식은 어떨 때 유용한가?
* 자바스크립트의 다형성을 구현하는 방법
* 기명 함수 표현식 사용 이유
* 함수 표현식에 이름을 붙이면 유리한 점은?

## 6.7 'new Function' 문법

* new Function으로 정의한 함수는 어떤 장점이 있는가?
* new Function을 이용해 만든 함수와 일반 함수의 차이점
* new Function 문법으로 함수 생성시 특징은?
* 기존에 사용하던 방법과 new Function을 사용해 함수를 만드는 방법의 가장 큰 차이는 뭘까요?

## 6.8 setTimeout과 setInterval을 이용한 호출 스케줄링

* setTimeout과 setInterval의 차이점
* 중첩 setTimeout이 setInterval에 비해 가지는 장점
* 스케줄링 메서드에 명시된 시간이 보장되지 않는 경우 세가지는?
* 중첩 setTimeout과 setInterval 을 이용하여 1초마다 작업을 수행한다고 했을 때, 차이점은 무엇일까요?

## 6.9 call/apply와 데코레이터, 포워딩

* call과 apply 메서드는 무슨 일을 하는가?
* 데코레이터 함수란?
* 데코레이터가 무엇일까요?

## 6.10 함수 바인딩

* 메서드를 콜백으로 전달할 때 ’this 정보가 사라지는’ 문제를 어떻게 해결 할 수 있는가?
* 메서드를 전달할 때, 컨텍스트도 제대로 유지하려면 어떻게 해야 할까요?
* 함수의 컨텍스트를 고정해서 넘길 때 사용하는 방법 두가지는?

```js
function sayHi() { alert(this.name); }
sayHi.test = 5;

let bound = sayHi.bind({ name: '윤석님!' });

alert(bound.test);

// 의 값과 이유를 알려주세요.
```

## 6.11 화살표 함수 다시 살펴보기

* 화살표 함수는 어떤 경우 사용하면 유용한가?
* 화살표 함수가 일반 함수와 다른 점은?
* 화살표 함수에는 일반 함수와 달리 무엇과 무엇이 없을까요?
