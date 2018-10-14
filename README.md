# begin-redux

리덕스 시작하기 튜토리얼 전용 템플릿

이 프로젝트는 총 6가지의 Branch 로 나뉘어져있습니다:

- [template](https://github.com/vega2k/begin-redux-template): 실습을 빠르게 진행하기 위한 템플릿
- [01]: Counter (기본)
- [02]: Counter (코드 정리)
- [03]: Todo 리스트 (기본)
- [04]: Todo 리스트 (Immutable Record 사용)
- [05]: ActionCreator 미리 bind하기
- [06]: immer.js 사용해보기
- [07]: MobX 로 구현해보기
- [08]: MobX 로 구현해보기 (Store 분리)

## 템플릿에 이미 이뤄진 작업:

### 0. 절대경로에서 파일을 불러 올 수 있도록 설정

- .env: NODE_PATH 설정
- jsconfig.json: 에디터 설정

### 1. 패키지 설치
```bash
$ yarn add redux react-redux redux-actions immutable
```

### 2. 불필요한 파일 제거
- App.js
- App.css
- App.test.js
- logo.svg

### 3. 주요 컴포넌트 생성 및 루트 컴포넌트 생성

- components/
  - App.js
  - AppTemplate.js
  - Counter.js
  - Todos.js
- containers/
  - CounterContainer.js
  - TodosContainer.js
- Root.js

### 4. 리덕스 관련 코드를 작성 할 파일 생성
- store
  - modules
    - counter.js
    - todo.js
    - index.js
  - configure.js
  - index.js
  - actionCreators.js