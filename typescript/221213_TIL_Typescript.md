# TypeScript

## TypeScript란 무엇인가?

> Typed JavaScript at any Scale

- JavaScript 에 Type을 적용시킴(type을 추가해서 javascript를 확장시킴)
- runtime이전에 에러를 감지해서 수정할 수 있다(시간절약 가능)
- 모든 javascript실행환경(e.i node), 모든 browser, 모든 OS에서 동작하는 오픈소스 라이브러리
- 타입스크립트는 `Programming Language 언어`
- 타입스크립트는 `Compiled Language`입니다
  - 전통적인 `Compiled Language` (e.i C++, Java …)와는 다른 점이 많다.
  - 그래서, `Transpile` 이라는 용어를 사용하기도 한다.
- 자바스크립트는 `Interpreted Language` 이다.

![typescript_process.png](data:image/png;base64,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)

### Compiled 언어와 Interpreted 언어의 차이

| Compiled 언어                                             | Interpreted 언어                    |
| --------------------------------------------------------- | ----------------------------------- |
| 컴파일이 필요함                                           | 컴파일이 필요하지 않음              |
| 컴파일러가 필요함                                         | 컴파일러가 필요하지 않음            |
| 컴파일하는 시점이 있음 ⇒ 컴파일하는 시점에 에러 수정 가능 | 컴파일하는 시점이 없음              |
| 컴파일된 결과물을 실행                                    | 코드를 실행하는 시점(런타임)에 실행 |

## TypeScript 설치 및 사용

### 자바스크립트 실행 환경 설치

<aside>
💡 자바스크립트 실행 환경

</aside>

| node.js                                                                                                                               | browser                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Chrome`s V8 JavaScript Engine을 사용하여, 자바스크립트를 해석하고 OS 레벨에서의 API를 제공한느 서버사이드 용 자바스크립트 런타임 환경 | HTML을 동적으로 만들기 위해 브라우저에서 자바스크립트를 해석하고, DOM을 제어할 수 있도록 하는 자바스크립트 런타임 환경 |

- node.js 설치
  - [https://nodejs.org](https://nodejs.org) 접속해서 다운로드
    - LTS : Long Term Support, 안정적인 버전
    - Current : 최신 버전
  - node.js version manager
    - nvm
      - [https://gitbub.com/creationix/nvm](https://gitbub.com/creationix/nvm)
      - [https://github.com/corebutler/nvm-windows](https://github.com/corebutler/nvm-windows)
    - n
      - [https://github.com/tj/n](https://github.com/tj/n)
- browser 설치
  - chrome을 많이 사용하고 개발자에게 도움이 되는 도구를 제공해주기 때문에 chrome 사용을 권장

### 타입스크립트 컴파일러 설치

- npm 으로 설치 (권장)
  - `npm i typescript -g`
    - global 옵션이 없을 경우 보통은 현재 프로젝트에`node_modules`폴더가 생성되고 설치되며, 타입스크립트를 실행할 수 있도록 `/.bin/tsc` 폴더가 생성된다.
      (`node_modules/.bin/tsc`)
    - `npm i typescript -D` 로 설치할 경우 devDependencies에 추가되서 개발용으로 사용하는 라이브러리라는 것을 명시적으로 표현할 수 있다.
  - `tsc source.ts` 와 같이 tsc를 이용해서 cli로 typescript를 실행할 수 있다. (typescript → javascript)
- Visual Studio plugin 으로 설치
  - Visual Studio 2017 / 2015 Update 3 이후로는 기본으로 설치되어있지만, 만약에 없을 경우에는 설치하면 된다.

### TSC, tsconfig

- 현재 프로젝트 cli에 `tsc` 만 입력할 때, 현재 프로젝트의 타입스크립트 파일을 어떻게 컴파일할지에 대한 설정이 없을 경우 실행되지 않는다.
- cli에 `tsc --init` 을 입력하면 자동으로 `tsconfig.json`이라는 default 설정파일을 생성해준다. 보통은 프로젝트 root 디렉토리에 생성한다.
- tsconfig.json이 있는 디렉토리에서 tsc를 실행할 경우 tsconfig.json의 설정에 따라 작업된다.
- watch 모드 : `tsc -w` 변경사항이 실시간으로 반영된다.
- typescript를 전역이 아니라 현재 프로젝트에 설치하였을 경우 cli에서 tsc를 실행하는 방법

```jsx
$ ls -al node_modules/.bin

...

tsc -> ../typescript/bin/tsc
tsserver -> ../typescript/bin/tsserver

...
```

위와 같이 확인 되기 때문에

1. node_modules/.bin/tsc
2. node_modules/typescript/bin/tsc

의 경로로 tsc를 실행할 수 있다.

⇒ `npx tsc` 로 축약해서 사용할 수 있다.

```json
{
	...
	"scripts": {
		"build" : "tsc"
	}
}
```

위와 같이 package.json에서 script를 추가하면 `npm run build` 로 tsc를 실행할 수 있다.

## Visual Studio Code 설치 및 설정

- TypeScript Compiler
  - VS Code에 컴파일러가 내장되어 있다.
  - 내장된 컴파일러 버전은 VS Code가 업데이트 되면서 올라간다.
    - 컴파일러 버전과 VS Code의 버전은 상관 관계가 있다.
  - 내장된 컴파일러를 선택할 수 있고, 직접 설치한 컴파일러를 선택할 수도 있다.

<aside>
💡 ctrl + shift + p ⇒ shell Command: Install ’code’ command in PATH 를 선택할 경우 cli에서 code command를 통해 vscode를 열 수 있다.

</aside>

## Type Annotation

- 타입스크립트가 가진 고유한 기능
- type이 code상에서 드러남

```tsx
// ./test.ts
// 값을 할당하지 않고 선언할 경우 타입스크립트는 변수 a를 any타입이라고 해석한다.
let a;

// type annotation : 타입을 명시
let b: string;
// b = 39; 에러(변수 b는 string타입이라고 선언되었지만, 변수 b에 number 타입의 값을 할당하려고 하기 때문에)

function hello(b: number) {}

hello(39); // ok
// hello('Mark'); 에러
```
