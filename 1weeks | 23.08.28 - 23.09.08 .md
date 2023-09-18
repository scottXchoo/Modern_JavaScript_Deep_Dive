> 23.08.28(월) - 23.09.08(금)

# 01장. 프로그래밍
## 1.1 프로그래밍이란?
**문제(요구사항)를 명확히 이해하는 것**이 우선되어야 하며 **복잡함을 단순하게 분해(decomposition)** 하고 **자료를 정리하고 구분(modeling)** 해야 하며 **순서에 맞게 행위를 배열** 해야 한다.

## 1.2 프로그래밍 언어
컴파일러(complier) 혹은 인터프리터(interpreter) => 컴퓨터가 이해할 수 있는 기계어로 변환하는 일종의 번역기

## 1.3 구문과 의미
프로그래밍은 요구사항의 집합을 분석해서 적절한 자료구조와 함수의 집합으로 변환한 후, 그 흐름을 제어하는 것이다.

---

# 02. 자바스크립트란?
## 2.1 자바스크립트의 탄생
- **1996년 3월 :** 넷스케이프 커뮤니케이션즈의 웹 브라우저인 넷스케이프 내비게이터2에 탑재되었고 "모카(Mocha)"로 명명되었다.
- **1996년 9월 :** "라이브스크립트(LiveScript)"로 이름이 바뀌었다.
- **1996년 12월 :** "자바스크립트(JavaScript)"라는 이름으로 최종 명명되었다.

## 2.2 자바스크립트의 표준화

- **1996년 11월 :** 넷스케이프 커뮤니케이션즈는 컴퓨터 시스템의 표준을 관리하는 비영리 표준화 기구인 ECMA 인터내셔널에 자바스크립트의 표준화를 요청한다.


- **ECMAScript 버전별 특징**
  - ES1 - 1997년 : 초판
  - ES5 - 2009년 : HTML5와 함께 출현한 표준안
  - ES6(ECMAScript 2015) - 2015년
  : let/const, 클래스, 화살표 함수, 템플릿 리터럴, 디스트럭처링 할당, 스프레드 문법, rest 파라미터, 심벌, 프로미스, Map/Set, 이터러블, for ... of, 제너레이터, Proxy, 모듈 import/export
  
## 2.3 자바스크립트 성장의 역사

### 2.3.1 Ajax

**1999년 :** 자바스크립트를 이용해 서버와 브라우저가 **비동기(asynchronous)** 방식으로 데이터를 교환할 수 있는 통신 기능인 **Ajax(Asynchronous JavaScript and XML)** 가 **XMLHttpRequest** 라는 이름으로 등장했다.

**Ajax 기능 :** 웹페이지에서 변경할 필요가 없는 부분은 다시 렌더링하지 않고, 서버로부터 필요한 데이터만 전송받아 변경해야 하는 부분만 한정적으로 렌더링하는 방식이 가능해진 것이다. (패러다임 획기적으로 전환)

**2005년 :** 구글이 발표한 구글 맵스(Google Maps)는 웹 애플리케이션 프로그래밍 언어로서 자바스크립트의 기능성을 확인하는 계기를 마련했다.

### 2.3.2 jQuery

**2006년 :** jQuery의 등장으로 다소 번거롭고 논란이 있던 DOM(Document Object Model)을 더욱 쉽게 제어할 수 있게 되었고 크로스 브라우징 이슈도 어느 정도 해결되었다.

### 2.3.3 V8 자바스크립트 엔진

**2008년 :** 더욱 빠르게 동작하는 자바스크립트 엔진의 필요성이 대두되었다. 구글의 V8 자바스크립트 엔진은 이러한 요구에 부합하는 빠른 성능을 보여주었다.

이 엔진으로 촉발된 자바스크립트의 발전으로 과거 웹 서버에서 수행되던 로직들이 대거 클라이언트(브라우저)로 이동했고, 이는 **웹 애플리케이션 개발에서 프론트엔드 영역이 주목받는 계기**로 작용했다.

