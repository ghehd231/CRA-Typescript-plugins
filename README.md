## 참고

[참고블로그 링크](https://velog.io/@junghyeonsu/React-create-react-app-Typescript-%EC%B4%88%EA%B8%B0-%EC%84%B8%ED%8C%85-%EC%99%84%EB%B2%BD-%EC%A0%95%EB%A6%AC)

## CRA

### 설치

```
$npx create-react-app "이름" —-template typescript
```

기존 cra에 typescript 추가

[React 공홈 링크](https://github.com/Microsoft/TypeScript-React-Starter#typescript-react-starter)

`create-react-app my-app --scripts-version=react-scripts-ts`

<br/>

## eslint, prettier

### 설치

```
npm install -D eslint
```

후에 `npx eslint --init ` 질문에 y/n 은 다 y

추가 플러그인 (airbnb)

```
npm i -D eslint-config-airbnb-base # 리액트 관련 규칙 X
npm i -D eslint-config-airbnb # 리액트 관련 규칙 O

npm i -D eslint-plugin-react eslint-plugin-react-hooks
npm i -D eslint-plugin-jsx-a11y eslint-plugin-import eslint-plugin-prettier eslint-config-prettier
```

- eslint-plugin-import : ES6의 import, export 구문을 지원, 필수 플러그인
- eslint-plugin-react : React 규칙이 들어있는 플러그인
- eslint-plugin-react-hooks : React Hooks 규칙이 들어있는 플러그인
- eslint-plugin-jsx-a11y : JSX요소의 접근성 규칙에 대한 정적 검사 플러그인

## prettier

### 설치

` $npm install -D prettier`

.prettierrc 생성 [https://prettier.io/docs/en/options.html]

```
{
  "singleQuote": true,
  "semi": true,
  "useTabs": false,
  "tabWidth": 2,
  "trailingComma": "all",
  "printWidth": 80,
  "arrowParens": "always",
  "orderedImports": true,
  "bracketSpacing": true,
  "jsxBracketSameLine": false
}
```

오류 났을떄 추가로 설치

`npm i -D prettier eslint-config-prettier eslint-plugin-prettier`
