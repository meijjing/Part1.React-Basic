# Part1.React-Basic

Created with CodeSandbox

## 02. DOM 다루기 Element 생성하기

- CodeSandBox - 온라인 코드 에디터
- Vailla js Dom - W3Schools / createElement
- CDN - unpkg
- React / React-dom - element생성 / appendChild

## 03. JSX과 Babel , JSX 다루기

- JSX - React.createElement 표현식
- Babel - JavaScript Compiler
- JSX 다루기 - spread 연산자

## 04. 멀티 Element 생성하기

- Fragment - React.Fragment 또는 <></>

## 05. Element 찍어내기

- Functino - 재사용 가능한 Element
- Custom Element - Upper case
- Children - 개수 무제한

## 06. JS와 JSX 섞어쓰기

- Interpolation - 이미 HTML에서도 쓰고 있었다.

## 07. 중간 복습1

- console.log(element)

## 08. 리액트의 리랜더링 알아보기

- 바닐라 JS - 변경으로 인해 Element를 다시 그림
- React - 변경된 부분만 다시 그림

## 09. 리액트의 리랜더링 알아보기 2

1. [리액트 엘리먼트 랜더링](https://ko.reactjs.org/docs/rendering-elements.html)

- 리액트 element는 **불변객체(immutable)**이다.
- 불변객체란? **변하지 않는** 객체
- 우리는 그저 ReactDOM.render(element, rootElement); 로 **전달**할뿐...
- 변경 판단 및 반영은 리액트가 알아서 한다.

2. [리액트 재조정](https://ko.reactjs.org/docs/reconciliation.html)

- element 타입이 바뀌면? 이전 엘리먼트는 버리고 새로그린다.
- element 타입이 같다면? (key를 먼저 비교하고) props를 비교해서 변경사항을 반영한다.

> - 리액드 엘리먼트 - 불변객체
> - 변경 사항 반영 - 리액트에게 일임
> - 리액트의 비교 - Reconciliation
> - Virtual Dom - 비교시 활용

## 10. 이벤트 핸들러 써보기

- 바닐라 JS

  - addEventListener
  - on{event} onclick onmouseout onfocus onblur...

- 리액트 (카멜케이스)
  - on{Event} onClick onMouseOut onFocus onBlur...

> 카멜 케이스 onClick
> 파스칼 케이스 OnClick
> 케밥 케이스 on-click
> 스네이크 케이스 on_click

## 11. 이벤트 핸들러 써보기 2 (여러가지 시도해보기)

- 간단한 검색창 만들기
- Object.assign - 객체 내용 복사 (바뀐부분만 덮어쓰기)
- 전역 변수 변경 - ReactDOM.render

## 13. 컴포넌트 상태 다루기 (useState)

- DOM - 논리트리
- 컴포넌트 - 엘리먼트의 집합
- 엘리먼트 - 요소
- **useState - 상태값을 관리해주는 훅**

## 14. 컴포넌트 사이드이펙트 다루기 (useEffect)

- 사이드이펙트 = 부작용 의도하지 않은 효과 vs **부수 효과**
- useState - lazy initialize
- useEffect - dependency array
- React.useEffect(() => {함수}, [effect를 이루어주고 싶은 대상, 생략가능])

## 15. 커스텀 훅 만들기 use{Name}

- 찍어내기/반복 => 함수화
- useState/useEffect 등 훅 반복 => 커스텀 훅

## 16. Hookflow 이해하기 (App - Child)

- 훅의 호출 타이밍을 알자
- hook flow - hook들의 호출 타이밍
- useState - setState시 prev값이 주입된다.

## 17. Hookflow 이해하기 2 (App - Child)

- useEffect - render가 끝난 뒤 실행 (자식요소 먼저 실행)
- update시 - useEffect clean up실행 후, useEffect 실행
- dependency array - 전달받은 값의 변화 있는 경우에만