### 2.3.4 Node.js

**2009년 :** 라이언 달이 발표현 Node.js는 구글 V8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임 환경(runtime environment)이다.

Node.js는 브라우저의 자바스크립트 엔진에서만 동작하던 자바스크립트를 브라우저 이외의 환경에서도 동작할 수 있도록 자바스크립트 엔진을 브라우저에서 독립시킨 자바스크립트 실행 환경이다.

Node.js는 비동기 I/O를 지원하며 단일 스레드(single thread) 이벤트 루프 기반으로 동작함으로써 요청(request) 처리 성능이 좋다.

Node.js의 등장으로 자바스크립트는 브라우저를 벗어나 서버 사이드 애플리케이션 개발에서도 사용할 수 있는 범용 프로그래밍 언어가 되었다. 브라우저에서만 동작하는 반쪽짜리 프로그래밍 언어 취급을 받던 자바스크립트는 이제 **프론트엔트 영역은 물론 백엔드 영역까지 아우르는 웹 프로그래밍 언어의 표준**으로 자리 잡고 있다.

### 2.3.5 SPA 프레임워크
모던 웹 애플리케이션은 데스크톱 애플리케이션과 비교해도 손색없는 성능과 사용자 경험을 제공하는 것이 필수가 되었고, 더불어 개발 규모와 복잡도가 상승했다.

CBD(Component based development) 방법론을 기반으로 하는 SPA(Single Page Application)가 대중화되면서 Angular, React, Vue.js, Svelte 등 다양한 SPA 프레임워크/라이브러리 또한 많은 사용층을 확보하고 있다.

## 2.4 자바스크립트와 ECMAScript
ECMAScript는 자바스크립트의 표준 사양인 **ECMA-262**를 말한다.

자바스크립트는 일반적으로 프로그래밍 언어로서 기본 뼈대(core)를 이루는 ECMASCript와 브라우저가 별도 지원하는 **클라이언트 사이드 Web API**, 즉 DOM, BOM, Canvas, XMLHttpRequest, fetch, requestAnimationFrame, SVG, Web Storage, Web Component, Web Worker 등을 아우르는 개념이다.

## 2.5 자바스크립트의 특징
자바스크립트는 HTML, CSS와 함께 웹을 구성하는 요소 중 하나로 **웹 브라우저에서 동작하는 유일한 프로그래밍 언어**다.

자바스크립트는 개발자가 별도의 컴파일 작업을 수행하지 않는 **인터프리터 언어**(interpreter language)다.

**인터프리터 :** 소스코드를 즉시 실행하고 컴파일러는 빠르게 동작하는 머신 코드를 생성하고 최적화한다.

자바스크립트는 명령형(imperative), 함수형(functional), 프로토타입 기반(prototype-based) 객체지향 프로그래밍을 지원하는 **멀티 패러다임 프로그래밍 언어다**.

## 2.6 ES6 브라우저 지원 현황
Node.js는 v4부터 ES6를 지원하기 시작했다.

따라서, 브라우저에서 아직 지원하지 않는 최신 기능을 사용하거나 ES6를 대부분 지원하지 않는 인터넷 익스플로러나 구형 브라우저를 고려해야 하는 상황이라면 바벨(Bebel)과 같은 트랜스파일러를 사용해 ES6 이상의 사양으로 구현한 소스코드를 ES5 이하의 사양으로 다운그레이드할 필요가 있다.

---

# 03장. 자바스크립트 개발 환경와 실행 방법
## 3.1 자바스크립트 실행 환경
모든 브라우저와 Node.js는 자바스크립트를 해석하고 실행할 수 있는 자바스크립트 엔진을 내장하고 있다. 따라서 자바스크립트는 브라우저 환경 또는 Node.js 환경에서 실행할 수 있다.

