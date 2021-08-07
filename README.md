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