브라우저는 HTML, CSS, 자바스크립트를 실행해 웹페이지를 브라우저 환경에 렌더링하는 것이 주된 목적이지만 Node.js는 브라우저 외부에서 자바스크립트 실행 환경을 제공하는 것이 주된 목적이다.

## 3.2 웹 브라우저
크롬 브라우저의 V8 자바스크립트 엔진은 Node.js에서도 사용하고 있다.
### 3.2.1 개발자 도구
### 3.2.2 콘솔
### 3.2.3 브라우저에서 자바스크립트 실행
### 3.2.4 디버깅

## 3.3 Node.js
브라우저에서 동작하는 간단한 웹 애플리케이션은 브라우저만으로도 개발할 수 있다. 하지만, 프로젝트 규모가 커짐에 따라 React, Angular, Lodash 같은 프레임워크 또는 라이브러리를 도입하거나 Babel, Webpack, ESLint 등 여러 가지 도구를 사용할 필요가 있다. 이때 Node.js와 npm이 필요하다.

### 3.3.1 Node.js와 npm 소개
npm(node package manager)은 자바스크립트 패키지 매니저다. Node.js에서 사용할 수 있는 모듈들을 패키지화해서 모아둔 저장소 역할과 패키지 설치 및 관리를 위한 CLI(Command line interface)를 제공한다.

### 3.3.2 Node.js 설치
### 3.3.3 Node.js REPL
Node.js가 제공하는 REPL(Read Eval Print Loop)을 사용하면 간단한 자바스크립트 코드를 실행해 결과를 확인해 볼 수 있다.
> $ node
자바스크립트 코드를 실행해 볼 수 있다.

> $ node index.js
자바스크립트 파일을 실행하려면 node 명령어 뒤에 파일 이름을 입력한다. 파일 확장자 .js는 생략해도 된다.


## 3.4 비주얼 스튜디오 코드
### 3.4.1 비주얼 스튜디오 코드 설치
### 3.4.2 내장 터미널
### 3.4.3 Code Runner 확장 플러그인
### 3.4.4 Live Server 확장 플러그인

---

# 04장. 변수
## 4.1 변수란 무엇인가? 왜 필요한가?

> 변수(variable)는 하나의 값을 저장하기 위해 확보한 메모리 공간 자체 또는 그 메모리 공간을 식별하기 위해 붙인 이름을 말한다. 값의 위치를 가리키는 상징적인 이름이다.

변수는 프로그래밍 언어에서 데이터를 관리하기 위한 핵심 개념이다.

메모리(memory)는 데이터를 저장할 수 있는 메모리 셀(memory cell)의 집합체다. 메모리 셀 하나의 크기는 1바이트(8비트)이며, 컴퓨터는 메모리 셀의 크기, 즉 1바이트 단위로 데이터를 저장(write)하거나 읽어(read)들인다.

변수에 값을 저장하는 것을 할당(assignment - 대입, 저장)이라 하고, 변수에 저장된 값을 읽어 들이는 것을 참조(reference)라 한다.

## 4.2 식별자
**변수 이름을 식별자(identifier)** 라고도 한다. 식별자는 어떤 값을 구별해서 식별할 수 있는 고유한 이름을 말한다.

식별자는 값이 아니라 메모리 주소를 기억하고 있다. 즉, 식별자는 메모리 주소에 붙인 이름이라고 할 수 있다.

변수, 함수, 클래스 등의 이름은 모두 식별자다. 선언(declaration)에 의해 자바스크립트 엔진에 식별자의 존재를 알린다.

## 4.3 변수 선언
**변수 선언(variable declaration)** 이란 변수를 생성하는 것을 말한다. 조금 더 자세히 말하면, **값을 저장하기 위한 메모리 공간을 확보(allocate)** 하고 **함수 이름과 확보된 메모리 공간의 주소를 연결(name binding)** 해서 **값을 저장할 수 있게 준비하는 것** 이다.

> **Q. 변수 이름은 어디에 등록되는가?**
변수 이름을 비롯한 모든 식별자는 **실행 컨텍스트에 등록** 된다. 자바스크립트 엔진은 실행 컨텍스트를 통해 식별자와 스코프를 관리한다.

**초기화(initialization) :** 변수가 선언된 이후 최초로 값을 할당하는 것
만약 초기화 단계를 거치지 않으면, 확보된 메모리 공간에는 이전에 다른 애플리케이션이 사용했던 값이 남아 있을 수 있다. 이러한 값을 쓰레기 값(garbage value)이라 한다.

변수뿐만 아니라 모든 식별자(함수, 클래스 등)를 사용하려면, 반드시 선언이 필요하다. 만약 선언하지 않은 식별자에 접근하면 Reference Error(참조 에러)가 발생한다.

## 4.4 변수 선언의 실행 시점과 변수 호이스팅
```javascript
console.log(score); // undefined
var score; // 변수 선언문
```
> **Q. 위의 코드는 참조 에러가 발생할 것 처럼 보이지만, undefined가 출력된다.**
변수 선언이 소스코드가 한 줄씩 순차적으로 실행되는 시점, 즉 런타임(runtime)이 아니라 그 이전 단계에서 먼저 실행되기 때문이다.

1. **평가과정 :** 소스코드 실행을 위한 준비 단계이자 변수 선언을 포함한 모든 선언문을 소스코드에서 찾아내 먼저 실행하는 단계
2. **런타임 :** 소스코드 한 줄씩 순차적 실행되는 시점

**변수 호이스팅(variable hoisting) :** 변수 선언문이 코드의 선두로 끌어 올려진 것처럼 동작하는 자바스크립트의 고유의 특징

## 4.5 값의 할당
변수 선언과 값의 할당의 실행 시점이 다르다.

1. **변수 선언 :** 소스코드가 순차적으로 실행되는 시점인 런타임 이전에 먼저 실행
2. **값의 할당 :** 소스코드가 순차적으로 실행되는 시점인 런타임에 실행

## 4.6 값의 재할당
**재할당 :** 이미 값이 할당되어 있는 변수에 새로운 값을 또다시 할당하는 것. 현재 변수에 저장된 값을 버리고 새로운 값을 저장하는 것.
> 기존 값이 할당된 메모리 공간에 새로운 값을 저장하는 것이 아니라, 새로운 메모리 공간을 확보하고 그곳에 할당 값을 저장한다!

**상수(constant) :** 값을 재할당할 수 없어서 변수에 저장된 값을 변경할 수 없다면, 변수가 아니라 상수라 한다. 즉, 상수는 단 한 번만 할당할 수 있는 변수다.

## 4.7 식별자 네이밍 규칙

**식별자(identifier) 네이밍 규칙 :** 특수문자를 제외한 문자, 숫자, 언더스코어(_), 달러 기호($)를 포함할 수 있다. 단, 숫자로 시작하는 것은 허용하지 않는다.

**카멜 케이스(camelCase) :** 변수나 함수의 이름
**파스칼 케이스(PascalCase) :** 생성자 함수, 클래스의 이름

---
# 05장. 표현식과 문
> 개념을 이해한다는 것은 바로 **용어를 정확히 이해하고 설명할 수 있다는 것** 이다.

## 5.1 값

**값(value) :** 식(표현식 expression)이 평가(evaluate)되어 생성된 결과

## 5.2 리터럴
> 리터럴은 평가되어 값을 생성한다.
자바스크립트 엔진은 코드가 실행되는 시점인 런타임(runtime)에 리터럴을 평가해 값을 생성한다.

**리터럴(literal) :** 사람이 이해할 수 있는 문자 또는 약속된 기호를 사용해 값을 생성하는 표기법(notaion)을 말한다.

## 5.3 표현식
**표현식(expression) :** 값으로 평가될 수 있는 문(statement)이다. 즉, 표현식이 평가되면 새로운 값을 생성하거나 기존 값을 참조한다. 즉, 값으로 평가될 수 있는 문은 모두 표현식이다.

## 5.4 문

**"문(statement)"** 과 **"표현식(expression)"** 을 구별하고 해석할 수 있다면 자바스크립트 엔진의 입장에서 코드를 읽을 수 있고 실행 결과를 예측하는 데 도움이 된다.

**문(statement) :** 프로그램을 구성하는 기본 단위이자 최소 실행 단위다. 문의 집합으로 이뤄진 것이 바로 프로그램이며, 문을 작성하고 순서에 맞게 나열하는 것이 프로그래밍이다. 명령문이라고도 부른다.

**토큰(token) :** 문법적인 의미를 가지며, 문법적으로 더 이상 나눌 수 없는 코드의 기본 요소를 의미한다. 문은 여러 토큰으로 구성된다.

## 5.5 세미콜론과 세미콜론 자동 삽입 기능
**세미콜론(;) :** 문의 종료 의미. 단, 0개 이상의 문을 중괄호로 묶은 코드 블록({ ... }) 뒤에는 세미콜론을 붙이지 않는다. (자체 종결성 - self closing)

**세미콜론 자동 삽입 기능(ASI) :** 자바스크립트 엔진이 소스코드를 해석할 때 문의 끝이라고 예측되는 지점에 세미콜론을 자동으로 붙여주는 기능

> **TC39 :** ECMAScript 기술 위원회 -> 세미콜론 사용 권장하는 분위기

## 5.6 표현식인 문과 표현식이 아닌 문
> 문과 표현식이 비슷해서 구별하기 어렵다고 느낄 수 있다.

**변수에 할당** 이 가능하다면, 표현식인 문이고 아니면, 표현식이 아닌 문이다.

---

# 06장. 데이터 타입
- **원시 타입(primitive type)**
  - 숫자(number) 타입
  - 문자열(string) 타입
  - 불리언(boolean) 타입
  - undefined 타입
  - null 타입
  - 심벌(symbol) 타입
  

- **객체 타입(object/reference type)** : 객체, 함수, 배열 등

## 6.1 숫자 타입
C나 자바의 경우, 정수(소수점 이하가 없는 숫자)와 실수(소수점 이하가 있는 숫자)를 구분해서 int, long, float, double 등과 같은 다양한 숫자 타입을 제공한다.

하지만, **자바스크립트는 독특하게 하나의 숫자(number) 타입만 존재한다.**

## 6.2 문자열 타입
문자열은 0개 이상의 16비트 유니코드 문자(UTF-16)의 집합으로 전 세계 대부분의 문자를 표현할 수 있다.

## 6.3 템플릿 리터럴
ES6부터 템플릿 리터럴(template literal)이라고 하는 새로운 문자열 표기법이 도입되었다. **런타임에 일반 문자열로 변환** 되어 처리된다.

### 6.3.1 멀티라인 문자열
일반 문자열 내에서는 줄바꿈(개행)이 허용되지 않는다. 백슬래시('\')로 시작하는 이스케이프 시퀀스(escape sequence)를 사용해야 된다.

템플릿 리너털 내에서는 이스케이프 시퀀스를 사용하지 않고도 줄바꿈이 허용되며, 모든 공백도 있는 그대로 적용된다.

### 6.3.2 표현식 삽입
일반 문자열은 문자열 연산자 '+'를 사용해 연결할 수 있다.

템플릿 리터널 내에서는 **${ }** 을 사용한 표현식 삽입(expression interpolation)으로 간단히 문자열을 삽입할 수 있다.
```javascript
console.log(`1 + 2 = ${1 + 2}`); // 1 + 2 = 3
```

## 6.4 불리언 타입
논리적 참, 거짓을 나타내는 true와 false뿐이다.


