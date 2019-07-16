# React Interview Questions & Answers

### Contributor

<a href="https://github.com/SeonHyungJo" target="_blank" rel="nofollow">
	<img src="https://avatars2.githubusercontent.com/u/24274424?s=60&v=4">
</a>
<a href="https://github.com/BKJang" target="_blank" rel="nofollow">
	<img src="https://avatars2.githubusercontent.com/u/24209005?s=60&v=4">
</a>

> * :clipboard: 본 문서는 [sudheerj](https://github.com/sudheerj)의 [reactjs-interview-questions](https://github.com/sudheerj/reactjs-interview-questions)의 번역본입니다.
> * :star: 이 프로젝트가 마음에 드셨다면 **STAR**를 눌러주세요.
> * :heavy_check_mark: 풀 리퀘스트는 언제든 환영입니다.
> * :clap: [vuejs-interview-questions-korean](https://github.com/sudheerj/vuejs-interview-questions-korean)를 참고를 해서 작성하였습니다.

### Table of Contents

| No. | Questions |
| --- | --------- |
|   | **Core React** |
|1  | [React란 무엇인가?](#React란-무엇인가) |
|2  | [React의 주요 특징은?](#React의-주요-특징은) |
|3  | [JSX란 무엇인가?](#JSX란-무엇인가) |
|4  | [Element와 Component의 차이점은?](#element와-component의-차이점은) |
|5  | [React에서 components는 어떻게 만드나?](#React에서-components는-어떻게-만드나) |
|6  | [언제 Function Component 대신에 Class Component를 사용하나?](#언제-Function-Component-대신에-Class-Component를-사용하나) |
|7  | [Pure Components란 무엇인가?](#Pure-Components란-무엇인가) |
|8  | [React에서 state는 무엇인가?](#React에서-state는-무엇인가) |
|9  | [React에서 props는 무엇인가?](#React에서-props는-무엇인가) |
|10 | [state와 prop의 차이점은?](#state와-prop의-차이점은) |
|11 | [왜 state를 직접 update하면 안되나?](#왜-state를-직접-update하면-안되나) |
|12 | [setState()의 argument로 callback 함수를 사용하는 이유는?](#setState()의-argument로-callback-함수를-사용하는-이유는) |
|13 | [HTML과 React의 event handling의 차이점은?](#HTML과-React의-event-handling의-차이점은) |
|14 | [어떻게 JSX 콜백에서 메서드와 이벤트 핸들러를 바인드하나?](#어떻게-JSX-콜백에서-메서드와-이벤트-핸들러를-바인드하나) |
|15 | [어떻게 이벤트 핸들러나 콜백에 매개 변수를 전달하나?](#어떻게-이벤트-핸들러나-콜백에-매개-변수를-전달하나) |
|16 | [React에 SyntheticEvent란 무엇인가?](#React에-SyntheticEvent란-무엇인가) |
|17 | [인라인 조건 표현식이란?](#인라인-조건-표현식이란) |
|18 | ["key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?](#key-props는-무엇이며-elements의-배열에서-사용하면-이점이-무엇인가) |
|19 | [refs는 어떻게 사용되는가?](#refs는-어떻게-사용되는가) |
|20 | [refs는 어떻게 생성하는가?](#refs는-어떻게-생성하는가)
|21 | [forward refs는 무엇인가?](#forward-refs는-무엇인가) |
|22 | [callback refs 및 findDOMNode()에서 선호되는 옵션은?](#callback-refs-및-findDOMNode()에서-선호되는-옵션은) |
|23 | [String Refs가 왜 legacy인가?](#String-Refs가-왜-legacy인가) |
|24 | [Virtual DOM이란?](#Virtual-DOM이란) 
|25 | [Virtual DOM은 어떻게 작동하나?](#Virtual-DOM은-어떻게-작동하나) |
|26 | [Shadow DOM과 Virtual DOM의 차이점](#Shadow-DOM과-Virtual-DOM의-차이점) |
|27 | [React Fiber란?](#React-Fiber란) |
|28 | [React Fiber의 주요 목표는?](#React-Fiber의-주요-목표는) |
|29 | [controlled components란?](#controlled-components란) |
|30 | [uncontrolled components란?](#uncontrolled-components란) |
|31 | [createElement와 cloneElement의 차이점은?](#createElement와-cloneElement의-차이점은?) |
|32 | [React에서 Lifting State Up란?](#React에서-Lifting-State-Up란) |
|33 | [컴포넌트 라이프 사이클의 다른 단계들은?](#컴포넌트-라이프-사이클의-다른-단계들은?) |
|34 | [React의 라이프 사이클 메서드에는 무엇이 있나?](#React의-라이프-사이클-메서드에는-무엇이-있나?) |
|35 | [고차(Higher-Order) 컴포넌트란?](#고차(Higher-Order)-컴포넌트란?) |
|36 | [HOC 컴포넌트를 사용해서 props 프록시를 만드는 방법은?](#HOC-컴포넌트를-사용해서-props-프록시를-만드는-방법은) |
|37 | [context란?](#context란) |
|38 | [children prop이란?](#children-prop이란) |
|39 | [React에서 주석을 어떻게 다는가?](#React에서-주석을-어떻게-다는가) |
|40 | [props argument가 있는 생성자에서 super를 사용하는 목적은 무엇입니까?](#props-argument가-있는-생성자에서-super를-사용하는-목적은-무엇입니까) |
|41 | [조정(reconciliation)이란?](#조정(reconciliation)이란) |
|42 | [state의 키 이름을 동적으로 설정하는 방법은?](#state의-키-이름을-동적으로-설정하는-방법은?) |
|43 | [컴포넌트가 렌더링 될 때마다 호출되는 함수에 대한 실수는 무엇일까?](#컴포넌트가-렌더링-될-때마다-호출되는-함수에-대한-실수는-무엇일까) |
|44 | [왜 컴포넌트 이름은 대문자로 해야 하나?](#왜-컴포넌트-이름은-대문자로-해야-하나) |
|45 | [React는 왜 class가 아닌 className 속성을 사용하나?](#React는-왜-class가-아닌-className-속성을-사용하나?) |
|46 | [fragments란?](#fragments란) |
|47 | [div보다 fragments가 더 우수한 이유는?](#div보다-fragments가-더-우수한-이유는) |
|48 | [React의 portals이란?](#React의-portals이란) |
|49 | [stateless 컴포넌트란?](#stateless-컴포넌트란) |
|50 | [stateful 컴포넌트란?](#stateful-컴포넌트란) |
|51 | [React에서 props 유효성 검사를 적용하는 방법은?](#React에서-props-유효성-검사를-적용하는-방법은) |
|52 | [React의 장점은?](#React의-장점은) |
|53 | [React의 한계는?](#React의-한계는) |
|54 | [React v16에서 error boundaries란 무엇인가?](#React-v16에서-error-boundaries란-무엇인가) 
|55 | [React v15에서는 어떻게 error boundaries 조작하나?](#React-v15에서는-어떻게-error-boundaries-조작하나) |
|56 | [정적 타입 검사에 권장되는 방법은?](#정적-타입-검사에-권장되는-방법은) |
|57 | [react-dom 패키지 사용법은?](#react-dom-패키지-사용법은) |
|58 | [react-dom의 render 메서드란?](#react-dom의-render-메서드란) |
|59 | [ReactDOMServer란?](#ReactDOMServer란) |
|60 | [React에서 innerHTML를 사용하는 방법?](#React에서-innerHTML를-사용하는-방법) |
|61 | [React에서 스타일을 사용하는 방법?](#React에서-스타일을-사용하는-방법) |
|62 | [React에서 이벤트가 어떻게 다른가?](#React에서-이벤트가-어떻게-다른가) |
|63 | [생성자에서 setState()를 사용하면 어떻게 되나?](#생성자에서-setState()를-사용하면-어떻게-되나) |
|64 | [키로 인덱스를 사용하면?](#키로-인덱스를-사용하면) |
|65 | [componentWillMount() 메서드에서 setState()를 사용하는 것은 좋은가?](#componentWillMount()-메서드에서-setState()를-사용하는-것은-좋은가) |
|66 | [초기 state에 props를 사용하면 어떻게 되나?](#초기-state에-props를-사용하면-어떻게-되나) |
|67 | [컴포넌트를 조건부로 렌더링하는 방법?](#컴포넌트를-조건부로-렌더링하는-방법)
|68 | [DOM 엘리먼트에서 spread props를 조심해야하는 이유는?](#DOM-엘리먼트에서-spread-props를-조심해야하는-이유는) 
|69 | [React에서 데코레이터를 사용하는 방법?](#React에서-데코레이터를-사용하는-방법) |
|70 | [컴포넌트를 어떻게 메모하나?](#컴포넌트를-어떻게-메모하나) |
|71 | [Server Side Rendering 또는 SSR 구현방법?](#Server-Side-Rendering-또는-SSR-구현방법) |
|72 | [React에서 production 모드를 사용하는 방법?](#React에서-production-모드를-사용하는-방법) |
|73 | [CRA란 무엇이며 장점은?](#CRA란-무엇이며-장점은) |
|74 | [마운팅의 라이프 사이클 메서드 순서는?](#마운팅의-라이프-사이클-메서드-순서는) |
|75 | [What are the lifecycle methods going to be deprecated in React v16?](#what-are-the-lifecycle-methods-going-to-be-deprecated-in-react-v16) |
|76 | [getDerivedStateFromProps() 라이프 사이클 메서드의 사용 목적은?](#getDerivedStateFromProps()-라이프-사이클-메서드의-사용-목적은) |
|77 | [getSnapshotBeforeUpdate() 라이프 사이클 메서드의 사용 목적은?](#getSnapshotBeforeUpdate()-라이프-사이클-메서드의-사용-목적은) |
|78 | [Hooks는 렌더링 props와 고차원 컴포넌트를 대체한다?](#Hooks는-렌더링-props와-고차원-컴포넌트를-대체한다) |
|79 | [컴포넌트를 명명하는데 권장되는 방법은?](#컴포넌트를-명명하는데-권장되는-방법은) |
|80 | [컴포넌트 클래스에서 권장되는 메서드 순서는?](#컴포넌트-클래스에서-권장되는-메서드-순서는) |
|81 | [스위칭 컴포넌트란?](#스위칭-컴포넌트란) |
|82 | [왜 setState()에 함수를 전달해야 하나?](#왜-setState()에-함수를-전달해야-하나) |
|83 | [React의 strict mode란?](#React의-strict-mode란) |
|84 | [React Mixins이란?](#React-Mixins이란) |
|85 | [왜 isMounted()가 안티 패턴이며 적절한 해결책은?](#왜-isMounted()가-안티-패턴이며-적절한-해결책은) |
|86 | [React에서 지원되는 Pointer Events는?](#React에서-지원되는-Pointer-Events는) |
|87 | [왜 컴포넌트의 이름은 대문자로 시작하나?](#왜-컴포넌트의-이름은-대문자로-시작하나) |
|88 | [React v16에서 사용자 정의 DOM 속성을 지원하나?](#React-v16에서-사용자-정의-DOM-속성을-지원하나) |
|89 | [constructor과 getInitialState의 차이점은?](#constructor과-getInitialState의-차이점은) |
|90 | [setState를 호출하지 않고도 컴포넌트 리렌더링이 가능한가?](#setState를-호출하지-않고도-컴포넌트-리렌더링이-가능한가) |
|91 | [ES6 클래스를 사용하는 React에서 super()와 super(props)의 차이점은?](#ES6-클래스를-사용하는-React에서-super()와-super(props)의-차이점은) |
|92 | [JSX 내부에서 반복하는 방법?](#JSX-내부에서-반복하는-방법) |
|93 | [속성 인용문에 props를 어떻게 넣나?](#속성-인용문에-props를-어떻게-넣나) |
|94 | [모양이 있는 React proptype array란?](#모양이-있는-React-proptype-array란) |
|95 | [클래스 속성을 조건부로 적용하는 방법은?](#클래스-속성을-조건부로-적용하는-방법은) |
|96 | [React와 ReactDOM의 차이점?](#React와-ReactDOM의-차이점) |
|97 | [왜 ReactDOM은 React와 분리되었나?](#왜-ReactDOM은-React와-분리되었나) |
|98 | [React 라벨 엘리먼트를 사용하는 방법은?](#React-라벨-엘리먼트를-사용하는-방법은) |
|99 | [여러 개의 인라인 스타일 객체를 결합하는 방법은?](#여러-개의-인라인-스타일-객체를-결합하는-방법은) |
|100| [브라우저 크기를 조정할 때 뷰를 리렌더링하는 방법은?](#브라우저-크기를-조정할-때-뷰를-리렌더링하는-방법은)
|101| [setState()와 replaceState() 메서드의 차이점은?](#setState()와-replaceState()-메서드의-차이점은) |
|102| [state 변경을 인지하는 방법?](#state-변경을-인지하는-방법) |
|103| [React state에서 배열 엘리먼트를 제거하는 권장 방법은?](#React-state에서-배열-엘리먼트를-제거하는-권장-방법은) |
|104| [HTML 렌더링없이 React를 사용할 수 있나?](#HTML-렌더링없이-React를-사용할-수-있나) |
|105| [React에서 JSON을 이쁘게 출력하는 방법?](#React에서-JSON을-이쁘게-출력하는-방법) |
|106| [React에서 props를 업데이트할 수 없는 이유는?](#React에서-props를-업데이트할-수-없는-이유는) |
|107| [페이지 로드 시 input 엘리먼트에 포커스를 주는 방법은?](#페이지-로드-시-input-엘리먼트에-포커스를-주는-방법은) |
|108| [What are the possible ways of updating objects in state?](#what-are-the-possible-ways-of-updating-objects-in-state) |
|109| [왜 함수가 setState() 객체보다 선호되는가?](#왜-함수가-setState()-객체보다-선호되는가) |
|110| [브라우저 런타임에 React 버전을 어떻게 알 수 있나?](#브라우저-런타임에-React-버전을-어떻게-알-수-있나) |
|111| [create-react-app에 polyfill을 포함시키는 방법은?](#create-react-app에-polyfill을-포함시키는-방법은) |
|112| [create-react-app에서 http 대신 https를 사용하는 방법?](#create-react-app에서-http-대신-https를-사용하는-방법) |
|113| [How to avoid using relative path imports in create-react-app?](#how-to-avoid-using-relative-path-imports-in-create-react-app) |
|114| [React Router용 Google 웹 로그 분석을 추가하는 방법은?](#React-Router용-Google-웹-로그-분석을-추가하는-방법은) |
|115| [매 초마다 컴포넌트를 업데이트 하는 방법은?](#매-초마다-컴포넌트를-업데이트-하는-방법은) |
|116| [React에서 인라인 스타일에 벤더 접두사는 어떻게 적용하나?](#React에서-인라인-스타일에-벤더-접두사는-어떻게-적용하나) |
|117| [React와 ES6를 사용해서 컴포넌트를 가져오고 내보내는 방법은?](#React와-ES6를-사용해서-컴포넌트를-가져오고-내보내는-방법은) |
|118| [React 컴포넌트 이름이 대문자로 시작해야 하는 이유는?](#React-컴포넌트-이름이-대문자로-시작해야-하는-이유는) |
|119| [컴포넌트 생성자는 왜 한 번만 불리나?](#컴포넌트-생성자는-왜-한-번만-불리나) |
|120| [React에서 상수를 정의하는 방법은?](#React에서-상수를-정의하는-방법은) |
|121| [React에서 프로그래밍 방식으로 클릭 이벤트를 발생시키는 방법은?](#React에서-프로그래밍-방식으로-클릭-이벤트를-발생시키는-방법은) |
|122| [async/await를 평범한 React에서 사용할 수 있나?](#async/await를-평범한-React에서-사용할-수-있나) |
|123| [React의 일반적인 폴더 구조는?](#React의-일반적인-폴더-구조는) |
|124| [인기 애니메이션 패키지는?](#인기-애니메이션-패키지는) |
|125| [스타일 모듈의 이점은?](#스타일-모듈의-이점은) |
|126| [인기있는 React-관련 linters는?](#인기있는-React-관련-linters는) |
|127| [AJAX 호출하는 방법과 어느 컴포넌트 라이프 사이클 메서드에서 AJAX 호출을 해야하나?](#AJAX-호출하는-방법과-어느-컴포넌트-라이프-사이클-메서드에서-AJAX-호출을-해야하나?) |
|128| [render props란?](#render-props란) |
|   | **React Router** |
|129| [React Router란?](#React-Router란) |
|130| [React Router가 history 라이브러리와 다른점은?](#React-Router가-history-라이브러리와-다른점은) |
|131| [What are the \<Router> components of React Router v4?](#what-are-the-router-components-of-react-router-v4) |
|132| [What is the purpose of push and replace methods of history?](#what-is-the-purpose-of-push-and-replace-methods-of-history) |
|133| [How do you programmatically navigate using React router v4?](#how-do-you-programmatically-navigate-using-react-router-v4) |
|134| [How to get query parameters in React Router v4](#how-to-get-query-parameters-in-react-router-v4) |
|135| [Why you get "Router may have only one child element" warning?](#why-you-get-router-may-have-only-one-child-element-warning) |
|136| [How to pass params to history.push method in React Router v4?](#how-to-pass-params-to-historypush-method-in-react-router-v4) |
|137| [How to implement default or NotFound page?](#how-to-implement-default-or-notfound-page) |
|138| [How to get history on React Router v4?](#how-to-get-history-on-react-router-v4) |
|139| [How to perform automatic redirect after login?](#how-to-perform-automatic-redirect-after-login) |
|   | **React Internationalization** |
|140| [What is React-Intl?](#what-is-react-intl) |
|141| [What are the main features of React Intl?](#what-are-the-main-features-of-react-intl) |
|142| [What are the two ways of formatting in React Intl?](#what-are-the-two-ways-of-formatting-in-react-intl) |
|143| [How to use FormattedMessage as placeholder using React Intl?](#how-to-use-formattedmessage-as-placeholder-using-react-intl) |
|144| [How to access current locale with React Intl](#how-to-access-current-locale-with-react-intl) |
|145| [How to format date using React Intl?](#how-to-format-date-using-react-intl) |
|   | **React Testing** |
|146| [What is Shallow Renderer in React testing?](#what-is-shallow-renderer-in-react-testing) |
|147| [What is TestRenderer package in React?](#what-is-testrenderer-package-in-react) |
|148| [What is the purpose of ReactTestUtils package?](#what-is-the-purpose-of-reacttestutils-package) |
|149| [What is Jest?](#what-is-jest) |
|150| [What are the advantages of Jest over Jasmine?](#what-are-the-advantages-of-jest-over-jasmine) |
|151| [Give a simple example of Jest test case](#give-a-simple-example-of-jest-test-case) |
|   | **React Redux** |
|152| [What is Flux?](#what-is-flux) |
|153| [What is Redux?](#what-is-redux) |
|154| [What are the core principles of Redux?](#what-are-the-core-principles-of-redux) |
|155| [What are the downsides of Redux compared to Flux?](#what-are-the-downsides-of-redux-compared-to-flux) |
|156| [What is the difference between mapStateToProps() and mapDispatchToProps()?](#what-is-the-difference-between-mapstatetoprops-and-mapdispatchtoprops) |
|157| [Can I dispatch an action in reducer?](#can-i-dispatch-an-action-in-reducer) |
|158| [How to access Redux store outside a component?](#how-to-access-redux-store-outside-a-component) |
|159| [What are the drawbacks of MVW pattern](#what-are-the-drawbacks-of-mvw-pattern) |
|160| [Are there any similarities between Redux and RxJS?](#are-there-any-similarities-between-redux-and-rxjs) |
|161| [How to dispatch an action on load?](#how-to-dispatch-an-action-on-load) |
|162| [How to use connect from React Redux?](#how-to-use-connect-from-react-redux) |
|163| [How to reset state in Redux?](#how-to-reset-state-in-redux) |
|164| [Whats the purpose of at symbol in the redux connect decorator?](#whats-the-purpose-of-at-symbol-in-the-redux-connect-decorator) |
|165| [What is the difference between React context and React Redux?](#what-is-the-difference-between-react-context-and-react-redux) |
|166| [Why are Redux state functions called reducers?](#why-are-redux-state-functions-called-reducers) |
|167| [How to make AJAX request in Redux?](#how-to-make-ajax-request-in-redux) |
|168| [Should I keep all component's state in Redux store?](#should-i-keep-all-components-state-in-redux-store) |
|169| [What is the proper way to access Redux store?](#what-is-the-proper-way-to-access-redux-store) |
|170| [What is the difference between component and container in React Redux?](#what-is-the-difference-between-component-and-container-in-react-redux) |
|171| [What is the purpose of the constants in Redux? ](#what-is-the-purpose-of-the-constants-in-redux) |
|172| [What are the different ways to write mapDispatchToProps()?](#what-are-the-different-ways-to-write-mapdispatchtoprops) |
|173| [What is the use of the ownProps parameter in mapStateToProps() and mapDispatchToProps()?](#what-is-the-use-of-the-ownprops-parameter-in-mapstatetoprops-and-mapdispatchtoprops) |
|174| [How to structure Redux top level directories?](#how-to-structure-redux-top-level-directories) |
|175| [What is redux-saga?](#what-is-redux-saga) |
|176| [What is the mental model of redux-saga?](#what-is-the-mental-model-of-redux-saga) |
|177| [What are the differences between call and put in redux-saga](#what-are-the-differences-between-call-and-put-in-redux-saga) |
|178| [What is Redux Thunk?](#what-is-redux-thunk) |
|179| [What are the differences between redux-saga and redux-thunk](#what-are-the-differences-between-redux-saga-and-redux-thunk) |
|180| [What is Redux DevTools?](#what-is-redux-devtools) |
|181| [What are the features of Redux DevTools?](#what-are-the-features-of-redux-devtools) |
|182| [What are Redux selectors and Why to use them?](#what-are-redux-selectors-and-why-to-use-them) |
|183| [What is Redux Form?](#what-is-redux-form) |
|184| [What are the main features of Redux Form?](#what-are-the-main-features-of-redux-form) |
|185| [How to add multiple middlewares to Redux?](#how-to-add-multiple-middlewares-to-redux) |
|186| [How to set initial state in Redux?](#how-to-set-initial-state-in-redux) |
|187| [How Relay is different from Redux?](#how-relay-is-different-from-redux) |
|   | **React Native** |
|188| [What is the difference between React Native and React?](#what-is-the-difference-between-react-native-and-react) |
|189| [How to test React Native apps?](#how-to-test-react-native-apps) |
|190| [How to do logging in React Native?](#how-to-do-logging-in-react-native) |
|191| [How to debug your React Native?](#how-to-debug-your-react-native) |
|   | **React supported libraries and Integration** |
|192| [What is reselect and how it works?](#what-is-reselect-and-how-it-works) |
|193| [What is Flow?](#what-is-flow) |
|194| [What is the difference between Flow and PropTypes?](#what-is-the-difference-between-flow-and-proptypes) |
|195| [How to use font-awesome icons in React?](#how-to-use-font-awesome-icons-in-react) |
|196| [What is React Dev Tools?](#what-is-react-dev-tools) |
|197| [Why is DevTools not loading in Chrome for local files?](#why-is-devtools-not-loading-in-chrome-for-local-files) |
|198| [How to use Polymer in React?](#how-to-use-polymer-in-react) |
|199| [What are the advantages of React over Vue.js?](#what-are-the-advantages-of-react-over-vuejs) |
|200| [What is the difference between React and Angular?](#what-is-the-difference-between-react-and-angular) |
|201| [Why React tab is not showing up in DevTools?](#why-react-tab-is-not-showing-up-in-devtools) |
|202| [What are styled components?](#what-are-styled-components) |
|203| [Give an example of Styled Components?](#give-an-example-of-styled-components) |
|204| [What is Relay?](#what-is-relay) |
|205| [How to use TypeScript in create-react-app application?](#how-to-use-typescript-in-create-react-app-application) |
|   | **Miscellaneous** |
|206| [What are the main features of reselect library?](#what-are-the-main-features-of-reselect-library) |
|207| [Give an example of reselect usage?](#give-an-example-of-reselect-usage) |
|208| [What is an action in Redux?](#what-is-an-action-in-redux) |
|209| [Does the statics object work with ES6 classes in React?](#does-the-statics-object-work-with-es6-classes-in-react) |
|210| [Can Redux only be used with React?](#can-redux-only-be-used-with-react) |
|211| [Do you need to have a particular build tool to use Redux?](#do-you-need-to-have-a-particular-build-tool-to-use-redux) |
|212| [How Redux Form initialValues get updated from state?](#how-redux-form-initialvalues-get-updated-from-state) |
|213| [How React PropTypes allow different type for one prop?](#how-react-proptypes-allow-different-types-for-one-prop) |
|214| [Can I import an SVG file as react component?](#can-i-import-an-svg-file-as-react-component) |
|215| [Why are inline ref callbacks or functions not recommended?](#why-are-inline-ref-callbacks-or-functions-not-recommended)|
|216| [What is render hijacking in React?](#what-is-render-hijacking-in-react)|
|217| [What are HOC factory implementations?](#what-are-hoc-factory-implementations)|
|218| [How to pass numbers to React component?](#how-to-pass-numbers-to-react-component)|
|219| [Do I need to keep all my state into Redux? Should I ever use react internal state?](#do-i-need-to-keep-all-my-state-into-redux-should-i-ever-use-react-internal-state)|
|220| [What is the purpose of registerServiceWorker in React?](#what-is-the-purpose-of-registerserviceworker-in-react)|
|221| [What is React memo function?](#what-is-react-memo-function)|
|222| [What is React lazy function?](#what-is-react-lazy-function)|
|223| [How to prevent unnecessary updates using setState?](#how-to-prevent-unnecessary-updates-using-setstate)|
|224| [How do you render Array, Strings and Numbers in React 16 Version?](#how-do-you-render-array-strings-and-numbers-in-react-16-version)|
|225| [How to use class field declarations syntax in React classes?](#how-to-use-class-field-declarations-syntax-in-react-classes)|
|226| [What are hooks?](#what-are-hooks)|
|227| [What are the rules needs to follow for hooks?](#what-are-the-rules-needs-to-follow-for-hooks)|
|228| [How to ensure hooks followed the rules in your project?](#how-to-ensure-hooks-followed-the-rules-in-your-project)|
|229| [What are the differences between Flux and Redux?](#what-are-the-differences-between-flux-and-redux)|
|230| [What are the benefits of React Router V4?](#what-are-the-benefits-of-react-router-v4)|
|231| [Can you describe about componentDidCatch lifecycle method signature?](#can-you-describe-about-componentdidcatch-lifecycle-method-signature)|
|232| [In which scenarios error boundaries do not catch errors?](#in-which-scenarios-error-boundaries-do-not-catch-errors)|
|233| [Why do not you need error boundaries for event handlers?](#why-do-not-you-need-error-boundaries-for-event-handlers)|
|234| [What is the difference between try cath block and error boundaries?](#what-is-the-difference-between-try-catch-block-and-error-boundaries)|
|235| [What is the behavior of uncaught errors in react 16?](#what-is-the-behavior-of-uncaught-errors-in-react-16)|
|236| [What is the proper placement for error boundaries?](#what-is-the-proper-placement-for-error-boundaries)|
|237| [What is the benefit of component stack trace from error boundary?](#what-is-the-benefit-of-component-stack-trace-from-error-boundary)|
|238| [What is the required method to be defined for a class component?](#what-is-the-required-method-to-be-defined-for-a-class-component)|
|239| [What are the possible return types of render method?](#what-are-the-possible-return-types-of-render-method)|
|240| [What is the main purpose of constructor?](#what-is-the-main-purpose-of-constructor)|
|241| [Is it mandatory to define constructor for React component?](#is-it-mandatory-to-define-constructor-for-react-component)|
|242| [What are default props?](#what-are-default-props)|
|243| [Why should not call setState in componentWillUnmount?](#why-should-not-call-setstate-in-componentwillunmount)|
|244| [What is the purpose of getDerivedStateFromError?](#what-is-the-purpose-of-getderivedstatefromerror)|
|245| [What is the methods order when component re-rendered?](#what-is-the-methods-order-when-component-re-rendered)|
|246| [What are the methods invoked during error handling?](#what-are-the-methods-invoked-during-error-handling)|
|247| [What is the purpose of displayName class property?](#what-is-the-purpose-of-displayname-class-property)|
|248| [What is the browser support for react applications?](#what-is-the-browser-support-for-react-applications)|
|249| [What is the purpose of unmountComponentAtNode method?](#what-is-the-purpose-of-unmountcomponentatnode-method)|
|250| [What is code-splitting?](#what-is-code-splitting)|
|251| [What is the benefit of strict mode?](#what-is-the-benefit-of-strict-mode)|
|252| [What are Keyed Fragments?](#what-are-keyed-fragments)|
|253| [Is it React support all HTML attributes?](#is-it-react-support-all-html-attributes)|
|254| [What are the limitations with HOCs?](#what-are-the-limitations-with-hocs)|
|255| [How to debug forwardRefs in DevTools?](#how-to-debug-forwardrefs-in-devtools)|
|256| [When component props defaults to true?](#when-component-props-defaults-to-true)|
|257| [What is NextJS and major features of it?](#what-is-nextjs-and-major-features-of-it)|
|258| [How do you pass an event handler to a component?](#how-do-you-pass-an-event-handler-to-a-component)|
|259| [Is it good to use arrow functions in render methods?](#is-it-good-to-use-arrow-functions-in-render-methods)|
|260| [How to prevent a function from being called multiple times?](#how-to-prevent-a-function-from-being-called-multiple-times)|
|261| [How JSX prevents Injection Attacks?](#how-jsx-prevents-injection-attacks)|
|262| [How do you update rendered elements?](#how-do-you-update-rendered-elements)|
|263| [How do you say that props are read only?](#how-do-you-say-that-props-are-read-only)|
|264| [How do you say that state updates are merged?](#how-do-you-say-that-state-updates-are-merged)|
|265| [How do you pass arguments to an event handler?](#how-do-you-pass-arguments-to-an-event-handler)|
|266| [How to prevent component from rendering?](#how-to-prevent-component-from-rendering)|
|267| [What are the conditions to safely use the index as a key?](#what-are-the-conditions-to-safely-use-the-index-as-a-key)|
|268| [Is it keys should be globally unique?](#is-it-keys-should-be-globally-unique)|
|269| [What is the popular choice for form handling?](#what-is-the-popular-choice-for-form-handling)|
|270| [What are the advantages of formik over redux form library?](#what-are-the-advantages-of-formik-over-redux-form-library)|
|271| [Why do you not required to use inheritance?](#why-do-you-not-required-to-use-inheritance)|
|272| [Can I use web components in react application?](#can-i-use-web-components-in-react-application)|
|273| [What is dynamic import?](#what-is-dynamic-import)|
|274| [What are loadable components?](#what-are-loadable-components)|
|275| [What is suspense component?](#what-is-suspense-component)|
|276| [What is route based code splitting?](#what-is-route-based-code-splitting)|
|277| [Give an example on How to use context?](#give-an-example-on-how-to-use-context)|
|278| [What is the purpose of default value in context?](#what-is-the-purpose-of-default-value-in-context)|
|279| [How do you use contextType?](#how-do-you-use-contexttype)|
|280| [What is a consumer?](#what-is-a-consumer)|
|281| [How do you solve performance corner cases while using context?](#how-do-you-solve-performance-corner-cases-while-using-context)|
|282| [What is the purpose of forward ref in HOCs?](#what-is-the-purpose-of-forward-ref-in-hocs)|
|283| [Is it ref argument available for all functions or class components?](#is-it-ref-argument-available-for-all-functions-or-class-components)|
|284| [Why do you need additional care for component libraries while using forward refs?](#why-do-you-need-additional-care-for-component-libraries-while-using-forward-refs)|
|285| [How to create react class components without ES6?](#how-to-create-react-class-components-without-es6)|
|286| [Is it possible to use react without JSX?](#is-it-possible-to-use-react-without-jsx)|
|287| [What is diffing algorithm?](#what-is-diffing-algorithm)|
|288| [What are the rules covered by diffing algorithm?](#what-are-the-rules-covered-by-diffing-algorithm)|
|289| [When do you need to use refs?](#when-do-you-need-to-use-refs)|
|290| [Is it prop must be named as render for render props?](#is-it-prop-must-be-named-as-render-for-render-props)|
|291| [What are the problems of using render props with pure components?](#what-are-the-problems-of-using-render-props-with-pure-components)|
|292| [How do you create HOC using render props?](#how-do-you-create-hoc-using-render-props)|
|293| [What is windowing technique?](#what-is-windowing-technique)|
|294| [How do you print falsy values in JSX?](#how-do-you-print-falsy-values-in-jsx)|
|295| [What is the typical use case of portals?](#what-is-the-typical-use-case-of-portals?)|
|296| [How do you set default value for uncontrolled component?](#how-do-you-set-default-value-for-uncontrolled-component)|
|297| [What is your favorite React stack?](#what-is-your-favorite-react-stack)|
|298| [What is the difference between Real DOM and Virtual DOM?](#what-is-the-difference-between-real-dom-and-virtual-dom)|
|299| [How to add a bootstrap for a react application?](#how-to-add-a-bootstrap-for-a-react-application)|
|300| [Can you list down top websites or applications using react as front end framework?](#can-you-list-down-top-websites-or-applications-using-react-as-front-end-framework)|
|301| [Is it recommended to use CSS In JS technique in React?](#is-it-recommended-to-use-css-in-js-technique-in-react)|
|302| [Do I need to rewrite all my class components with hooks?](#do-i-need-to-rewrite-all-my-class-components-with-hooks)|
|303| [How to fetch data with React Hooks?](#how-to-fetch-data-with-react-hooks)|
|304| [Is Hooks cover all use cases for classes?](#is-hooks-cover-all-use-cases-for-classes)|
|305| [What is the stable release for hooks support?](#what-is-the-stable-release-for-hooks-support)|
|306| [Why do we use square brackets in useState?](#why-do-we-use-square-brackets-in-usestate)|
|307| [What are the sources used for introducing hooks?](#what-are-the-sources-used-for-introducing-hooks)|
|308| [How do you access imperative API of web components?](#how-do-you-access-imperative-api-of-web-components)|
|309| [What is formik?](#what-is-formik)|
|310| [What are typical middleware choices for handling asynchronous calls in Redux?](#what-are-typical-middleware-choices-for-handling-asynchronous-calls-in-redux)|
|311| [Is browsers understand JSX code?](#is-browsers-understand-jsx-code)|
|312| [Describe about data flow in react?](#describe-about-data-flow-in-react)|

## Core React

1. ### React란 무엇인가?

    React는 단일 페이지 어플리케이션으로 UI(user interface)를 만드는데 사용되는 **오픈-소스 프론트엔드 JavaScript 라이브러리** 로 웹과 모바일 앱에서 view layer를 다루는데 사용된다. React는 Facebook에서 소프트웨어 엔지니어로 있는 Jordan Walke가 만들었다. React는 2011년 Facebook's News Feed, 2012년 Instagram에서 처음 선보였다.

2. ### React의 주요 특징은?

    React의 주요 특징은 :

    * 실제돔(RealDOM)을 조작하는 것은 비용이 크다는 것을 고려하여 실제돔 대신에 **가상돔(VirtualDOM)** 을 사용한다.
    * **서버-사이드 렌더링(server-side rendering)** 를 지원한다.
    * **단방향** 데이터 흐름 또는 데이터 바인딩을 따른다.
    * 화면 개발을 위해 **재사용 가능한(reusable)/구성 가능한(composable)** UI 컴포넌트를 사용한다.

3. ### JSX란 무엇인가?

    *JSX* 는 ECMAScript를 위한 XML-처럼 생긴 구문 확장자(*JavaScript XML* 의 약어)이다. 기본적으로 `React.createElement()` 함수를 위한 syntactic sugar, JavaScript의 표현력과 HTML같은 템플릿 문법을 제공한다.

    아래 예제에서 `<h1>` 태그 안의 텍스트는 render 함수에 JavaScript 함수로 반환된다.

    ```jsx harmony
    class App extends React.Component {
      render() {
        return(
          <div>
            <h1>{'Welcome to React world!'}</h1>
          </div>
        )
      }
    }
    ```

4. ### Element와 Component의 차이점은?

    *Element* 는 DOM 노드나 다른 컴포넌트들 관점에서 화면에 보이기 원하는 걸 묘사한 일반 객체이다. *Elements* 는 props에 있는 다른 *Elements* 를 포함할 수 있다. React element를 만드는 것은 저렴하다. 일단 element가 만들어지면 절대 변경되지 않는다.

    React Element 객체 표현은 다음과 같다. :

    ```javascript
    const element = React.createElement(
      'div',
      {id: 'login-btn'},
      'Login'
    )
    ```

    위의 `React.createElement()` 함수는 객체를 반환한다. :

    ```
    {
      type: 'div',
      props: {
        children: 'Login',
        id: 'login-btn'
      }
    }
    ```

    마지막으로 `ReactDOM.render()` 를 사용해서 DOM으로 렌더링한다. :

    ```html
    <div id='login-btn'>Login</div>
    ```

    반면에 **component** 는 여러 다른 방법으로 선언될 수 있다. `render()` 메소드를 포함한 클래스가 될 수 있다. 또는 단순하게 함수로 정의될 수 있다. 두 경우 모두, 입력으로 props를 가져오고, 출력으로 JSX tree를 return한다.

    ```javascript
    const Button = ({ onLogin }) =>
      <div id={'login-btn'} onClick={onLogin} />
    ```

    JSX는 `React.createElement()` 함수 트리로 변환된다. :

    ```javascript
    const Button = ({ onLogin }) => React.createElement(
      'div',
      { id: 'login-btn', onClick: onLogin },
      'Login'
    )
    ```

5. ### React에서 components는 어떻게 만드나?

    컴포넌트를 만드는 방법은 2가지가 있다.

    1. **Function Components:** 컴포넌트를 만드는 가장 간단한 방법이다. 순수 JavaScript functions 로 첫번째 인자로는 props 객체를 받고 React elements를 반환한다. : 

        ```jsx harmony
        function Greeting({ message }) {
          return <h1>{`Hello, ${message}`}</h1> 
        }
        ```

    2. **Class Components:** ES6의 class를 사용해서 컴포넌트를 만들 수 있다. 위의 함수는 다음과 같이 작성될 수 있다. :

        ```jsx harmony
        class Greeting extends React.Component {
          render() {
            return <h1>{`Hello, ${this.props.message}`}</h1>
          }
        }
        ```

6. ### 언제 Function Component 대신에 Class Component를 사용하나?

    만약, 컴포넌트가 `state나 lifecycle methods`가 필요하다면 class 컴포넌트를 사용하고 아니라면 function 컴포넌트를 사용한다.
    
7. ### Pure Components란 무엇인가?

    *`React.PureComponent`* 는 `shouldComponentUpdate()` 메서드를 제어하는 것을 제외하면 *`React.Component`*와 다르지 않다. props나 state가 변경되면 *PureComponent* 는 props와 state 에 대해서 얕은 비교를 수행한다. 반면에 *Component* 는 현재의 props와 state에 대해 비교를 하지 않는다. 따라서 `shouldComponentUpdate`가 호출될 때마다 리렌더링된다.
    
8. ### React에서 state는 무엇인가?

    컴포넌트의 *State*는 컴포넌트의 변경 될 수 있는 정보를 보유하는 객체이다. 가능한 한 간단하게 상태를 만들고 stateful 컴포넌트의 수를 최소화해야 한다. message state를 가진 User 컴포넌트를 만들어보자.

    ```jsx harmony
    class User extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          message: 'Welcome to React world'
        }
      }

      render() {
        return (
          <div>
            <h1>{this.state.message}</h1>
          </div>
        )
      }
    }
    ```

    ![state](images/state.jpg)

    state는 props와 비슷하지만 private 하며 컴포넌트에 의해 제어된다. 즉, 상태는 이를 가지고 있거나 설정할 수 있는 컴포넌트 이외에는 접근할 수 없다.

9. ### React에서 props는 무엇인가?

      *Props*는 컴포넌트에 대한 입력이다. Props는 HTML 태그 속성과 같은 작명 규칙을 사용하여 컴포넌트에 전달되는 단일 값 혹은 객체다. props는 부모 컴포넌트에서 자식 컴포넌트로 전달된다.

      React에서 props의 주목적은 다음과 같은 컴포넌트의 기능들을 제공하는 것이다.

      1. 커스텀 데이터를 컴포넌트로 전달한다.
      2. state의 변경을 일으킨다.
      3. 컴포넌트의 `render()` 메서드 내에서 `this.props.reactProp` 를 통해 사용한다.

      예를 들어 `reactProp` 요소를 가진 엘리먼트를 만들어보자.

    ```jsx harmony
    <Element reactProp={'1'} />
    ```
    
    이 `reactProp` (또는 여러분이 만든 것은 무엇이든) React를 사용하여 생성된 모든 컴포넌트에 원래 존재하는 props 객체의 속성이 된다.

    ```
    props.reactProp
    ```

10. ### state와 prop의 차이점은?

    *props*와 *state*는 모두 순수 자바스크립트 객체다. 둘 다 렌더링 결과에 영향을 주는 정보를 가지고 있지만, 컴포넌트와 관련된 기능 면에서 다르다. props는 함수의 매개변수와 비슷하게 컴포넌트로 전달되는 반면, state는 함수 내에서 선언된 변수와 유사하게 컴포넌트 내에서 관리된다.

11. ### 왜 state를 직접 update하면 안되나?

    혹시라도 state를 직접적으로 업데이트를 하게 되면 컴포넌트는 re-render를 하지 않는다.

    ```javascript
    //Wrong
    this.state.message = 'Hello world'
    ```

    대신에 `setState()` 메소드를 사용한다. 이 메소드는 컴포넌트의 state 객체에 대한 업데이트를 예약한다. state가 바뀌게 되면, 컴포넌트는 re-rendering으로 응답을 한다.

    ```javascript
    //Correct
    this.setState({ message: 'Hello World' })
    ```

    **Note:** *constructor*에서나 최신 Javascript의 class 선언 구문을 사용해서 state 객체에 직접 할당할 수 있다.

12. ### `setState()`의 argument로 callback 함수를 사용하는 이유는?

    callback 함수는 setState가 끝나고 컴포넌트가 render 되었을 때 작동한다. `setState()`는 **비동기식**이여서 callback 함수는 모든 작업 후 사용된다.

    **Note:** 이 callback 함수보다는 lifecycle 메소드를 사용하는 것이 좋다.

    ```javascript
    setState({ name: 'John' }, () => console.log('The name has updated and component re-rendered'))
    ```

13. ### HTML과 React의 event handling의 차이점은?

    1. HTML에서, 이벤트 이름은 *소문자*여야 한다:

    ```html
    <button onclick='activateLasers()'>
    ```

    반면에 React에서는 *camelCase* 규칙을 따른다:

    ```jsx harmony
    <button onClick={activateLasers}>
    ```

    1.  HTML에서, 기본 동작 방지를 위해 `false`를 반환할 수 있다:

    ```html
    <a href='#' onclick='console.log("The link was clicked."); return false;' />
    ```

    반면에 React에서는 `preventDefault()`를 명시적으로 호출해야 한다:

    ```javascript
    function handleClick(event) {
      event.preventDefault()
      console.log('The link was clicked.')
    }
    ```

14. ### 어떻게 JSX 콜백에서 메서드와 이벤트 핸들러를 바인드하나?

    이를 이루기 위한 3가지 방법이 있다.

    1.	**생성자에서 바인딩:** JavaScript 클래스에서, 메서드는 기본적으로 바인딩 되지 않는다. 클래스 메서드로 정의된 React  이벤트 핸들러에게서도 똑같은 문제가 적용된다. 일반적으로 우리는 생성자 안에서 바인드를 한다.

    ```javascript
    class Component extends React.Componenet {
      constructor(props) {
        super(props)
        this.handleClick = this.handleClick.bind(this)
      }

      handleClick() {
        // ...
      }
    }
    ```

    1. **Public 클래스 필드 구문:** 바인드 접근법이 싫다면 콜백을 올바르게 바인드하기 위해 *public 클래스 필드 구문* 을 사용할 수 있다.

    ```jsx harmony
    handleClick = () => {
      console.log('this is:', this)
    }
    ```

    ```jsx harmony
    <button onClick={this.handleClick}>
      {'Click me'}
    </button>
    ```

    1. **콜백 안에서 화살표 함수:** 콜백 안에서 직접 *화살표 함수*를 사용할 수 있다.

    ```jsx harmony
    <button onClick={(event) => this.handleClick(event)}>
      {'Click me'}
    </button>
    ```

    **Note:** 콜백이 자식 컴포넌트에 prop으로 전달이 되면, 해당 컴포넌트는 추가 리렌더링을 수행할 수 있다. 이 경우에, 성능을 고려하여 `.bind()` 또는 *public 클래스 필드 구문* 접근법을 사용하는 것이 좋다.

15. ### 어떻게 이벤트 핸들러나 콜백에 매개 변수를 전달하나?

    *화살표 함수*를 사용해서 *이벤트 핸들러*를 감싸고 매개변수를 전달할 수 있다.

    ```jsx harmony
    <button onClick={() => this.handleClick(id)} />
    ```

    `.bind`를 호출하는 것과 동일하다:

    ```jsx harmony
    <button onClick={this.handleClick.bind(this, id)} />
    ```
    Apart from these two approaches, you can also pass arguments to a function which is defined as array function
    ```jsx harmony
    <button onClick={this.handleClick(id)} />
    handleClick = (id) => () => {
        console.log("Hello, your ticket number is", id)
    };
    ```

16. ### React에 SyntheticEvent란 무엇인가?

    `SyntheticEvent`는 브라우저의 기본 이벤트를 감싼 cross-browser wrapper이다. `stopPropagation()`과 `preventDefault()`를 포함한 API로, 브라우저의 기본 이벤트와 동일하지만, 모든 브라우저에서 동일하게 작동한다는 점이 다르다.

17. ### 인라인 조건 표현식이란?

    JS에서 조건부로 식을 표현하기 위해서 *if 문* 이나 *삼항 표현식* 을 사용할 수 있다. 이러한 접근법 외에도, JS 논리연산자인 `&&`가 있는 중괄호로 감싼 표현식을 JSX에 포함할 수도 있다.

    ```jsx harmony
    <h1>Hello!</h1>
    {
        messages.length > 0 && !isLogin?
          <h2>
              You have {messages.length} unread messages.
          </h2>
          :
          <h2>
              You don't have unread messages.
          </h2>
    }
    ```

18. ### "key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?

    `key`는 elements 배열을 만들 때 포함**시켜야 하는** 특수 문자열 속성이다. *Keys*는 React가 변경, 추가, 제거된 항목을 식별하는 데 도움을 준다.

    우리는 대개 데이터에서 ID를 *keys*로 사용한다.

    ```jsx harmony
    const todoItems = todos.map((todo) =>
      <li key={todo.id}>
        {todo.text}
      </li>
    )
    ```

    렌더링된 항목 중 안정적인 ID가 없을 때, 마지막 수단으로 항목의 *index*를 *key*로 사용할 수 있다.

    ```jsx harmony
    const todoItems = todos.map((todo, index) =>
      <li key={index}>
        {todo.text}
      </li>
    )
    ```

    **Note:**

    1. 항목의 순서가 변경될 수 있는 경우 *index*를 *keys*로 사용하는 것은 **추천하지 않는다.** 이는 성능 저하와 컴포넌트 state에 문제를 발생시킬 수 있다.
    2. 리스트 항목을 별도의 컴포넌트로 추출하는 경우 `li` 태그 대신에 리스트 컴포넌트에 *keys*를 적용해라.
    3. 리스트 항목에 `key` prop가 없으면 console에 경고 메시지가 표시될 것이다.

19. ### refs는 어떻게 사용되는가?

    *ref*는 엘리먼트에 대한 참조를 반환하는 데 사용된다. 대부분의 경우에서 *피하는 것이 좋지만*, DOM 엘리먼트나 컴포넌트의 인스턴스에 직접 접근하는 경우 유용할 수 있다.

20. ### refs는 어떻게 생성하는가?

    refs를 생성하는 방법에는 2가지 방법이 있다.
    1. 다음은 최근에 추가된 방법이다. *Refs*는 `React.createRef()`메서드를 통해 생성되며 `ref` 속성을 통해 React 엘리먼트에 적용된다. 엘리먼트 전체에서 *refs*를 사용하려면 생성자 내의 인스턴스 속성에 *ref*를 할당하면 된다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        this.myRef = React.createRef()
      }
      render() {
        return <div ref={this.myRef} />
      }
    }
    ```
    1. React 버전에 관계없이 ref 콜백 접근법을 사용할 수도 있다. 예를 들어, 검색창 컴포넌트의 입력 엘리먼트에서는 다음과 같이 접근한다.
    ```jsx harmony
    class SearchBar extends Component {
       constructor(props) {
          super(props);
          this.txtSearch = null;
          this.state = { term: '' };
          this.setInputSearchRef = e => {
             this.txtSearch = e;
          }
       }
       onInputChange(event) {
          this.setState({ term: this.txtSearch.value });
       }
       render() {
          return (
             <input
                value={this.state.term}
                onChange={this.onInputChange.bind(this)}
                ref={this.setInputSearchRef} />
          );
       }
    }
    ```

    **클로저(closures)** 를 사용하여 함수형 컴포넌트에서 *refs*를 사용할 수도 있다.
    **참고**: 권장하진 않지만, 인라인 ref 콜백을 이용할 수도 있다.

21. ### forward refs는 무엇인가?

    *Ref 전달(Ref forwarding)* 특정 컴포넌트에서 *ref*를 받아 자식에게 전달하는 기능이다.

    ```jsx harmony
    const ButtonElement = React.forwardRef((props, ref) => (
      <button ref={ref} className="CustomButton">
        {props.children}
      </button>
    ));

    // Create ref to the DOM button:
    const ref = React.createRef();
    <ButtonElement ref={ref}>{'Forward Ref'}</ButtonElement>
    ```

22. ### callback refs 및 findDOMNode()에서 선호되는 옵션은?

    `findDOMNode()` API 위에 *callback refs*를 사용하는 것이 좋다. `findDOMNode()`이 추후 React에서의 개선 사항을 방해하기 때문이다.

    `findDOMNode`를 사용하는 **legacy** 접근법은 다음과 같다.

    ```javascript
    class MyComponent extends Component {
      componentDidMount() {
        findDOMNode(this).scrollIntoView()
      }

      render() {
        return <div />
      }
    }
    ```

    권장되는 접근법은 다음과 같다.

    ```javascript
    class MyComponent extends Component {
      componentDidMount() {
        this.node.scrollIntoView()
      }

      render() {
        return <div ref={node => this.node = node} />
      }
    }
    ```

23. ### String Refs가 왜 legacy인가?

    React를 사용해보기 전이라면, 예전 API에서 `ref={'textInput'}`과 같은 `ref` 속성이 문자열인 것과 DOM node가 `this.refs.textInput`과 같이 액세스 되는 것에 익숙할 것이다. *String Refs에 문제가 있어*, legacy로 간주하기 때문에 사용하지 않기를 바란다. String Refs는 **React v16에 제거되었다**.

    1. *React가 현재 실행 중인 컴포넌트를 추적하도록 강제된다*. 이는 react 모듈을 stateful 하게 만들고, react 모듈이 번들에 복제될 때 이상한 오류를 유발하기 때문에 문제가 된다.
    2. *composable* 하지 않다. — 라이브러리가 전달된 자식에 ref를 넣으면, 사용자는 다른 ref를 추가할 수 없다. Callback ref는 완벽하게 구성이 가능하다.
    3. Flow와 같은 *정적 분석에서는 작동하지 않는다*. Flow는 프레임워크가 String Refs를 `this.refs`에 표시하도록 하는 마법과 그것의 타입(다를 수 있음)을 추측할 수 없다. Callback ref는 정적 분석에 친숙합니다..
    4. 대부분의 사람이 생각하는 "render callback" 패턴으로 작동하지 않는다. (예). `<DataGrid renderRow={this.renderRow} />`)
       ```jsx harmony
       class MyComponent extends Component {
         renderRow = (index) => {
           // This won't work. Ref will get attached to DataTable rather than MyComponent:
           return <input ref={'input-' + index} />;

           // This would work though! Callback refs are awesome.
           return <input ref={input => this['input-' + index] = input} />;
         }

         render() {
           return <DataTable data={this.props.data} renderRow={this.renderRow} />
         }
       }
       ```
24. ### Virtual DOM이란?

    *Virtual DOM* (VDOM)는 *실제 DOM*의 인-메모리 표현이다. UI 표현은 메모리에 유지되고 "실제" DOM과 동기화된다. 이는 렌더 함수의 호출과 화면상 elements를 표현하는 사이에 발생하는 단계이다. 이 전체 프로세스는 *조정* 이라고 한다.

25. ### Virtual DOM은 어떻게 작동하나?

    *Virtual DOM*는 세 가지 간단한 단계로 작동한다.

    1. 기본 데이터가 변경될 때마다, 전체 UI는 Virtual DOM 표현으로 리렌더링 된다.
        ![vdom](images/vdom1.png)

    2. 이전 DOM 표현과 새로운 표현 사이의 차이를 계산한다.
        ![vdom2](images/vdom2.png)

    3. 계산이 완료되면, 실제 DOM은 실제로 변경된 것만 업데이트할 것이다.
        ![vdom3](images/vdom3.png)

26. ### Shadow DOM과 Virtual DOM의 차이점

    *Shadow DOM* 주로 *웹 컴포넌트*에서 변수와 CSS의 범위 지정을 위해 디자인된 브라우저 기술이다. *Virtual DOM*는 브라우저 API를 기반으로 Javascript 라이브러리로 구현된 개념이다.

27. ### React Fiber란?

    Fiber는 React v16에서 새로운 *조정된* 엔진 또는 핵심 알고리즘의 재구현이다. React Fiber의 목표는 애니메이션, 레이아웃, 제스처, 작업 일시중지, 중단, 재사용 같은 영역에 대한 적합성을 높이고 다양한 유형의 업데이트에 우선순위를 정하는 것이다. 

28. ### React Fiber의 주요 목표는??

    *React Fiber*의 목표는 애니메이션, 레이아웃, 제스처, 작업 일시중지, 중단, 재사용 같은 영역에 대한 적합성을 높이는 것이다. 주요 기능은 **incremental rendering**으로 렌더링 작업을 청크(chunk)로 분할하고 여러 프레임에 걸쳐 펼치는 기능이다.

29. ### controlled components란?

    사용자가 입력한 뒤 폼의 입력창을 제어하는 component를 **Controlled Component**라고 한다. 즉 모든 상태 변이에는 관련된 핸들러 함수가 있다.

    예를 들어, 모든 이름을 대문자로 작성하기 위해서, 아래와 같은 handleChange를 사용한다.

    ```javascript
    handleChange(event) {
      this.setState({value: event.target.value.toUpperCase()})
    }
    ```

30. ### uncontrolled components란?

    The **Uncontrolled Components**는 내부적으로 자신의 상태를 저장하는 것으로, 현재의 값을 찾기 위해 필요하다면 ref를 사용하여 DOM에서 찾아온다. 이것은 전통적인 HTML과 더 비슷하다.

    아래의 UserProfile component에서, `이름` 입력은 ref를 사용해서 액세스한다.

    ```jsx harmony
    class UserProfile extends React.Component {
      constructor(props) {
        super(props)
        this.handleSubmit = this.handleSubmit.bind(this)
        this.input = React.createRef()
      }

      handleSubmit(event) {
        alert('A name was submitted: ' + this.input.current.value)
        event.preventDefault()
      }

      render() {
        return (
          <form onSubmit={this.handleSubmit}>
            <label>
              {'Name:'}
              <input type="text" ref={this.input} />
            </label>
            <input type="submit" value="Submit" />
          </form>
        );
      }
    }
    ```

    대부분의 경우 양식을 구현하는 데 controlled components를 사용하는 것을 추천한다.

31. ### createElement와 cloneElement의 차이점은?

    JSX elements는 `React.createElement()` 함수로 옮겨져서 UI의 객체 표현에 사용되는 React elements를 만든다. 반면에 `cloneElement`은 element를 복사하고 새로운 props로 전달하는 데 사용된다.

32. ### React에서 Lifting State Up란?

    여러 컴포넌트가 동일한 변경 데이터를 공유해야 하는 경우 가장 가까운 공통 조상으로 *lift the shared state up*을 하는 것을 추천한다. 즉 2개의 자식 컴포넌트가 부모로부터 동일한 데이터를 공유하는 경우, 모든 자식 컴포넌트에서 로컬 상태를 유지하는 대신에 상태를 부모에서 관리하는 것이다.

33. ### 컴포넌트 라이프 사이클의 다른 단계들은?

    컴포넌트 라이프 사이클는 세 가지의 고유한 단계가 있다.

    1. **Mounting:** 컴포넌트가 브라우저 DOM에 mount 할 준비가 되었다. 이 단계는 `constructor()`, `getDerivedStateFromProps()`, `render()`, `componentDidMount()` 라이프 사이클 메서드의 초기화에 대해 다룬다.

    2. **Updating:** 이 단계에서는, 컴포넌트는 두 가지 방법으로 업데이트가 되는데, 새로운 props를 보내거나, `setState()` 또는 `forceUpdate()`으로 state를 업데이트하는 것이다. 이 단계에서는 `getDerivedStateFromProps()`, `shouldComponentUpdate()`, `render()`, `getSnapshotBeforeUpdate()`, `componentDidUpdate()` 라이프 사이클 메서드를 다룬다.

    3. **Unmounting:** 이 마지막 단계에서는, 컴포넌트는 필요하지 않으며 브라우저 DOM에서 unmount된다. 이 단계에서는 `componentWillUnmount()` 라이프 사이클 메서드가 포함된다.

    React는 DOM에 변경 사항을 적용할 때 내부적으로 단계의 개념을 가지고 있다는 것을 언급할 필요가 있다. 다음과 같이 분리된다.

    1. **Render** 컴포넌트는 부수 효과 없이 렌더링 된다. Pure 컴포넌트에 적용되며 이 단계에서 React는 렌더링을 일시 정지, 중단 또는 재시작할 수 있다.

    2. **Pre-commit** 컴포넌트가 실제로 DOM에 변경사항을 적용하기 전에, React가 `getSnapshotBeforeUpdate()`를 통해서 DOM을 읽을 수 있는 순간이다.

    3. **Commit** React는 DOM과 함께 작동하고 Mount를 위한 `componentDidMount()`, 업데이트를 위한 `componentDidMount()`, Unmount를 위한 `componentWillUnmount()`의 최종 라이프 사이클을 각각 실행한다.

    React 16.3+ 단계 (또는) [일반적인 버전](http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/))

    ![phases 16.3+](images/phases16.3.jpg)

    React 16.3 전에는

    ![phases 16.2](images/phases.png)


34. ### React의 라이프 사이클 메서드에는 무엇이 있나?

    React 16.3+

    - **getDerivedStateFromProps:** `render()`가 호출되기 바로 전에 호출되며 *모든* 렌더링에서 호출된다. 이전 state가 필요한 드문 경우에 사용이 된다. [이전 state가 필요하면](https://reactjs.org/blog/2018/06/07/you-probably-dont-need-derived-state.html) 읽을만한 가치가 있다.
    - **componentDidMount:** 첫 번째 렌더링 이후에 실행되고, 여기서 모든 AJAX 요청, DOM 또는 state 업데이트 및 이벤트 리스너가 설정된다.
    - **shouldComponentUpdate:** 컴포넌트를 업데이트 해야 할지 여부를 결정한다. 기본적으로 `true`를 반환한다. state나 props가 업데이트된 후에 컴포넌트를 렌더링할 필요 없다고 확신하는 경우 false를 반환할 수 있다. 컴포넌트가 새로운 props를 받으면 리렌더링하는 것을 방지할 수 있어 성능을 향상하는데 매우 좋다.
    - **getSnapshotBeforeUpdate:** 렌더링 된 출력이 DOM에 커밋되기 바로 직전에 실행된다. 이로 인해 모든 값은 `componentDidUpdate()`에 전달이 된다. DOM에서 스크롤 위치 같은 정보를 가져오는 데 유용하다.
    - **componentDidUpdate:** 주로 props나 state의 변경에 대한 응답으로 DOM을 업데이트하는데 사용된다. `shouldComponentUpdate()`가 `false`를 반환하면 실행되지 않는다.
    - **componentWillUnmount** 나가는 네트워크 요청을 취소하거나 컴포넌트와 관련된 모든 이벤트 리스너를 제거하는 데 사용된다.

    Before 16.3

    - **componentWillMount:** 렌더링 전에 실행되며 root 컴포넌트의 App 수준 구성을 하는 데 사용된다.
    - **componentDidMount:** 첫 번째 렌더링 이후에 실행되고, 여기서 모든 AJAX 요청, DOM 또는 state 업데이트 및 이벤트 리스너가 설정된다.
    - **componentWillReceiveProps:** 특정 props 업데이트가 state 전환을 일으킬 때 실행된다.
    - **shouldComponentUpdate:** 컴포넌트를 업데이트 해야 할지 여부를 결정한다. 기본적으로 `true`를 반환한다. state나 props가 업데이트된 후에 컴포넌트를 렌더링할 필요 없다고 확신하는 경우 false를 반환할 수 있다. 컴포넌트가 새로운 props를 받으면 리렌더링하는 것을 방지할 수 있어 성능을 향상하는데 매우 좋다.
    - **componentWillUpdate:** true를 반환하는 `shouldComponentUpdate()`에 의해 확인된 props 및 state 변경이 있을 때 컴포넌트를 리렌더링하기 전에 실행된다.
    - **componentDidUpdate:** 주로 props나 state 변경에 대한 응답으로 DOM을 업데이트하는 데 사용된다.
    - **componentWillUnmount:** 나가는 네트워크 요청을 취소하거나 컴포넌트와 관련된 모든 이벤트 리스너를 제거하는 데 사용된다.

35. ### 고차(Higher-Order) 컴포넌트란?

    *고차(Higher-Order) 컴포넌트* (*HOC*)는 컴포넌트를 가져와서 새로운 컴포넌트를 반환하는 함수이다. 기본적으로, 컴포넌트 구성상의 본질에서 파생된 패턴이다.

    동적으로 제공된 자식 컴포넌트는 허용할 수 있지만, 입력 컴포넌트의 어떠한 동작을 수정하거나 복사하지 않으므로 **순수 컴포넌트(pure components)** 라고 부른다. 

    ```javascript
    const EnhancedComponent = higherOrderComponent(WrappedComponent)
    ```

    HOC는 아래와 같은 많은 사례에서 사용할 수 있다.

    1. 코드 재사용, 논리 및 부트스트랩 추상화
    2. 도용 렌더링
    3. State 추상화 및 조작
    4. Props 조작.

36. ### HOC 컴포넌트를 사용해서 props 프록시를 만드는 방법은?

    다음과 같이 *props proxy* 패턴을 사용하여 컴포넌트에 전달된 props를 추가/편집할 수 있다.

    ```jsx harmony
    function HOC(WrappedComponent) {
      return class Test extends Component {
        render() {
          const newProps = {
            title: 'New Header',
            footer: false,
            showFeatureX: false,
            showFeatureY: true
          }

          return <WrappedComponent {...this.props} {...newProps} />
        }
      }
    }
    ```

37. ### context란?

    *Context*는 수동으로 모든 단계에 props를 전달하지 않고 컴포넌트 트리를 통해 데이터를 전달하는 방법을 제공한다. 예를 들어, 인증된 사용자, locale 기본 설정, UI 테마는 많은 컴포넌트를 통해 응용 프로그램에서 액세스해야 한다.

    ```javascript
    const {Provider, Consumer} = React.createContext(defaultValue)
    ```

38. ### children prop이란?

    *Children*(`this.prop.children`)는 다른 prop와 마찬가지로 다른 컴포넌트에 데이터를 전달할 수 있는 요소(`this.prop.children`)다. 컴포넌트의 여는 태그와 닫는 태그 사이에 놓인 컴포넌트 트리가 해당 컴포넌트의 `children` prop로 전달된다.

    이 prop을 사용하기 위해 React API에서 사용할 수 있는 여러 가지 방법이 있다. 여기에는`React.Children.map`,`React.Children.forEach`,`React.Children.count`,`React.Children.only`,`React.Children.toArray`가 포함된다.
    children prop의 간단한 사용법은 다음과 같다.

    ```jsx harmony
    const MyDiv = React.createClass({
      render: function() {
        return <div>{this.props.children}</div>
      }
    })

    ReactDOM.render(
      <MyDiv>
        <span>{'Hello'}</span>
        <span>{'World'}</span>
      </MyDiv>,
      node
    )
    ```

39. ### React에서 주석을 어떻게 다는가?

    React / JSX의 주석은 JavaScript Multiline 주석과 유사하지만 중괄호로 묶인다.

    **Single-line comments:**

    ```jsx harmony
    <div>
      {/* 한 줄 주석 (바닐라 자바 스크립트에서는 한 줄 주석은 이중 슬래시 (//)로 표시된다) */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```

    **Multi-line comments:**

    ```jsx harmony
    <div>
      {/* 한 줄이상의
        여러 줄 주석 */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```

40. ### props argument가 있는 생성자에서 super를 사용하는 목적은 무엇입니까?

    자식 클래스 생성자는`super()`메서드가 호출 될 때까지 `this`를 참조할 수 없습니다. ES6 하위 클래스에도 동일하게 적용된다. super() 호출에 props 매개 변수를 전달하는 주요한 이유는 자식 생성자에서 `this.props`에 접근하기 위해서다.

    **props 전달**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    **props 미전달**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()

        console.log(this.props) // prints undefined

        // but props parameter is still available
        console.log(props) // prints { name: 'John', age: 42 }
      }

      render() {
        // no difference outside constructor
        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    위 코드를 보면 `this.props`가 생성자 내에서만 다른 것을 볼 수 있다. 생성자 밖에서는 동일하다.

41. ### 조정(reconciliation)이란?

    컴포넌트의 props나 state가 변경되었을 때, React는 새로 반환된 엘리먼트와 이전에 렌더링된 것을 비교해서 실제 DOM이 업데이트가 필요한지를 결정한다. 동등하지 않을 때, React가 DOM을 업데이트할 것이다. 이 프로세스를 *조정(reconciliation)*이라고 한다.

42. ### state의 키 이름을 동적으로 설정하는 방법은?

    ES6나 Babel transpiler를 사용하여 JSX코드를 변환하는 경우 *원하는 속성(property)명*으로 설정할 수 있다.

    ```javascript
    handleInputChange(event) {
      this.setState({ [event.target.id]: event.target.value })
    }
    ```

43. ### 컴포넌트가 렌더링 될 때마다 호출되는 함수에 대한 실수는 무엇일까?

    함수를 매개변수로 전달하는 동안 함수가 호출되지 않도록 확인해야 한다.

    ```jsx harmony
    render() {
      // Wrong: handleClick is called instead of passed as a reference!
      return <button onClick={this.handleClick()}>{'Click Me'}</button>
    }
    ```

    대신에, 괄호 없이 함수 자체를 전달해야 한다.

    ```jsx harmony
    render() {
      // Correct: handleClick is passed as a reference!
      return <button onClick={this.handleClick}>{'Click Me'}</button>
    }
    ```

44. ### 왜 컴포넌트 이름은 대문자로 해야 하나?

    컴포넌트는 DOM 엘리먼트가 아니기 때문에 대문자로 표기해야 한다. 또한, JSX 소문자 태그 이름은 HTML 엘리먼트를 나타내며 컴포넌트는 참조하지 않는다.

45. ### React는 왜 `class`가 아닌 `className` 속성을 사용하나?

    `class`는 JavasScript의 키워드이며, JSX는 JavaScript의 확장이다. 이것이 React가 `class` 대신 `className`을 사용하는 주된 이유이다. `className` prop으로 문자열을 넘겨야 한다.

    ```jsx harmony
    render() {
      return <span className={'menu navigation-menu'}>{'Menu'}</span>
    }
    ```

46. ### fragments란?

    컴포넌트가 여러 엘리먼트를 반환하는 데 사용하는 React의 일반적인 패턴이다. *Fragments*를 사용하면 DOM에 노드를 추가하지 않고 자식 목록을 그룹화할 수 있다.

    ```jsx harmony
    render() {
      return (
        <React.Fragment>
          <ChildA />
          <ChildB />
          <ChildC />
        </React.Fragment>
      )
    }
    ```

    *더욱더 짧은 구문*도 있지만, 많은 도구에서 지원하지 않는다.

    ```jsx harmony
    render() {
      return (
        <>
          <ChildA />
          <ChildB />
          <ChildC />
        </>
      )
    }
    ```

47. ### div보다 fragments가 더 우수한 이유는?

    1. Fragments는 조금 더 빠르며 여분의 DOM 노드를 만들지 않아서 메모리를 덜 사용한다. 이것은 매우 크고 깊은 트리(tree)에서 실질적인 이득을 가져다준다.
    2. *Flexbox*와 *CSS Grid* 같은 일부 CSS 메커니즘에는 특수한 부모-자식 관계를 가지고 있어서, 중간에 div를 추가하면 원하는 레이아웃을 유지하기가 어렵다.
    3. DOM Inspector가 덜 복잡해진다.

48. ### React의 portals이란?

    *Portal*은 상위 컴포넌트의 DOM 계층 구조 외부에 있는 DOM 노드에 자식을 렌더링하는데 권장되는 방법이다.

    ```javascript
    ReactDOM.createPortal(child, container)
    ```

    첫 번째 인수는 렌더링 가능한 React 엘리먼트, 문자열, fragment 같은 하위요소이다. 두 번째 인수는 DOM 엘리먼트이다.

49. ### stateless 컴포넌트란?

    동작이 state와 관련이 없는 경우 stateless 컴포넌트가 될 수 있다. function이나 class를 사용해서 stateless 컴포넌트를 만들 수 있다. 컴포넌트에서 라이프 사이클 훅을 사용해야 하는 경우가 아니라면 function 컴포넌트를 사용하는게 좋다. function 컴포넌트를 사용하면 여러 이점이 있는데, 쓰기, 이해 및 테스트하기가 쉽고 더 빠르며, `this` 키워드를 피할 수 있다.

50. ### stateful 컴포넌트란?

    컴포넌트의 동작이 컴포넌트의 *state*에 따라 달라진다면 stateful 컴포넌트라고 할 수 있다. *stateful 컴포넌트*는 항상 *class 컴포넌트* 이며 `constructor`에서 초기화가 되어 state를 가지게 된다.

    ```javascript
    class App extends Component {
      constructor(props) {
        super(props)
        this.state = { count: 0 }
      }

      render() {
        // ...
      }
    }
    ```

51. ### React에서 props 유효성 검사를 적용하는 방법은?

    응용 프로그램이 *development 모드*에서 실행될 때, React는 자동으로 컴포넌트에 설정한 모든 props를 확인하여 *올바른 타입*인지 확인한다. 타입이 맞지 않는다면, React는 콘솔에 경고 메시지를 띄운다. *production 모드*에서는 성능에 영향을 미치므로 사용할 수 없다. 주요한 props는 `isRequired`로 정의된다.

    사전 정의된 props 타입이다.

    1. `PropTypes.number`
    2. `PropTypes.string`
    3. `PropTypes.array`
    4. `PropTypes.object`
    5. `PropTypes.func`
    6. `PropTypes.node`
    7. `PropTypes.element`
    8. `PropTypes.bool`
    9. `PropTypes.symbol`
    10. `PropTypes.any`

    다음과 같이 `User` 컴포넌트에 대한 `propTypes`을 정의할 수 있다.

    ```jsx harmony
    import React from 'react'
    import PropTypes from 'prop-types'

    class User extends React.Component {
      static propTypes = {
        name: PropTypes.string.isRequired,
        age: PropTypes.number.isRequired
      }

      render() {
        return (
          <>
            <h1>{`Welcome, ${this.props.name}`}</h1>
            <h2>{`Age, ${this.props.age}`}</h2>
          </>
        )
      }
    }
    ```

    **Note:** React v15.5버전에서 *PropTypes*는 `React.PropTypes`에서 `prop-types` 라이브러리로 이동되었다.

52. ### React의 장점은?

    1. *Virtual DOM*으로 애플리케이션의 성능이 향상된다.
    2. JSX는 코드를 읽고 쓰기 쉽게 해준다.
    3. 클라이언트와 서버사이드(*SSR*) 렌더링이 둘 다 가능하다.
    4. 오직 view 라이브러리이기 때문에, 프레임워크(Angular, Backbone)에 쉽게 통합이 가능하다.
    5. Jest와 같은 툴을 사용하여 단위 및 통합 테스트를 쉽게 작성할 수 있다.

53. ### React의 한계는?

    1. React는 프레임워크가 아닌, view 라이브러리이다.
    2. 웹 개발을 처음 접하는 초보자에게 러닝 커브가 존재한다.
    3. 기존 MVC 프레임워크에 React를 통합하려면 몇 가지 추가 구성이 필요하다.
    4. 인라인 템플릿과 JSX로 인해 코드 복잡성이 증가한다.
    5. 너무 많은 작은 컴포넌트는 엔지니어링 또는 보일러 플레이트로 이어진다.

54. ### React v16에서 error boundaries란 무엇인가?

    *Error boundaries*는 하위 컴포넌트의 모든 위치에서 JavaScript 오류를 catch하고, 오류를 기록하며, 오류가 발생한 컴포넌트 트리 대신 폴백(fallback) UI를 표시하는 컴포넌트이다.

    클래스 컴포넌트는 `componentDidCatch(error, info)` 또는 `static getDerivedStateFromError()`라는 새로운 라이프 사이클 메서드를 정의하면 error boundary가 된다.

    ```jsx harmony
    class ErrorBoundary extends React.Component {
      constructor(props) {
        super(props)
        this.state = { hasError: false }
      }

      componentDidCatch(error, info) {
        // You can also log the error to an error reporting service
        logErrorToMyService(error, info)
      }

      static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

      render() {
        if (this.state.hasError) {
          // You can render any custom fallback UI
          return <h1>{'Something went wrong.'}</h1>
        }
        return this.props.children
      }
    }
    ```

    그런 다음 일반 컴포넌트를 사용하면 된다.

    ```jsx harmony
    <ErrorBoundary>
      <MyWidget />
    </ErrorBoundary>
    ```

55. ### React v15에서는 어떻게 error boundaries 조작하나?

    React v15에서는 `unstable_handleError` 메서드를 사용하여 *error boundaries* 에 대한 매우 기본적인 지원을 제공한다. React v16에서 `componentDidCatch`로 이름이 변경되었다.

56. ### 정적 타입 검사에 권장되는 방법은?

    일반적으로 우리는 React 애플리케이션에서 *타입 검사*를 위해 *PropTypes 라이브러리*를 사용한다. (React v15.5 이후 `React.PropTypes`는 `prop-types` 패키지로 옮겨짐.) 큰 코드 기반의 경우, 컴파일 타임에 타입검사를 하고 자동 완성 기능을 제공하는 Flow나 TypeScript 같은 *정적 타입 검사기*를 사용하는 것이 좋다.

57. ### `react-dom` 패키지 사용법은?

    `react-dom` 패키지는 앱의 최상위 레벨에서 사용할 수 있는 *DOM-관련 메서드*를 제공한다. 대부분의 컴포넌트는 이 모듈을 사용할 필요가 없다. 이 패키지의 일부 메서드는 아래와 같다.

    1. `render()`
    2. `hydrate()`
    3. `unmountComponentAtNode()`
    4. `findDOMNode()`
    5. `createPortal()`

58. ### `react-dom`의 render 메서드란?

    이 메서드는 React 엘리먼트를 제공된 컨테이너의 DOM에 렌더링하고 컴포넌트에 대한 참조를 반환하는 데 사용된다. React 엘리먼트가 이전에 컨테이너로 렌더링 된 경우, 해당 엘리먼트에 대한 업데이트를 수행하고 필요에 따라 최신 변경 사항을 반영하기 위해 DOM을 변경한다.

    ```
    ReactDOM.render(element, container[, callback])
    ```

    선택적 콜백이 제공되면, 컴포넌트가 렌더링 되거나 업데이트 됐을 때 실행된다.

59. ### ReactDOMServer란?

    `ReactDOMServer` 객체를 사용하면 컴포넌트를 정적 마크업(일반적으로 노드 서버에서 사용한다.)으로 렌더링할 수 있다. 이 객체는 주로 *서버 사이드 렌더링*(SSR) 에 사용된다. 아래의 메서드들은 서버와 브라우저 환경에서 모두 사용할 수 있다.

    1. `renderToString()`
    2. `renderToStaticMarkup()`

    예를 들어, 일반적으로 Express, Hapi, 또는 Koa와 같은 노드 기반 웹 서버를 실행하고 `renderToString`를 호출하여 루트 컴포넌트를 문자열로 렌더링한 다음 응답으로 보낸다. 

    ```javascript
    // using Express
    import { renderToString } from 'react-dom/server'
    import MyPage from './MyPage'

    app.get('/', (req, res) => {
      res.write('<!DOCTYPE html><html><head><title>My Page</title></head><body>')
      res.write('<div id="content">')
      res.write(renderToString(<MyPage/>))
      res.write('</div></body></html>')
      res.end()
    })
    ```

60. ### React에서 innerHTML를 사용하는 방법?

    `dangerouslySetInnerHTML`는 브라우저 DOM에서 `innerHTML`를 사용하기 위한 React의 대체 속성이다. `innerHTML`과 같이, 크로스-사이트 스크립팅(XSS) 공격을 고려하여 이 속성을 사용하는 것은 위험하다. `__html` 객체를 키로 전달하고 HTML 텍스트를 값으로 전달하면 된다.

    이 예제에서 MyComponent는 HTML 마크업 설정을 위해 `dangerouslySetInnerHTML` 속성을 사용한다.

    ```jsx harmony
    function createMarkup() {
      return { __html: 'First &middot; Second' }
    }

    function MyComponent() {
      return <div dangerouslySetInnerHTML={createMarkup()} />
    }
    ```

61. ### React에서 스타일을 사용하는 방법?

    `style` 속성은 CSS 문자열 대신에 camelCased 속성이 있는 JavaScript 객체를 사용한다. 이것은 DOM 스타일 JavaScript 속성과 일치하며, 보다 효율적이고, XSS 보안 취약점을 방지한다.

    ```jsx harmony
    const divStyle = {
      color: 'blue',
      backgroundImage: 'url(' + imgUrl + ')'
    };

    function HelloWorldComponent() {
      return <div style={divStyle}>Hello World!</div>
    }
    ```

    스타일 키는 JavaScript에서 DOM 노드의 속성(e.g. `node.style.backgroundImage`)에 액세스하는 것과 일관성을 유지하기 위해서 camelCased로 작성한다.

62. ### React에서 이벤트가 어떻게 다른가?

    React 엘리먼트의 이벤트 처리에는 다음과 같은 문법적 차이가 있다.

    1. React 이벤트 핸들러는 소문자가 아닌 camelCase를 사용하여 명명된다.
    2. JSX에서는 문자열이 아닌 이벤트 핸들러로 함수를 전달한다.

63. ### 생성자에서 `setState()`를 사용하면 어떻게 되나?

    `setState()`를 사용하면, React에 객체 state를 할당하는 것과 별개로 컴포넌트와 모든 자식을 리렌더링한다. 다음과 같은 오류가 발생한다. *Can only update a mounted or mounting component.* 그래서 `this.state`를 사용하여 생성자 내부의 변수를 초기화해야 한다.

64. ### 키로 인덱스를 사용하면?

    React가 엘리먼트를 추적할 수 있도록 키는 안정적이고 예측 가능하며 고유해야 한다.

    아래의 코드 조각에서 각 엘리먼트의 키는 표현되는 데이터에 묶이지 않고 순서를 기반으로 한다. 이것은 React가 할 수 있는 최적화를 제한한다.

    ```jsx harmony
    {todos.map((todo, index) =>
      <Todo
        {...todo}
        key={index}
      />
    )}
    ```

    유니크한 키에 엘리먼트 데이터를 사용하는 경우, todo.id가 이 목록에서 유일하고 안정적이라고 가정하면, React는 요소를 재평가 할 필요없이 엘리먼트를 재정렬 할 수 있다.

    ```jsx harmony
    {todos.map((todo) =>
      <Todo {...todo}
        key={todo.id} />
    )}
    ```

65. ### `componentWillMount()` 메서드에서 `setState()`를 사용하는 것은 좋은가?

    `componentWillMount()` 라이프 사이클 메서드에서 비동기 초기화를 하지 않는게 좋다. `componentWillMount()`는 마운트가 발생하기 직전에 호출된다. `render()` 전에 호출되기 때문에 메서드에서 state를 설정하면 리렌더링 되지 않는다. 다음과 같은 메서드로 사이드 이펙트나 구독을 피하면된다. `componentWillMount()` 대신에 `componentDidMount()`에서 컴포넌트 초기화에 대한 비동기 호출을 한다.
 
    ```jsx harmony
    componentDidMount() {
      axios.get(`api/todos`)
        .then((result) => {
          this.setState({
            messages: [...result.data]
          })
        })
    }
    ```

66. ### 초기 state에 props를 사용하면 어떻게 되나?

    컴포넌트를 새로 고침 없이 컴포넌트의 props를 변경하면, 생성자 함수가 절대로 컴포넌트의 현재 state를 업데이트하지 않으므로 새로운 props 값이 표시되지 않는다. props로 state 초기화하는 것은 컴포넌트가 처음 만들어질 때만 실행된다. 

    아래의 컴포넌트는 업데이트된 입력값을 표시하지 않는다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          records: [],
          inputValue: this.props.inputValue
        };
      }

      render() {
        return <div>{this.state.inputValue}</div>
      }
    }
    ```

    render 메서드 안에서 props를 사용하면 값이 업데이트된다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          record: []
        }
      }

      render() {
        return <div>{this.props.inputValue}</div>
      }
    }
    ```

67. ### 컴포넌트를 조건부로 렌더링하는 방법?

    경우에 따라 일부 state에 따라 다른 컴포넌트를 렌더링하려고 한다. JSX는 `false` 또는 `undefined`를 렌더링하지 않아 조건부 *단락*을 사용하여 특정 조건이 true인 경우에만 컴포넌트의 주어진 부분을 렌더링할 수 있다.

    ```jsx harmony
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address &&
          <p>{address}</p>
        }
      </div>
    )
    ```

    `if-else` 조건이 필요하면 *삼항 연산자*를 사용하면 된다.

    ```jsx harmony
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address
          ? <p>{address}</p>
          : <p>{'Address is not available'}</p>
        }
      </div>
    )
    ```

68. ### DOM 엘리먼트에서 spread props를 조심해야하는 이유는?

    *spread props* 를 사용할 때 알 수 없는 HTML 속성을 추가할 위험이 있다. 이는 나쁜 습관이다. 대신 우리는 `...rest` 연산자로 props destructuring을 사용할 수 있으므로, 필요한 props만 추가할 수 있다. 예를 들어,

    ```jsx harmony
    const ComponentA = () =>
      <ComponentB isDisplay={true} className={'componentStyle'} />

    const ComponentB = ({ isDisplay, ...domProps }) =>
      <div {...domProps}>{'ComponentB'}</div>
    ```

69. ### React에서 데코레이터를 사용하는 방법?

    컴포넌트를 함수로 전달하는 것과 동일하게, *class* 컴포넌트를 *꾸밀 수* 있다. **데코레이터**는 컴포넌트 기능을 수정하는 유연하고 읽기 쉬운 방법이다.

    ```jsx harmony
    @setTitle('Profile')
    class Profile extends React.Component {
        //....
    }

    /*
      title은 문서 제목으로 설정될 문자열이다.
      WrappedComponent는 우리의 데코레이터가 위의 예제에서 볼 수 있듯이 컴포넌트 클래스 바로 위에 놓는다.
    */
    const setTitle = (title) => (WrappedComponent) => {
      return class extends React.Component {
        componentDidMount() {
          document.title = title
        }

        render() {
          return <WrappedComponent {...this.props} />
        }
      }
    }
    ```

    **Note:** 데코레이터는 ES7에 포함되지 않았지만, 현재 *stage 2 proposal*이다.

70. ### 컴포넌트를 어떻게 메모하나?

    함수형 컴포넌트에 사용할 수 있는 메모 라이브러리가 있다. 예를 들어 `moize` 라이브러리는 다른 컴포넌트에 컴포넌트를 메모할 수 있다.

    ```jsx harmony
    import moize from 'moize'
    import Component from './components/Component' // this module exports a non-memoized component

    const MemoizedFoo = moize.react(Component)

    const Consumer = () => {
      <div>
        {'I will memoize the following entry:'}
        <MemoizedFoo/>
      </div>
    }
    ```

71. ### Server Side Rendering 또는 SSR 구현방법?

    React는 이미 노드 서버에서 렌더링을 처리할 수 있도록 준비되어 있다. DOM 렌더러의 특수 버전을 사용할 수 있으며 클라이언트 측과 동일한 패턴을 따른다.

    ```jsx harmony
    import ReactDOMServer from 'react-dom/server'
    import App from './App'

    ReactDOMServer.renderToString(<App />)
    ```

    이 메서드는 일반 HTML을 문자열로 출력하며, 서버 응답의 일부로 페이지 본문 내에 배치할 수 있다. 클라이언트 측에서 React는 사전 렌더링된 컨텐츠를 탐지하고 중단된 부분을 완벽하게 파악한다.

72. ### React에서 production 모드를 사용하는 방법?

    Webpack의 `DefinePlugin` 메서드를 사용해서 `NODE_ENV`를 `production` 환경으로 설정해야 propType 유효성 검사 및 추가 경고와 같은 사항을 제거할 수 있다. 이와는 별개로, Uglify의 개발 코드와 주석을 제거하는 데드 코드(dead-code) 제거 기능을 사용하여 번들 크기를 크게 줄일 수 있다.

73. ### CRA란 무엇이며 장점은?

    `create-react-app` CLI 툴은 별도의 구성단계 없이 빠르게 React 애플리케이션을 만들고 실행할 수 있다.

    *CRA*로 Todo 앱을 만들어보자

    ```console
    # Installation
    $ npm install -g create-react-app

    # Create new project
    $ create-react-app todo-app
    $ cd todo-app

    # Build, test and run
    $ npm run build
    $ npm run test
    $ npm start
    ```
    React 앱을 제작하는 데 필요한 모든 것이 포함되어 있다.

    1. React, JSX, ES6, 및 Flow 문법 지원.
    2. object spread operator와 같은 ES6를 넘어선 언어 확장 기능.
    3. 자동 접두어가 붙은 CSS로, -webkit- 이나 다른 접두사는 필요 없다.
    4. coverage를 지원하는 내장된 빠른 대화형 단위 테스트 러너.
    5. 일반적인 실수에 대해서 경고하는 라이브 개발 서버.
    6. hashes와 sourcemaps을 사용하여 production 용 JS, CSS 및 images를 묶는 빌드 스크립트

74. ### 마운팅의 라이프 사이클 메서드 순서는?

    라이프 사이클 메서드는 컴포넌트 인스턴스가 생성되어 DOM에 삽입될 때 다음과 같은 순서로 호출된다.

    1. `constructor()`
    2. `static getDerivedStateFromProps()`
    3. `render()`
    4. `componentDidMount()`

75. ### React v16에서 더 이상 사용되지 않는 라이프 사이클 메서드는?

    다음 라이프 사이클 메소드는 안전하지 않은 코딩 방법이며 비동기 렌더링에서는 더욱 문제 될 것이다.

    1. `componentWillMount()`
    2. `componentWillReceiveProps()`
    3. `componentWillUpdate()`

    React v16.3에서 위의 메서드들은 `UNSAFE_` 접두어가 별칭으로 붙어주기 시작했으며, React v17에서 접두어가 없는 버전은 제거된다.

76. ### getDerivedStateFromProps() 라이프 사이클 메서드의 사용 목적은?

    새로운 정적 `getDerivedStateFromProps()` 라이프 사이클 메서드는 컴포넌트가 인스턴스화된 후뿐만 아니라 리렌더링 되기 전에 호출된다. update state를 object로 돌려줄 수도 있고, 새로운 props가 state 업데이트를 하지 않아도 되는 것을 나타내기 위해 `null`을 리턴할 수 있다.

    ```javascript
    class MyComponent extends React.Component {
      static getDerivedStateFromProps(props, state) {
        // ...
      }
    }
    ```

    이 라이프 사이클 메서드는 `componentDidUpdate()`와 `componentWillReceiveProps()`의 모든 사용 사례를 커버한다.

77. ### getSnapshotBeforeUpdate() 라이프 사이클 메서드의 사용 목적은??

    새로운 `getSnapshotBeforeUpdate()` 라이프 사이클 메서드는 DOM 업데이트 직전에 호출된다. 이 메서드의 반환 값은 세 번째 매개 변수로 `componentDidUpdate()`에 전달된다.

    ```javascript
    class MyComponent extends React.Component {
      getSnapshotBeforeUpdate(prevProps, prevState) {
        // ...
      }
    }
    ```

    이 라이프 사이클 메서드는 `componentDidUpdate()`와 `componentWillUpdate()`의 모든 사용 사례를 커버한다.

78. ### Hooks는 렌더링 props와 고차원 컴포넌트를 대체한다?

    렌더링 props와 고차원 컴포넌트 모두 하나의 자식만 렌더링하지만, 대부분의 경우 Hooks는 트리에서 중첩을 줄임으로써 제거하는 더 간단한 방법이다.

79. ### 컴포넌트를 명명하는데 권장되는 방법은?

    `displayName`을 사용하는 대신 참조로 컴포넌트의 이름을 지정하는 것이 좋다.

    컴포넌트 명명에 `displayName`를 사용하는 경우.

    ```javascript
    export default React.createClass({
      displayName: 'TodoApp',
      // ...
    })
    ```

    **권장되는** 접근 방법:

    ```javascript
    export default class TodoApp extends React.Component {
      // ...
    }
    ```

80. ### 컴포넌트 클래스에서 권장되는 메서드 순서는?

     *마운팅*에서 *렌더링 단계*까지 *권장되는* 메서드 순서는 아래와 같다. 

    1. `static` 메서드
    2. `constructor()`
    3. `getChildContext()`
    4. `componentWillMount()`
    5. `componentDidMount()`
    6. `componentWillReceiveProps()`
    7. `shouldComponentUpdate()`
    8. `componentWillUpdate()`
    9. `componentDidUpdate()`
    10. `componentWillUnmount()`
    11. `onClickSubmit()` 또는 `onChangeDescription()`과 같은 핸들러 또는 이벤트 핸들러를 클릭. 
    12. `getSelectReason()` 또는 `getFooterContent()`와 같은 렌더링을 위한 getter 메서드
    13. `renderNavigation()` 또는 `renderProfilePicture()`와 같은 선택적 렌더링 메서드
    14. `render()`

81. ### 스위칭 컴포넌트란?

    *스위칭 컴포넌트란*는 많은 컴포넌트 중 하나를 렌더링하는 컴포넌트이다. prop 값을 컴포넌트에 매핑하려면 object를 사용해야 한다.

    예를 들어, `page` prop을 기반으로 한 다른 페이지를 표시하는 스위칭 컴포넌트.

    ```jsx harmony
    import HomePage from './HomePage'
    import AboutPage from './AboutPage'
    import ServicesPage from './ServicesPage'
    import ContactPage from './ContactPage'

    const PAGES = {
      home: HomePage,
      about: AboutPage,
      services: ServicesPage,
      contact: ContactPage
    }

    const Page = (props) => {
      const Handler = PAGES[props.page] || ContactPage

      return <Handler {...props} />
    }

    // PAGES 객체의 키는 prop 타입에서 사용되어 dev-time errors를 잡아낼 수 있다.
    Page.propTypes = {
      page: PropTypes.oneOf(Object.keys(PAGES)).isRequired
    }
    ```

82. ### 왜 setState()에 함수를 전달해야 하나?

    `setState()`가 비동기 연산이기 때문이다. 성능상 이유로 React는 state를 일괄적으로 변경한다. 그래서 `setState()`가 호출되고 state가 즉시 변경되지 않는다. 즉 `setState()` 를 호출할 때 현재 상태에 의존해서는 안 되며 그 상태가 무엇인지 확신할 수 없게 된다. 해결방법은 이전 상태를 인수로 사용하기 위해 `setState()`에 함수를 전달하는 것이다. 이렇게 하면 `setState()`의 비동기 특성으로 인해 사용자가 액세스할 때 이전 상태 값을 가져오는 문제를 피할 수 있다.

    초기 count 값은 0이라고 가정해보자. 세 번의 연속 증가 연산을 하면, 값은 1만 증가한다.

    ```javascript
    // assuming this.state.count === 0
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    // this.state.count === 1, not 3
    ```

    `setState()`에 함수를 전달하면, count는 올바르게 증가한다.

    ```javascript
    this.setState((prevState, props) => ({
      count: prevState.count + props.increment
    }))
    // this.state.count === 3 as expected
    ```

83. ### React의 strict mode란?

    `React.StrictMode`는 애플리케이션의 잠재적인 문제점을 강조 표시하는데 유용한 컴포넌트이다. `<Fragment>`와 마찬가지로, `<StrictMode>`는 특정 DOM 엘리먼트에 렌더링하지 않는다. 자손에 대한 추가 점검과 경고를 활성화한다. 이러한 점검은 *개발 모드*에만 적용이 된다.

    ```jsx harmony
    import React from 'react'

    function ExampleApplication() {
      return (
        <div>
          <Header />
          <React.StrictMode>
            <div>
              <ComponentOne />
              <ComponentTwo />
            </div>
          </React.StrictMode>
          <Footer />
        </div>
      )
    }
    ```

    위의 예제에서, *strict mode* 검사는 `<ComponentOne>`와 `<ComponentTwo>` 컴포넌트에만 적용된다.

84. ### React Mixins이란?

    *Mixins*은 공통 기능을 갖도록 컴포넌트를 완전히 분리하는 방법이다. Mixins은 **사용하지 않아야 하며** *고차원 컴포넌트*나 *데코레이터*로 대체할 수 있다.

    가장 일반적으로 사용되는 mixins은 `PureRenderMixin`이다. props와 state가 이전 props, state와 얕게 동등할 때 불필요한 리렌더링을 방지하기 위해 일부 컴포넌트에서 사용할 수도 있다.

    ```javascript
    const PureRenderMixin = require('react-addons-pure-render-mixin')

    const Button = React.createClass({
      mixins: [PureRenderMixin],
      // ...
    })
    ````
    <!-- TODO: mixins은 더이상 사용되지 않는다. -->

85. ### 왜 isMounted()가 안티 패턴이며 적절한 해결책은?

    `isMounted()`의 주요 사용 사례는 컴포넌트가 마운트 해제된 후에 `setState()`를 호출하지 않도록 경고하는 것이다.

    ```javascript
    if (this.isMounted()) {
      this.setState({...})
    }
    ```

    `setState()`를 호출하기 전에 `isMounted()`를 검사하면 경고가 제거되지만, 경고의 목적도 상실된다. 컴포넌트가 마운트 해제된 후에 참조를 보유하고 있다고 생각하기 때문에 `isMounted()`를 사용하는 것은 코드 스멜이다.

    최적의 해결책은 컴포넌트가 마운트 해제된 후에 `setState()`가 호출될 수 있는 위치를 찾아 수정하는 것이다. 이러한 상황은 컴포넌트가 일부 데이터를 기다리며, 데이터가 도착하기 전에 마운트 해제될 때 콜백으로 인해 가장 일반적으로 발생한다. 이상적으로, 콜백은 마운트 해제 전에 `componentWillUnmount()`에서 취소해야 한다.

86. ### React에서 지원되는 Pointer Events는?

    *Pointer Events*는 모든 입력 이벤트를 처리하는 통일된 방법을 제공한다. 예전에는 마우스와 각각의 이벤트 리스너가 있었지만, 요즘에는 터치스크린이나 펜이 달린 휴대전화와 같이 마우스와 관련 없는 장치가 많다. 이러한 이벤트는 *Pointer Events* 사양을 지원하는 브라우저에서만 작동한다는 것을 기억해야 한다.

    *React DOM*에서 다음 이벤트 유형을 사용할 수 있다.

    1. `onPointerDown`
    2. `onPointerMove`
    3. `onPointerUp`
    4. `onPointerCancel`
    5. `onGotPointerCapture`
    6. `onLostPointerCaptur`
    7. `onPointerEnter`
    8. `onPointerLeave`
    9. `onPointerOver`
    10. `onPointerOut`

87. ### 왜 컴포넌트의 이름은 대문자로 시작하나?

    JSX를 사용하여 컴포넌트를 렌더링하는 경우, 해당 컴포넌트의 이름은 대문자로 시작해야 한다. 그렇지 않으면 React가 인식할 수 없는 태그로 오류를 발생시킨다. 이 규칙은 HTML 요소와 SVG 태그만 소문자로 시작할 수 있기 때문에 사용된다.

    이름이 소문자로 시작하는 컴포넌트 클래스를 정의할 수 있지만 가져올 때 대문자여야 한다. 아래와 같은 소문자는 괜찮다.

    ```jsx harmony
    class myComponent extends Component {
      render() {
        return <div />
      }
    }

    export default myComponent
    ```

    다른 파일을 가져올 때 대문자로 시작해야 한다.

    ```jsx harmony
    import MyComponent from './MyComponent'
    ```

88. ### React v16에서 사용자 정의 DOM 속성을 지원하나?

    그렇다. 과거에 React는 알 수 없는 DOM 속성을 무시하곤 했다. React가 인식하지 못하는 속성을 가진 JSX를 작성했다면 React는 그냥 건너뛸 것이다. 예를 들면, 다음과 같다.

    ```jsx harmony
    <div mycustomattribute={'something'} />
    ```

    React v15로 빈 div를 DOM에 렌더링한다.

    ```html
    <div />
    ```

    React v16에서는 알 수 없는 속성이 DOM에 저장된다.

    ```html
    <div mycustomattribute='something' />
    ```

    이것은 특정 브라우저 비표준 속성을 제공하고, 새로운 DOM API를 사용하고, 라이브러리와 통합할 때 유용하다.

89. ### constructor과 getInitialState의 차이점은?

    ES6의 클래스를 사용할 때는 생성자에서 상태를 초기화하고 `React.createClass()`를 사용할 때는  `getInitialState()` 메서드를 초기화해야 한다.

    ES6 클래스 사용 시

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        this.state = { /* initial state */ }
      }
    }
    ```

    `React.createClass()` 사용 시

    ```javascript
    const MyComponent = React.createClass({
      getInitialState() {
        return { /* initial state */ }
      }
    })
    ```

    **Note:** `React.createClass()`는 더 이상 사용되지 않으며 React v16에서 제거되었다. 대신에 자바스크립트 클래스를 사용해야 한다.

90. ### setState를 호출하지 않고도 컴포넌트 리렌더링이 가능한가?

    기본적으로, 컴포넌트의 state 또는 props가 변경되면 컴포넌트가 리렌더링이 된다. `render()` 메서드가 다른 데이터에 의존하는 경우, `forceUpdate()`를 호출하여 컴포넌트의 렌더링을 다시 해야 한다는 것을 React에게 알릴 수 있다.

    ```javascript
    component.forceUpdate(callback)
    ```

    `forceUpdate()`의 사용은 피하고 `render()`의 `this.props`과 `this.state`에서 읽기만 하는 것이 좋다.

91. ### ES6 클래스를 사용하는 React에서 super()와 super(props)의 차이점은?

    `constructor()`에서 `this.props`에 접근하려면 props를 `super()` 메서드에 전달해야 한다.

    `super(props)` 사용 시:

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        console.log(this.props) // { name: 'John', ... }
      }
    }
    ```

    `super()` 사용 시:

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()
        console.log(this.props) // undefined
      }
    }
    ```

    `constructor()` 외부에서는 `this.props`에 대해서 같은 값을 표시한다.

92. ### JSX 내부에서 반복하는 방법?

    ES6 *화살표 함수* 구문과 함께 `Array.prototype.map`을 간단히 사용할 수 있다. 예를 들어, 객체의 `items` 배열은 다음과 같은 컴포넌트의 배열과 매핑된다.

    ```jsx harmony
    <tbody>
      {items.map(item => <SomeComponent key={item.id} name={item.name} />)}
    </tbody>
    ```

    `for` 반복문을 사용하여 반복할 수 없다.

    ```jsx harmony
    <tbody>
      for (let i = 0; i < items.length; i++) {
        <SomeComponent key={items[i].id} name={items[i].name} />
      }
    </tbody>
    ```

    JSX 태그가 *함수 호출*로 변환되어 표현식안에 명령문을 사용할 수 없기 때문이다. 이것은 *stage 1 proposal*에 `올라가 있기` 때문에 바뀔수 있다.

93. ### 속성 인용문에 props를 어떻게 넣나?

    React (또는 JSX)는 속성값 내부의 변수 보간을 지원하지 않는다. 아래의 표현은 작동하지 않는다.

    ```jsx harmony
    <img className='image' src='images/{this.props.image}' />
    ```

    그러나 JS 표현식을 중괄호 안에 전체 속성값으로 넣을 수 있다. 따라서, 아래 표현식이 작동한다.

    ```jsx harmony
    <img className='image' src={'images/' + this.props.image} />
    ```

    *템플릿 문자열*을 사용하면 다음과 같이 사용할 수 있다.

    ```jsx harmony
    <img className='image' src={`images/${this.props.image}`} />
    ```

94. ### 모양이 있는 React proptype array란?

    특정 모양의 컴포넌트에 객체 배열을 전달하려면 `React.PropTypes.arrayOf()`에 대한 인수로 `React.PropTypes.shape()`를 사용한다.

    ```javascript
    ReactComponent.propTypes = {
      arrayWithShape: React.PropTypes.arrayOf(React.PropTypes.shape({
        color: React.PropTypes.string.isRequired,
        fontSize: React.PropTypes.number.isRequired
      })).isRequired
    }
    ```

95. ### 클래스 속성을 조건부로 적용하는 방법은?

    따옴표 안에서 중괄호를 사용하면 문자열로 평가되기 때문에 중괄호를 사용하면 안 된다.

    ```jsx harmony
    <div className="btn-panel {this.props.visible ? 'show' : 'hidden'}">
    ```

    대신 중괄호를 바깥으로 옮겨야 한다. (클래스 이름들 사이에 공백을 넣는 것을 잊지 말아야 한다.)

    ```jsx harmony
    <div className={'btn-panel ' + (this.props.visible ? 'show' : 'hidden')}>
    ```

    *템플릿 문자열*도 작동한다.

    ```jsx harmony
    <div className={`btn-panel ${this.props.visible ? 'show' : 'hidden'}`}>
    ```

96. ### React와 ReactDOM의 차이점?

    `react` 패키지는 `React.createElement()`, `React.Component`, `React.Children`, 엘리먼트 컴포넌트 및 클래스와 관련된 기타 도우미가 포함되어 있다. 컴포넌트를 만들 때 필요한 동형 또는 보편적인 도우미라고 생각할 수 있다. `react-dom` 패키지에는 `ReactDOM.render()`가 포함되어 있고, `react-dom/server`에는 `ReactDOMServer.renderToString()`과 `ReactDOMServer.renderToStaticMarkup()`을 사용하여 *서버 사이드 렌더링*을 지원한다.

97. ### 왜 ReactDOM은 React와 분리되었나?

    React 팀은 모든 DOM 관련 기능을 *ReactDOM*이라는 별도의 라이브러리로 분리했다. React v0.14는 라이브러리가 분리된 첫 번째 릴리즈이다. `react-native`, `react-art`, `react-canvas`, `react-three` 같은 일부 패키지를 살펴보면, React의 아름다움과 본질은 브라우저나 DOM과는 관련이 없다는 것을 분명히 한다. React가 렌더링할 수 있는 더 많은 환경을 구축하기 위해, React 팀은 주 React 패키지를 `react`와 `react-dom` 두 개로 나눌 계획을 세웠다. 이는 React과 React Native의 웹 버전 간에 공유할 수 있는 컴포넌트를 작성하는 길을 열어주었다.

98. ### React 라벨 엘리먼트를 사용하는 방법은?

    표준 `for` 속성을 사용하여 텍스트 입력에 바인드된 `<label>` 엘리먼트를 렌더링하려고 하면, 해당 속성이 없는 HTML이 생성되고 콘솔에 경고가 인쇄된다.

    ```jsx harmony
    <label for={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```

    `for`는 JavaScript에서 예약된 키워드이므로, 대신 `htmlFor`을 사용해야 한다.

    ```jsx harmony
    <label htmlFor={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```

99. ### 여러 개의 인라인 스타일 객체를 결합하는 방법은?

    일반적인 React에서 사용하는 *spread 연산자*.

    ```jsx harmony
     <button style={{...styles.panel.button, ...styles.panel.submitButton}}>{'Submit'}</button>
    ```

    React Native를 사용한다면 배열 표기법을 사용할 수 있다.

    ```jsx harmony
    <button style={[styles.panel.button, styles.panel.submitButton]}>{'Submit'}</button>
    ```

100. ### 브라우저 크기를 조정할 때 뷰를 리렌더링하는 방법은?

     `componentDidMount()`에서 `resize` 이벤트를 수신하면, 크기(`너비` 및 `높이`)를 업데이트 할 수 있다. `componentWillUnmount()` 메서드에서 리스너를 제거해야 한다.

     ```javascript
     class WindowDimensions extends React.Component {
       componentWillMount() {
         this.updateDimensions()
       }

       componentDidMount() {
         window.addEventListener('resize', this.updateDimensions)
       }

       componentWillUnmount() {
         window.removeEventListener('resize', this.updateDimensions)
       }

       updateDimensions() {
         this.setState({width: $(window).width(), height: $(window).height()})
       }

       render() {
         return <span>{this.state.width} x {this.state.height}</span>
       }
     }
     ```

101. ### `setState()`와 `replaceState()` 메서드의 차이점은?

     `setState()`를 사용하면 현재 state와 이전 state가 병합된다. `replaceState()`는 현재 state를 버리고 사용자가 넣은 state로 바꾼다. Usually 어떤 이유로 이전의 모든 키를 제거해야 하는 경우가 아니면 `setState()`를 사용한다. `replaceState()`를 사용하는 대신 `setState()`에서 state를 `false`/`null`로 설정할 수도 있다.

102. ### state 변경을 인지하는 방법?

     state가 변경되면 다음의 라이프 사이클 메서드가 호출된다. 제공된 state와 props 값을 현재 state, props와 비교하여 의미 있는 것이 변경되었는지 확인할 수 있다.

     ```
     componentWillUpdate(object nextProps, object nextState)
     componentDidUpdate(object prevProps, object prevState)
     ```

103. ### React state에서 배열 엘리먼트를 제거하는 권장 방법은?

     더 나은 방법은 `Array.prototype.filter()` 메서드를 사용하는 것이다.

     예를 들어, state를 업데이트하기 위한 `removeItem()` 메서드를 생성해보자

     ```javascript
     removeItem(index) {
       this.setState({
         data: this.state.data.filter((item, i) => i !== index)
       })
     }
     ```

104. ### HTML 렌더링없이 React를 사용할 수 있나?

     최신버전 (>=16.2)에서 가능하다. 가능한 옵션은 아래와 같다.

     ```jsx harmony
     render() {
       return false
     }
     ```

     ```jsx harmony
     render() {
       return null
     }
     ```

     ```jsx harmony
     render() {
       return []
     }
     ```

     ```jsx harmony
     render() {
       return <React.Fragment></React.Fragment>
     }
     ```

     ```jsx harmony
     render() {
       return <></>
     }
     ```

     `undefined` 반환은 작동하지 않는다

105. ### React에서 JSON을 이쁘게 출력하는 방법?

     `<pre>` 태그를 사용하여 `JSON.stringify()`의 서식이 유지되도록 할 수 있다.

     ```jsx harmony
     const data = { name: 'John', age: 42 }

     class User extends React.Component {
       render() {
         return (
           <pre>
             {JSON.stringify(data, null, 2)}
           </pre>
         )
       }
     }

     React.render(<User />, document.getElementById('container'))
     ```

106. ### React에서 props를 업데이트할 수 없는 이유는?

     React 철학은 props가 *불변*이고 *하향식*이어야 한다는 것이다. 즉, 부모는 모든 props 값을 자식에게 보낼 수 있지만, 자식은 받은 props를 수정할 수 없다.

107. ### 페이지 로드 시 input 엘리먼트에 포커스를 주는 방법은?

     `input` 엘리먼트에 대한 *ref*를 생성하고 `componentDidMount()`에서 이를 사용한다.

     ```jsx harmony
     class App extends React.Component{
       componentDidMount() {
         this.nameInput.focus()
       }

       render() {
         return (
           <div>
             <input
               defaultValue={'Won\'t focus'}
             />
             <input
               ref={(input) => this.nameInput = input}
               defaultValue={'Will focus'}
             />
           </div>
         )
       }
     }

     ReactDOM.render(<App />, document.getElementById('app'))
     ```

108. ### state에서 객체를 업데이트 할 수 있는 방법은?

     1. **state와 병합 할 객체가 있는 `setState()`를 호출한다.**

         * `Object.assign()`를 사용하여 객체의 복사본을 만든다:

             ```javascript
             const user = Object.assign({}, this.state.user, { age: 42 })
             this.setState({ user })
             ```

         * *spread 연산자*를 사용한다.

             ```javascript
             const user = { ...this.state.user, age: 42 }
             this.setState({ user })
             ```

     2. **`setState()`를 함수와 같이 사용한다.**

         ```javascript
         this.setState(prevState => ({
           user: {
             ...prevState.user,
             age: 42
           }
         }))
         ```

109. ### 왜 함수가 `setState()` 객체보다 선호되는가?

     React는 여러 `setState()` 호출을 성능 향상을 위해 단일 업데이트로 일괄처리한다. `this.props`와 `this.state`가 비동기적으로 업데이트될 수 있음으로 다음 state를 계산할 때 해당 값을 신뢰해서는 안 된다.

     counter 예제는 예상대로 업데이트되지 않는다.

     ```javascript
     // Wrong
     this.setState({
       counter: this.state.counter + this.props.increment,
     })
     ```

     선호되는 접근법은 객체가 아닌 함수로 `setState()`를 호출하는 것이다. 이 함수는 첫 번째 인수로 이전 state를 받고 두 번째 인수로 업데이트가 적용된 props를 받는다.

     ```javascript
     // Correct
     this.setState((prevState, props) => ({
       counter: prevState.counter + props.increment
     }))
     ```

110. ### 브라우저 런타임에 React 버전을 어떻게 알 수 있나?

     `React.version`을 사용해서 버전을 얻을 수 있다.

     ```jsx harmony
     const REACT_VERSION = React.version

     ReactDOM.render(
       <div>{`React version: ${REACT_VERSION}`}</div>,
       document.getElementById('app')
     )
     ```

111. ### `create-react-app`에 polyfill을 포함시키는 방법은?

     1. **`core-js`에서 수동으로 가져오기**

         `polyfills.js`와 같은 파일을 만들고 root `index.js` 파일에서 import한다. `npm install core-js` 또는 `yarn add core-js`를 실행하고 특정 필수 기능을 import한다.

         ```javascript
         import 'core-js/fn/array/find'
         import 'core-js/fn/array/includes'
         import 'core-js/fn/number/is-nan'
         ```

     2. **Polyfill 서비스를 사용하기:**

         이 줄을 `index.html`에 추가, polyfill.io CDN을 사용하여 사용자 지정 브라우저 전용 polyfill을 검색한다.

         ```html
         <script src='https://cdn.polyfill.io/v2/polyfill.min.js?features=default,Array.prototype.includes'></script>
         ```

         위의 스크립트에서 `Array.prototype.includes` 기능은 기본 기능 집합에 포함되어 있지 않음으로 명시적으로 요청해야 한다.

112. ### create-react-app에서 http 대신 https를 사용하는 방법?

     `HTTPS=true` 설정만 사용하면 된다. `package.json` 스크립트 섹션을 편집할 수 있다.

     ```json
     "scripts": {
       "start": "set HTTPS=true && react-scripts start"
     }
     ```

     또는 `set HTTPS=true && npm start`를 실행하면 된다.

113. ### create-react-app에서 상대 경로 가져오기 사용을 피하는 방법?

     프로젝트 루트에 `.env`라는 파일을 만들고 경로를 import 하면 된다. 

     ```
     NODE_PATH=src/app
     ```

     개발 서버를 다시 시작하면, 상대 경로 없이 `src/app` 내부의 내용을 import 할 수 있다.

114. ### React Router용 Google 웹 로그 분석을 추가하는 방법은?

     `history` 객체에 리스너를 추가하여 각각의 페이지 view를 기록한다.

     ```javascript
     history.listen(function (location) {
       window.ga('set', 'page', location.pathname + location.search)
       window.ga('send', 'pageview', location.pathname + location.search)
     })
     ```

115. ### 매 초마다 컴포넌트를 업데이트 하는 방법은?

     변경을 감지하려면 `setInterval()`을 사용해야 하지만 오류 및 메모리 누수를 방지하려면 컴포넌트가 마운트 해제될 때 타이머를 지워야 한다.

     ```javascript
     componentDidMount() {
       this.interval = setInterval(() => this.setState({ time: Date.now() }), 1000)
     }

     componentWillUnmount() {
       clearInterval(this.interval)
     }
     ```

116. ### React에서 인라인 스타일에 벤더 접두사는 어떻게 적용하나?

     React는 *벤더 접두사*를 자동으로 **적용하지 않는다**. 벤더 접두사를 수동으로 추가해야 한다.

     ```jsx harmony
     <div style={{
       transform: 'rotate(90deg)',
       WebkitTransform: 'rotate(90deg)', // note the capital 'W' here
       msTransform: 'rotate(90deg)' // 'ms' is the only lowercase vendor prefix
     }} />
     ```

117. ### React와 ES6를 사용해서 컴포넌트를 가져오고 내보내는 방법은?

     컴포넌트를 내보내려면 default를 사용하면 된다.

     ```jsx harmony
     import React from 'react'
     import User from 'user'

     export default class MyProfile extends React.Component {
       render(){
         return (
           <User type="customer">
             //...
           </User>
         )
       }
     }
     ```

      export 지정자를 사용하면 MyProfile이 멤버가 되어 이 모듈로 내보낼 수 있으며, 다른 컴포넌트에 이름을 언급하지 않고도 가져올 수 있다. 

118. ### React 컴포넌트 이름이 대문자로 시작해야 하는 이유는?

     JSX에서 소문자 태그 이름은 HTML 태그로 간주한다. 그러나 점으로 표시된 대문자 및 소문자 태그 이름(속성 접근자)은 없다.

     1. `<component />`는 `React.createElement('component')`로 컴파일된다. (i.e, HTML tag)
     2. `<obj.component />`는 `React.createElement(obj.component)`로 컴파일된다.
     3. `<Component />`는 `React.createElement(Component)`로 컴파일된다.

119. ### 컴포넌트 생성자는 왜 한 번만 불리나?

     React의 *reconciliation* 알고리즘에서는 정반대 정보가 없다고 가정하는데, 사용자 지정 컴포넌트가 후속 렌더링의 같은 위치에 나타나면, 이전 컴포넌트와 동일 하므로 이전 인스턴스를 새로 작성하지 않고 다시 사용한다.

120. ### React에서 상수를 정의하는 방법은?

     ES7 `static` 필드를 사용하여 상수를 정의할 수 있다.

     ```javascript
     class MyComponent extends React.Component {
       static DEFAULT_PAGINATION = 10
     }
     ```

     *Static fields*는 *Class Fields* 스테이지 3 제안의 일부이다.

121. ### React에서 프로그래밍 방식으로 클릭 이벤트를 발생시키는 방법은?

     ref prop를 사용하여 콜백을 통해 기본 `HTMLInputElement` 객체에 대한 참조를 가져와서, 참조를 클래스 속성으로 저장한 다음, 해당 참조의 `HTMLElement.click` 메서드를 사용하여 이벤트 핸들러에서 클릭을 트리거 할 수 있다.

     1. render 메서드 안에서 ref를 만든다.

         ```jsx harmony
         <input ref={input => this.inputElement = input} />
         ```

     2. 이벤트 핸들러에 클릭 이벤트를 적용한다.

         ```javascript
         this.inputElement.click()
         ```

122. ### async/await를 평범한 React에서 사용할 수 있나?

     React에서 `async`/`await`을 사용하려면, *Babel* 및 [transform-async-to-generator](https://babeljs.io/docs/en/babel-plugin-transform-async-to-generator) 플러그인이 필요하다. React Native는 Babel과 변경 세트를 구성해야 한다.

123. ### React의 일반적인 폴더 구조는?

     React 프로젝트 파일 구조는 일반적으로 사용되는 2가지 방법이 있다.

     1. **기능 또는 경로별로 그룹화**

         프로젝트를 구조화하는 일반적인 방법의 하나는 기능이나 경로별로 그룹화된 CSS, JS, 및 테스트를 함께 배치하는 것이다.

         ```
         common/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ APIUtils.js
         └─ APIUtils.test.js
         feed/
         ├─ index.js
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         └─ FeedAPI.js
         profile/
         ├─ index.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         ├─ ProfileHeader.css
         └─ ProfileAPI.js
         ```

     2. **파일 타입으로 그룹화**

         프로젝트를 구조화하는 다른 보편적인 방법은 유사한 파일끼리 그룹화하는 것이다.

         ```
         api/
         ├─ APIUtils.js
         ├─ APIUtils.test.js
         ├─ ProfileAPI.js
         └─ UserAPI.js
         components/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         └─ ProfileHeader.css
         ```

124. ### 인기 애니메이션 패키지는?

     *React Transition Group*과 *React Motion*이 React 생태계에서 가장 인기 있는 애니메이션 패키지이다.

125. ### 스타일 모듈의 이점은?

     컴포넌트에서 스타일 값을 하드 코딩 하는 것은 좋지 않다. 다른 UI 컴포넌트에서 사용될 가능성이 있는 값은 자체 모듈로 뽑아내야 한다.

     예를 들어, 이러한 스타일은 별도의 컴포넌트로 뽑아낼 수 있다.

     ```javascript
     export const colors = {
       white,
       black,
       blue
     }

     export const space = [
       0,
       8,
       16,
       32,
       64
     ]
     ```

     그런 다음 다른 컴포넌트에서 개별적으로 가져온다.

     ```javascript
     import { space, colors } from './styles'
     ```

126. ### 인기있는 React-관련 linters는?

     ESLint는 인기 있는 JavaScript linter이다. 특정 코드 스타일을 분석할 수 있는 플러그인이 있다. React에서 가장 일반적으로 사용되는 패키지 중 하나는 `eslint-plugin-react` npm 패키지다. 기본적으로, 반복자에게 있는 키부터 전체 prop 타입까지 검사하는 규칙을 사용하여 가장 좋은 사례를 여러 번 확인할 것이다. 또 다른 인기 있는 플러그인은 `eslint-plugin-jsx-a11y`로, 접근성과 관련된 일반적인 문제를 해결하는 데 도움이 된다. JSX는 일반 HTML과 약간 다른 구문을 제공하기 때문에 `alt` 텍스트나 `tabindex`와 관련된 문제는 일반적인 플러그인으로 찾아낼 수 없다.

127. ### AJAX 호출하는 방법과 어느 컴포넌트 라이프 사이클 메서드에서 AJAX 호출을 해야하나?

     Axios, jQuery AJAX 및 브라우저 내장 `fetch`와 같은 AJAX libraries를 사용할 수 있다. `componentDidMount()` 라이프 사이클 메서드에서 데이터를 가져와야 한다. 데이터를 검색할 때 `setState()`를 사용하여 컴포넌트를 업데이트 할 수 있다.

     예를 들어, 직원 목록은 API에서 가져와서 로컬 state에 설정한다.

     ```jsx harmony
     class MyComponent extends React.Component {
       constructor(props) {
         super(props)
         this.state = {
           employees: [],
           error: null
         }
       }

       componentDidMount() {
         fetch('https://api.example.com/items')
           .then(res => res.json())
           .then(
             (result) => {
               this.setState({
                 employees: result.employees
               })
             },
             (error) => {
               this.setState({ error })
             }
           )
       }

       render() {
         const { error, employees } = this.state
         if (error) {
           return <div>Error: {error.message}</div>;
         } else {
           return (
             <ul>
               {employees.map(item => (
                 <li key={employee.name}>
                   {employee.name}-{employees.experience}
                 </li>
               ))}
             </ul>
           )
         }
       }
     }
     ```

128. ### render props란?

     **Render Props**는 값이 함수인 prop을 사용하여 컴포넌트 간 코드를 공유하는 간단한 기술이다. 아래의 컴포넌트는 React 엘리먼트를 반환하는 render props를 사용한다.

     ```jsx harmony
     <DataProvider render={data => (
       <h1>{`Hello ${data.target}`}</h1>
     )}/>
     ```

     React Router와 DownShift 같은 라이브러리는 이 패턴을 사용한다.

## React Router

1.   ### React Router란?

     React Router는 React 위에 구축된 강력한 라우팅 라이브러리로 URL을 페이지에 표시된 내용과 동기화된 상태로 유지하면서 애플리케이션에 새로운 화면과 플로우를 추가할 수 있다.

2.   ### React Router가 history 라이브러리와 다른점은?

     React Router는 브라우저의 `window.history`와 브라우저 해쉬 기록의 상호 작용을 처리하는 `history` 라이브러리를 감싸는 래퍼이다. 또한 모바일 히스토리를 제공하여 모바일 앱 개발(React Native) 및 Node 단위 테스트와 같이 글로벌 히스토리가 없는 환경에 유용하다.

3.   ### What are the `<Router>` components of React Router v4?

     React Router v4 provides below 3 `<Router>` components:

     1. `<BrowserRouter>`
     2. `<HashRouter>`
     3. `<MemoryRouter>`

     The above components will create *browser*, *hash*, and *memory* history instances. React Router v4 makes the properties and methods of the `history` instance associated with your router available through the context in the `router` object.

4.   ### What is the purpose of `push()` and `replace()` methods of `history`?

     A history instance has two methods for navigation purpose.

     1. `push()`
     2. `replace()`

     If you think of the history as an array of visited locations, `push()` will add a new location to the array and `replace()` will replace the current location in the array with the new one.

5.   ### How do you programmatically navigate using React Router v4?

     There are three different ways to achieve programmatic routing/navigation within components.

     1. **Using the `withRouter()` higher-order function:**

         The `withRouter()` higher-order function will inject the history object as a prop of the component. This object provides `push()` and `replace()` methods to avoid the usage of context.

         ```jsx harmony
         import { withRouter } from 'react-router-dom' // this also works with 'react-router-native'

         const Button = withRouter(({ history }) => (
           <button
             type='button'
             onClick={() => { history.push('/new-location') }}
           >
             {'Click Me!'}
           </button>
         ))
         ```

     2. **Using `<Route>` component and render props pattern:**

         The `<Route>` component passes the same props as `withRouter()`, so you will be able to access the history methods through the history prop.

         ```jsx harmony
         import { Route } from 'react-router-dom'

         const Button = () => (
           <Route render={({ history }) => (
             <button
               type='button'
               onClick={() => { history.push('/new-location') }}
             >
               {'Click Me!'}
             </button>
           )} />
         )
         ```

     3. **Using context:**

         This option is not recommended and treated as unstable API.

         ```jsx harmony
         const Button = (props, context) => (
           <button
             type='button'
             onClick={() => {
               context.history.push('/new-location')
             }}
           >
             {'Click Me!'}
           </button>
         )

         Button.contextTypes = {
           history: React.PropTypes.shape({
             push: React.PropTypes.func.isRequired
           })
         }
         ```

6.   ### How to get query parameters in React Router v4?

     The ability to parse query strings was taken out of React Router v4 because there have been user requests over the years to support different implementation. So the decision has been given to users to choose the implementation they like. The recommended approach is to use query strings library.

     ```javascript
     const queryString = require('query-string');
     const parsed = queryString.parse(props.location.search);
     ```

     You can also use `URLSearchParams` if you want something native:

     ```javascript
     const params = new URLSearchParams(props.location.search)
     const foo = params.get('name')
     ```

     You should use a *polyfill* for IE11.

7.   ### Why you get "Router may have only one child element" warning?

     You have to wrap your Route's in a `<Switch>` block because `<Switch>` is unique in that it renders a route exclusively.

     At first you need to add `Switch` to your imports:

     ```javascript
     import { Switch, Router, Route } from 'react-router'
     ```

     Then define the routes within `<Switch>` block:

     ```jsx harmony
     <Router>
       <Switch>
         <Route {/* ... */} />
         <Route {/* ... */} />
       </Switch>
     </Router>
     ```

8.   ### How to pass params to `history.push` method in React Router v4?

     While navigating you can pass props to the `history` object:

     ```javascript
     this.props.history.push({
       pathname: '/template',
       search: '?name=sudheer',
       state: { detail: response.data }
     })
     ```

     The `search` property is used to pass query params in `push()` method.

9.   ### How to implement *default* or *NotFound* page?

     A `<Switch>` renders the first child `<Route>` that matches. A `<Route>` with no path always matches. So you just need to simply drop path attribute as below

     ```jsx harmony
     <Switch>
       <Route exact path="/" component={Home}/>
       <Route path="/user" component={User}/>
       <Route component={NotFound} />
     </Switch>
     ```

10.  ### How to get history on React Router v4?

     1. Create a module that exports a `history` object and import this module across the project.

         For example, create `history.js` file:

         ```javascript
         import { createBrowserHistory } from 'history'

         export default createBrowserHistory({
           /* pass a configuration object here if needed */
         })
         ```

     2. You should use the `<Router>` component instead of built-in routers. Imported the above `history.js` inside `index.js` file:

         ```jsx harmony
         import { Router } from 'react-router-dom'
         import history from './history'
         import App from './App'

         ReactDOM.render((
           <Router history={history}>
             <App />
           </Router>
         ), holder)
         ```

     3. You can also use push method of `history` object similar to built-in history object:

         ```javascript
         // some-other-file.js
         import history from './history'

         history.push('/go-here')
         ```

11.  ### How to perform automatic redirect after login?

     The `react-router` package provides `<Redirect>` component in React Router. Rendering a `<Redirect>` will navigate to a new location. Like server-side redirects, the new location will override the current location in the history stack.

     ```javascript
     import React, { Component } from 'react'
     import { Redirect } from 'react-router'

     export default class LoginComponent extends Component {
       render() {
         if (this.state.isLoggedIn === true) {
           return <Redirect to="/your/redirect/page" />
         } else {
           return <div>{'Login Please'}</div>
         }
       }
     }
     ```

## React Internationalization

1.   ### What is React Intl?

     The *React Intl* library makes internalization in React straightforward, with off-the-shelf components and an API that can handle everything from formatting strings, dates, and numbers, to pluralization. React Intl is part of *FormatJS* which provides bindings to React via its components and API.

2.   ### What are the main features of React Intl?

     1. Display numbers with separators.
     2. Display dates and times correctly.
     3. Display dates relative to "now".
     4. Pluralize labels in strings.
     5. Support for 150+ languages.
     6. Runs in the browser and Node.
     7. Built on standards.

3.   ### What are the two ways of formatting in React Intl?

     The library provides two ways to format strings, numbers, and dates: react components or an API.

     ```jsx harmony
     <FormattedMessage
       id={'account'}
       defaultMessage={'The amount is less than minimum balance.'}
     />
     ```

     ```javascript
     const messages = defineMessages({
       accountMessage: {
         id: 'account',
         defaultMessage: 'The amount is less than minimum balance.',
       }
     })

     formatMessage(messages.accountMessage)
     ```

4.   ### How to use `<FormattedMessage>` as placeholder using React Intl?

     The `<Formatted... />` components from `react-intl` return elements, not plain text, so they can't be used for placeholders, alt text, etc. In that case, you should use lower level API `formatMessage()`. You can inject the `intl` object into your component using `injectIntl()` higher-order component and then format the message using `formatMessage()` available on that object.

     ```jsx harmony
     import React from 'react'
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => {
       const placeholder = intl.formatMessage({id: 'messageId'})
       return <input placeholder={placeholder} />
     }

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

5.   ### How to access current locale with React Intl?

     You can get the current locale in any component of your application using `injectIntl()`:

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => (
       <div>{`The current locale is ${intl.locale}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

6.   ### How to format date using React Intl?

     The `injectIntl()` higher-order component will give you access to the `formatDate()` method via the props in your component. The method is used internally by instances of `FormattedDate` and it returns the string representation of the formatted date.

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const stringDate = this.props.intl.formatDate(date, {
       year: 'numeric',
       month: 'numeric',
       day: 'numeric'
     })

     const MyComponent = ({intl}) => (
       <div>{`The formatted date is ${stringDate}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

## React Testing

1.   ### What is Shallow Renderer in React testing?

     *Shallow rendering* is useful for writing unit test cases in React. It lets you render a component *one level deep* and assert facts about what its render method returns, without worrying about the behavior of child components, which are not instantiated or rendered.

     For example, if you have the following component:

     ```javascript
     function MyComponent() {
       return (
         <div>
           <span className={'heading'}>{'Title'}</span>
           <span className={'description'}>{'Description'}</span>
         </div>
       )
     }
     ```

     Then you can assert as follows:

     ```jsx harmony
     import ShallowRenderer from 'react-test-renderer/shallow'

     // in your test
     const renderer = new ShallowRenderer()
     renderer.render(<MyComponent />)

     const result = renderer.getRenderOutput()

     expect(result.type).toBe('div')
     expect(result.props.children).toEqual([
       <span className={'heading'}>{'Title'}</span>,
       <span className={'description'}>{'Description'}</span>
     ])
     ```

2.   ### What is `TestRenderer` package in React?

     This package provides a renderer that can be used to render components to pure JavaScript objects, without depending on the DOM or a native mobile environment. This package makes it easy to grab a snapshot of the platform view hierarchy (similar to a DOM tree) rendered by a ReactDOM or React Native without using a browser or `jsdom`.

     ```jsx harmony
     import TestRenderer from 'react-test-renderer'

     const Link = ({page, children}) => <a href={page}>{children}</a>

     const testRenderer = TestRenderer.create(
       <Link page={'https://www.facebook.com/'}>{'Facebook'}</Link>
     )

     console.log(testRenderer.toJSON())
     // {
     //   type: 'a',
     //   props: { href: 'https://www.facebook.com/' },
     //   children: [ 'Facebook' ]
     // }
     ```

3.   ### What is the purpose of ReactTestUtils package?

     *ReactTestUtils* are provided in the `with-addons` package and allow you to perform actions against a simulated DOM for the purpose of unit testing.

4.   ### What is Jest?

     *Jest* is a JavaScript unit testing framework created by Facebook based on Jasmine and provides automated mock creation and a `jsdom` environment. It's often used for testing components.

5.   ### What are the advantages of Jest over Jasmine?

     There are couple of advantages compared to Jasmine:

     - Automatically finds tests to execute in your source code.
     - Automatically mocks dependencies when running your tests.
     - Allows you to test asynchronous code synchronously.
     - Runs your tests with a fake DOM implementation (via `jsdom`) so that your tests can be run on the command line.
     - Runs tests in parallel processes so that they finish sooner.

6.   ### Give a simple example of Jest test case

     Let's write a test for a function that adds two numbers in `sum.js` file:

     ```javascript
     const sum = (a, b) => a + b

     export default sum
     ```

     Create a file named `sum.test.js` which contains actual test:

     ```javascript
     import sum from './sum'

     test('adds 1 + 2 to equal 3', () => {
       expect(sum(1, 2)).toBe(3)
     })
     ```

     And then add the following section to your `package.json`:

     ```json
     {
       "scripts": {
         "test": "jest"
       }
     }
     ```

     Finally, run `yarn test` or `npm test` and Jest will print a result:

     ```console
     $ yarn test
     PASS ./sum.test.js
     ✓ adds 1 + 2 to equal 3 (2ms)
     ```

## React Redux

1.   ### What is flux?

     *Flux* is an *application design paradigm* used as a replacement for the more traditional MVC pattern. It is not a framework or a library but a new kind of architecture that complements React and the concept of Unidirectional Data Flow. Facebook uses this pattern internally when working with React.

     The workflow between dispatcher, stores and views components with distinct inputs and outputs as follows:

     ![flux](images/flux.png)

2.   ### What is Redux?

     *Redux* is a predictable state container for JavaScript apps based on the *Flux design pattern*. Redux can be used together with React, or with any other view library. It is tiny (about 2kB) and has no dependencies.

3.   ### What are the core principles of Redux?

     Redux follows three fundamental principles:

     1. **Single source of truth:** The state of your whole application is stored in an object tree within a single store. The single state tree makes it easier to keep track of changes over time and debug or inspect the application.
     2. **State is read-only:** The only way to change the state is to emit an action, an object describing what happened. This ensures that neither the views nor the network callbacks will ever write directly to the state.
     3. **Changes are made with pure functions:** To specify how the state tree is transformed by actions, you write reducers. Reducers are just pure functions that take the previous state and an action as parameters, and return the next state.

4.   ### What are the downsides of Redux compared to Flux?

     Instead of saying downsides we can say that there are few compromises of using Redux over Flux. Those are as follows:

     1. **You will need to learn to avoid mutations:** Flux is un-opinionated about mutating data, but Redux doesn't like mutations and many packages complementary to Redux assume you never mutate the state. You can enforce this with dev-only packages like `redux-immutable-state-invariant`, Immutable.js, or instructing your team to write non-mutating code.
     2. **You're going to have to carefully pick your packages:** While Flux explicitly doesn't try to solve problems such as undo/redo, persistence, or forms, Redux has extension points such as middleware and store enhancers, and it has spawned a rich ecosystem.
     3. **There is no nice Flow integration yet:** Flux currently lets you do very impressive static type checks which Redux doesn't support yet.

5.   ### What is the difference between `mapStateToProps()` and `mapDispatchToProps()`?

     `mapStateToProps()` is a utility which helps your component get updated state (which is updated by some other components):

     ```javascript
     const mapStateToProps = (state) => {
       return {
         todos: getVisibleTodos(state.todos, state.visibilityFilter)
       }
     }
     ```

     `mapDispatchToProps()` is a utility which will help your component to fire an action event (dispatching action which may cause change of application state):

     ```javascript
     const mapDispatchToProps = (dispatch) => {
       return {
         onTodoClick: (id) => {
           dispatch(toggleTodo(id))
         }
       }
     }
     ```

6.   ### Can I dispatch an action in reducer?

     Dispatching an action within a reducer is an **anti-pattern**. Your reducer should be *without side effects*, simply digesting the action payload and returning a new state object. Adding listeners and dispatching actions within the reducer can lead to chained actions and other side effects.

7.   ### How to access Redux store outside a component?

     Yes. You just need to export the store from the module where it created with `createStore()`. Also, it shouldn't pollute the global window object.

     ```javascript
     store = createStore(myReducer)

     export default store
     ```

8.   ### What are the drawbacks of MVW pattern?

     1. The DOM manipulation is very expensive which causes applications behaves slowly and inefficient.
     2. Due to circular dependencies, a complicated model was created around models and views.
     3. Lot of data changes happens for collaborative applications(like Google Docs).
     4. No way to do undo (travel back in time) easily without adding so much extra code.

9.   ### Are there any similarities between Redux and RxJS?

     These libraries are very different for very different purposes, but there are some vague similarities.

     Redux is a tool for managing state throughout the application. It is usually used as an architecture for UIs. Think of it as an alternative to (half of) Angular. RxJS is a reactive programming library. It is usually used as a tool to accomplish asynchronous tasks in JavaScript. Think of it as an alternative to Promises. Redux uses the Reactive paradigm because the Store is reactive. The Store observes actions from a distance, and changes itself. RxJS also uses the Reactive paradigm, but instead of being an architecture, it gives you basic building blocks, Observables, to accomplish this pattern.

10.  ### How to dispatch an action on load?

     You can dispatch an action in `componentDidMount()` method and in `render()` method you can verify the data.

     ```javascript
     class App extends Component {
       componentDidMount() {
         this.props.fetchData()
       }

       render() {
         return this.props.isLoaded
           ? <div>{'Loaded'}</div>
           : <div>{'Not Loaded'}</div>
       }
     }

     const mapStateToProps = (state) => ({
       isLoaded: state.isLoaded
     })

     const mapDispatchToProps = { fetchData }

     export default connect(mapStateToProps, mapDispatchToProps)(App)
     ```

11.  ### How to use `connect()` from React Redux?

     You need to follow two steps to use your store in your container:

     1. **Use `mapStateToProps()`:** It maps the state variables from your store to the props that you specify.
     2. **Connect the above props to your container:** The object returned by the `mapStateToProps` function is connected to the container. You can import `connect()` from `react-redux`.

         ```jsx harmony
         import React from 'react'
         import { connect } from 'react-redux'

         class App extends React.Component {
           render() {
             return <div>{this.props.containerData}</div>
           }
         }

         function mapStateToProps(state) {
           return { containerData: state.data }
         }

         export default connect(mapStateToProps)(App)
         ```

12.  ### How to reset state in Redux?

     You need to write a *root reducer* in your application which delegate handling the action to the reducer generated by `combineReducers()`.

     For example, let us take `rootReducer()` to return the initial state after `USER_LOGOUT` action. As we know, reducers are supposed to return the initial state when they are called with `undefined` as the first argument, no matter the action.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         state = undefined
       }

       return appReducer(state, action)
     }
     ```

     In case of using `redux-persist`, you may also need to clean your storage. `redux-persist` keeps a copy of your state in a storage engine. First, you need to import the appropriate storage engine and then, to parse the state before setting it to undefined and clean each storage state key.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         Object.keys(state).forEach(key => {
           storage.removeItem(`persist:${key}`)
         })

         state = undefined
       }

       return appReducer(state, action)
     }
     ```

13.  ### Whats the purpose of `at` symbol in the Redux connect decorator?

     The **@** symbol is in fact a JavaScript expression used to signify decorators. *Decorators* make it possible to annotate and modify classes and properties at design time.

     Let's take an example setting up Redux without and with a decorator.

     * **Without decorator:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         class MyApp extends React.Component {
           // ...define your main app here
         }

         export default connect(mapStateToProps, mapDispatchToProps)(MyApp)
         ```

     * **With decorator:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         @connect(mapStateToProps, mapDispatchToProps)
         export default class MyApp extends React.Component {
           // ...define your main app here
         }
         ```

     The above examples are almost similar except the usage of decorator. The decorator syntax isn't built into any JavaScript runtimes yet, and is still experimental and subject to change. You can use babel for the decorators support.

14.  ### What is the difference between React context and React Redux?

     You can use **Context** in your application directly and is going to be great for passing down data to deeply nested components which what it was designed for. Whereas **Redux** is much more powerful and provides a large number of features that the Context API doesn't provide. Also, React Redux uses context internally but it doesn't expose this fact in the public API.

15.  ### Why are Redux state functions called reducers?

     Reducers always return the accumulation of the state (based on all previous and current actions). Therefore, they act as a reducer of state. Each time a Redux reducer is called, the state and action are passed as parameters. This state is then reduced (or accumulated) based on the action, and then the next state is returned. You could *reduce* a collection of actions and an initial state (of the store) on which to perform these actions to get the resulting final state.

16.  ### How to make AJAX request in Redux?

     You can use `redux-thunk` middleware which allows you to define async actions.

     Let's take an example of fetching specific account as an AJAX call using *fetch API*:

     ```javascript
     export function fetchAccount(id) {
       return dispatch => {
         dispatch(setLoadingAccountState()) // Show a loading spinner
         fetch(`/account/${id}`, (response) => {
           dispatch(doneFetchingAccount()) // Hide loading spinner
           if (response.status === 200) {
             dispatch(setAccount(response.json)) // Use a normal function to set the received state
           } else {
             dispatch(someError)
           }
         })
       }
     }

     function setAccount(data) {
      return { type: 'SET_Account', data: data }
     }
     ```

17.  ### Should I keep all component's state in Redux store?

      Keep your data in the Redux store, and the UI related state internally in the component.

18.  ### What is the proper way to access Redux store?

     The best way to access your store in a component is to use the `connect()` function, that creates a new component that wraps around your existing one. This pattern is called *Higher-Order Components*, and is generally the preferred way of extending a component's functionality in React. This allows you to map state and action creators to your component, and have them passed in automatically as your store updates.

     Let's take an example of `<FilterLink>` component using connect:

     ```javascript
     import { connect } from 'react-redux'
     import { setVisibilityFilter } from '../actions'
     import Link from '../components/Link'

     const mapStateToProps = (state, ownProps) => ({
       active: ownProps.filter === state.visibilityFilter
     })

     const mapDispatchToProps = (dispatch, ownProps) => ({
       onClick: () => dispatch(setVisibilityFilter(ownProps.filter))
     })

     const FilterLink = connect(
       mapStateToProps,
       mapDispatchToProps
     )(Link)

     export default FilterLink
     ```

     Due to it having quite a few performance optimizations and generally being less likely to cause bugs, the Redux developers almost always recommend using `connect()` over accessing the store directly (using context API).

     ```javascript
     class MyComponent {
       someMethod() {
         doSomethingWith(this.context.store)
       }
     }
     ```

19.  ### What is the difference between component and container in React Redux?

     **Component** is a class or function component that describes the presentational part of your application.

     **Container** is an informal term for a component that is connected to a Redux store. Containers *subscribe* to Redux state updates and *dispatch* actions, and they usually don't render DOM elements; they delegate rendering to presentational child components.

20.  ### What is the purpose of the constants in Redux?

     Constants allows you to easily find all usages of that specific functionality across the project when you use an IDE. It also prevents you from introducing silly bugs caused by typos – in which case, you will get a `ReferenceError` immediately.

     Normally we will save them in a single file (`constants.js` or `actionTypes.js`).

     ```javascript
     export const ADD_TODO = 'ADD_TODO'
     export const DELETE_TODO = 'DELETE_TODO'
     export const EDIT_TODO = 'EDIT_TODO'
     export const COMPLETE_TODO = 'COMPLETE_TODO'
     export const COMPLETE_ALL = 'COMPLETE_ALL'
     export const CLEAR_COMPLETED = 'CLEAR_COMPLETED'
     ```

     In Redux you use them in two places:

     1. **During action creation:**

         Let's take `actions.js`:

         ```javascript
         import { ADD_TODO } from './actionTypes';

         export function addTodo(text) {
           return { type: ADD_TODO, text }
         }
         ```

     2. **In reducers:**

         Let's create `reducer.js`:

         ```javascript
         import { ADD_TODO } from './actionTypes'

         export default (state = [], action) => {
           switch (action.type) {
             case ADD_TODO:
               return [
                 ...state,
                 {
                   text: action.text,
                   completed: false
                 }
               ];
             default:
               return state
           }
         }
         ```

21.  ### What are the different ways to write `mapDispatchToProps()`?

     There are a few ways of binding *action creators* to `dispatch()` in `mapDispatchToProps()`. Below are the possible options:

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: () => dispatch(action())
     })
     ```

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: bindActionCreators(action, dispatch)
     })
     ```

     ```javascript
     const mapDispatchToProps = { action }
     ```

     The third option is just a shorthand for the first one.

22.  ### What is the use of the `ownProps` parameter in `mapStateToProps()` and `mapDispatchToProps()`?

     If the `ownProps` parameter is specified, React Redux will pass the props that were passed to the component into your *connect* functions. So, if you use a connected component:

     ```jsx harmony
     import ConnectedComponent from './containers/ConnectedComponent';

     <ConnectedComponent user={'john'} />
     ```

     The `ownProps` inside your `mapStateToProps()` and `mapDispatchToProps()` functions will be an object:

     ```javascript
     { user: 'john' }
     ```

     You can use this object to decide what to return from those functions.

23.  ### How to structure Redux top level directories?

     Most of the applications has several top-level directories as below:

     1. **Components**: Used for *dumb* components unaware of Redux.
     2. **Containers**: Used for *smart* components connected to Redux.
     3. **Actions**: Used for all action creators, where file names correspond to part of the app.
     4. **Reducers**: Used for all reducers, where files name correspond to state key.
     5. **Store**: Used for store initialization.

     This structure works well for small and medium size apps.

24.  ### What is redux-saga?

     `redux-saga` is a library that aims to make side effects (asynchronous things like data fetching and impure things like accessing the browser cache) in React/Redux applications easier and better.

     It is available in NPM:

     ```console
     $ npm install --save redux-saga
     ```

25.  ### What is the mental model of redux-saga?

     *Saga* is like a separate thread in your application, that's solely responsible for side effects. `redux-saga` is a redux *middleware*, which means this thread can be started, paused and cancelled from the main application with normal Redux actions, it has access to the full Redux application state and it can dispatch Redux actions as well.

26.  ### What are the differences between `call()` and `put()` in redux-saga?

     Both `call()` and `put()` are effect creator functions. `call()` function is used to create effect description, which instructs middleware to call the promise. `put()` function creates an effect, which instructs middleware to dispatch an action to the store.

     Let's take example of how these effects work for fetching particular user data.

     ```javascript
     function* fetchUserSaga(action) {
       // `call` function accepts rest arguments, which will be passed to `api.fetchUser` function.
       // Instructing middleware to call promise, it resolved value will be assigned to `userData` variable
       const userData = yield call(api.fetchUser, action.userId)

       // Instructing middleware to dispatch corresponding action.
       yield put({
         type: 'FETCH_USER_SUCCESS',
         userData
       })
     }
     ```

27.  ### What is Redux Thunk?

     *Redux Thunk* middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods `dispatch()` and `getState()` as parameters.

28.  ### What are the differences between `redux-saga` and `redux-thunk`?

     Both *Redux Thunk* and *Redux Saga* take care of dealing with side effects. In most of the scenarios, Thunk uses *Promises* to deal with them, whereas Saga uses *Generators*. Thunk is simple to use and Promises are familiar to many developers, Sagas/Generators are more powerful but you will need to learn them. But both middleware can coexist, so you can start with Thunks and introduce Sagas when/if you need them.

29.  ### What is Redux DevTools?

     *Redux DevTools* is a live-editing time travel environment for Redux with hot reloading, action replay, and customizable UI. If you don't want to bother with installing Redux DevTools and integrating it into your project, consider using Redux DevTools Extension for Chrome and Firefox.

30.  ### What are the features of Redux DevTools?

     1. Lets you inspect every state and action payload.
     2. Lets you go back in time by *cancelling* actions.
     3. If you change the reducer code, each *staged* action will be re-evaluated.
     4. If the reducers throw, you will see during which action this happened, and what the error was.
     5. With `persistState()` store enhancer, you can persist debug sessions across page reloads.

31.  ### What are Redux selectors and why to use them?

     *Selectors* are functions that take Redux state as an argument and return some data to pass to the component.

     For example, to get user details from the state:

     ```javascript
     const getUserData = state => state.user.data
     ```

32.  ### What is Redux Form?

     *Redux Form* works with React and Redux to enable a form in React to use Redux to store all of its state. Redux Form can be used with raw HTML5 inputs, but it also works very well with common UI frameworks like Material UI, React Widgets and React Bootstrap.

33.  ### What are the main features of Redux Form?

       1. Field values persistence via Redux store.
       2. Validation (sync/async) and submission.
       3. Formatting, parsing and normalization of field values.

34.  ### How to add multiple middlewares to Redux?

     You can use `applyMiddleware()`.

     For example, you can add `redux-thunk` and `logger` passing them as arguments to `applyMiddleware()`:

     ```javascript
     import { createStore, applyMiddleware } from 'redux'
     const createStoreWithMiddleware = applyMiddleware(ReduxThunk, logger)(createStore)
     ```

35.  ### How to set initial state in Redux?

     You need to pass initial state as second argument to createStore:

     ```javascript
     const rootReducer = combineReducers({
       todos: todos,
       visibilityFilter: visibilityFilter
     })

     const initialState = {
       todos: [{ id: 123, name: 'example', completed: false }]
     }

     const store = createStore(
       rootReducer,
       initialState
     )
     ```

36.  ### How Relay is different from Redux?

     Relay is similar to Redux in that they both use a single store. The main difference is that relay only manages state originated from the server, and all access to the state is used via *GraphQL* queries (for reading data) and mutations (for changing data). Relay caches the data for you and optimizes data fetching for you, by fetching only changed data and nothing more.

## React Native

1.   ### What is the difference between React Native and React?

     **React** is a JavaScript library, supporting both front end web and being run on the server, for building user interfaces and web applications.

     **React Native** is a mobile framework that compiles to native app components, allowing you to build native mobile applications (iOS, Android, and Windows) in JavaScript that allows you to use React to build your components, and implements React under the hood.

2.   ### How to test React Native apps?

     React Native can be tested only in mobile simulators like iOS and Android. You can run the app in your mobile using expo app (https://expo.io) Where it syncs using QR code, your mobile and computer should be in same wireless network.

3.   ### How to do logging in React Native?

     You can use `console.log`, `console.warn`, etc. As of React Native v0.29 you can simply run the following to see logs in the console:

     ```
     $ react-native log-ios
     $ react-native log-android
     ```

4.   ### How to debug your React Native?

     Follow the below steps to debug React Native app:

     1. Run your application in the iOS simulator.
     2. Press `Command + D` and a webpage should open up at `http://localhost:8081/debugger-ui`.
     3. Enable *Pause On Caught Exceptions* for a better debugging experience.
     4. Press `Command + Option + I` to open the Chrome Developer tools, or open it via `View` -> `Developer` -> `Developer Tools`.
     5. You should now be able to debug as you normally would.

## React supported libraries & Integration

192. ### What is reselect and how it works?

     *Reselect* is a **selector library** (for Redux) which uses *memoization* concept. It was originally written to compute derived data from Redux-like applications state, but it can't be tied to any architecture or library.

     Reselect keeps a copy of the last inputs/outputs of the last call, and recomputes the result only if one of the inputs changes. If the the same inputs are provided twice in a row, Reselect returns the cached output. It's memoization and cache are fully customizable.

193. ### What is Flow?

     *Flow* is a *static type checker* designed to find type errors in JavaScript. Flow types can express much more fine-grained distinctions than traditional type systems. For example, Flow helps you catch errors involving `null`, unlike most type systems.

194. ### What is the difference between Flow and PropTypes?

     Flow is a *static analysis tool* (static checker) which uses a superset of the language, allowing you to add type annotations to all of your code and catch an entire class of bugs at compile time. PropTypes is a *basic type checker* (runtime checker) which has been patched onto React. It can't check anything other than the types of the props being passed to a given component. If you want more flexible typechecking for your entire project Flow/TypeScript are appropriate choices.

195. ### How to use Font Awesome icons in React?

     The below steps followed to include Font Awesome in React:

     1. Install `font-awesome`:

     ```console
     $ npm install --save font-awesome
     ```

     2. Import `font-awesome` in your `index.js` file:

     ```javascript
     import 'font-awesome/css/font-awesome.min.css'
     ```

     3. Add Font Awesome classes in `className`:

     ```javascript
     render() {
       return <div><i className={'fa fa-spinner'} /></div>
     }
     ```

196. ### What is React Dev Tools?

     *React Developer Tools* let you inspect the component hierarchy, including component props and state. It exists both as a browser extension (for Chrome and Firefox), and as a standalone app (works with other environments including Safari, IE, and React Native).

     The official extensions available for different browsers or environments.
     1. **Chrome extension**
     2. **Firefox extension**
     3. **Standalone app** (Safari, React Native, etc)

197. ### Why is DevTools not loading in Chrome for local files?

     If you opened a local HTML file in your browser (`file://...`) then you must first open *Chrome Extensions* and check `Allow access to file URLs`.

198. ### How to use Polymer in React?

     1. Create a Polymer element:

         ```jsx harmony
         <link rel='import' href='../../bower_components/polymer/polymer.html' />
         Polymer({
           is: 'calender-element',
           ready: function() {
             this.textContent = 'I am a calender'
           }
         })
         ```

     2. Create the Polymer component HTML tag by importing it in a HTML document, e.g. import it in the `index.html` of your React application:

         ```html
         <link rel='import' href='./src/polymer-components/calender-element.html'>
         ```

         3. Use that element in the JSX file:

         ```javascript
         import React from 'react'

         class MyComponent extends React.Component {
           render() {
             return (
               <calender-element />
             )
           }
         }

         export default MyComponent
         ```

199. ### What are the advantages of React over Vue.js?

     React has the following advantages over Vue.js:

     1. Gives more flexibility in large apps developing.
     2. Easier to test.
     3. Suitable for mobile apps creating.
     4. More information and solutions available.

200. ### What is the difference between React and Angular?

     | React | Angular |
     | ----- | ------- |
     | React is a library and has only the View layer | Angular is a framework and has complete MVC functionality |
     | React handles rendering on the server side | AngularJS renders only on the client side but Angular 2 and above renders on the server side |
     | React uses JSX that looks like HTML in JS which can be confusing | Angular follows the template approach for HTML, which makes code shorter and easy to understand |
     | React Native, which is a React type to build mobile applications are faster and more stable | Ionic, Angular's mobile native app is relatively less stable and slower |
     | In React, data flows only in one way and hence debugging is easy | In Angular, data flows both way i.e it has two-way data binding between children and parent and hence debugging is often difficult |

201. ### Why React tab is not showing up in DevTools?

     When the page loads, *React DevTools* sets a global named `__REACT_DEVTOOLS_GLOBAL_HOOK__`, then React communicates with that hook during initialization. If the website is not using React or if React fails to communicate with DevTools then it won't show up the tab.

202. ### What are Styled Components?

     `styled-components` is a JavaScript library for styling React applications. It removes the mapping between styles and components, and lets you write actual CSS augmented with JavaScript.

203. ### Give an example of Styled Components?

     Lets create `<Title>` and `<Wrapper>` components with specific styles for each.

     ```javascript
     import React from 'react'
     import styled from 'styled-components'

     // Create a <Title> component that renders an <h1> which is centered, red and sized at 1.5em
     const Title = styled.h1`
       font-size: 1.5em;
       text-align: center;
       color: palevioletred;
     `

     // Create a <Wrapper> component that renders a <section> with some padding and a papayawhip background
     const Wrapper = styled.section`
       padding: 4em;
       background: papayawhip;
     `
     ```

     These two variables, `Title` and `Wrapper`, are now components that you can render just like any other react component.

     ```jsx harmony
     <Wrapper>
       <Title>{'Lets start first styled component!'}</Title>
     </Wrapper>
     ```

204. ### What is Relay?

     Relay is a JavaScript framework for providing a data layer and client-server communication to web applications using the React view layer.

205. ### How to use TypeScript in `create-react-app` application?

     When you create a new project supply `--scripts-version` option as `react-scripts-ts`. `react-scripts-ts` is a set of adjustments to take the standard `create-react-app` project pipeline and bring TypeScript into the mix.

     Now the project layout should look like the following:

     ```
     my-app/
     ├─ .gitignore
     ├─ images.d.ts
     ├─ node_modules/
     ├─ public/
     ├─ src/
     │  └─ ...
     ├─ package.json
     ├─ tsconfig.json
     ├─ tsconfig.prod.json
     ├─ tsconfig.test.json
     └─ tslint.json
     ```

## Miscellaneous

206. ### What are the main features of Reselect library?

       1. Selectors can compute derived data, allowing Redux to store the minimal possible state.
       2. Selectors are efficient. A selector is not recomputed unless one of its arguments changes.
       3. Selectors are composable. They can be used as input to other selectors.

207. #### Give an example of Reselect usage?

     Let's take calculations and different amounts of a shipment order with the simplified usage of Reselect:

     ```javascript
     import { createSelector } from 'reselect'

     const shopItemsSelector = state => state.shop.items
     const taxPercentSelector = state => state.shop.taxPercent

     const subtotalSelector = createSelector(
       shopItemsSelector,
       items => items.reduce((acc, item) => acc + item.value, 0)
     )

     const taxSelector = createSelector(
       subtotalSelector,
       taxPercentSelector,
       (subtotal, taxPercent) => subtotal * (taxPercent / 100)
     )

     export const totalSelector = createSelector(
       subtotalSelector,
       taxSelector,
       (subtotal, tax) => ({ total: subtotal + tax })
     )

     let exampleState = {
       shop: {
         taxPercent: 8,
         items: [
           { name: 'apple', value: 1.20 },
           { name: 'orange', value: 0.95 },
         ]
       }
     }

     console.log(subtotalSelector(exampleState)) // 2.15
     console.log(taxSelector(exampleState))      // 0.172
     console.log(totalSelector(exampleState))    // { total: 2.322 }
     ```

208. ### What is an action in Redux?

     *Actions* are plain JavaScript objects or payloads of information that send data from your application to your store. They are the only source of information for the store. Actions must have a type property that indicates the type of action being performed.

     For example an example action which represents adding a new todo item:

     ```
     {
       type: ADD_TODO,
       text: 'Add todo item'
     }
     ```

209. ### Does the statics object work with ES6 classes in React?

     No, `statics` only works with `React.createClass()`:

     ```javascript
     someComponent= React.createClass({
       statics: {
         someMethod: function() {
           // ..
         }
       }
     })
     ```

     But you can write statics inside ES6+ classes or writing them outside class as below,

     ```javascript
     class Component extends React.Component {
       static propTypes = {
         // ...
       }

       static someMethod() {
         // ...
       }
     }
     ```
     ```javascript
     class Component extends React.Component {
        ....
     }

     Component.propTypes = {...}
     Component.someMethod = function(){....}
     ```

210. ### Can Redux only be used with React?

     Redux can be used as a data store for any UI layer. The most common usage is with React and React Native, but there are bindings available for Angular, Angular 2, Vue, Mithril, and more. Redux simply provides a subscription mechanism which can be used by any other code.

211. ### Do you need to have a particular build tool to use Redux?

     Redux is originally written in ES6 and transpiled for production into ES5 with Webpack and Babel. You should be able to use it regardless of your JavaScript build process. Redux also offers a UMD build that can be used directly without any build process at all.

212. ### How Redux Form `initialValues` get updated from state?

     You need to add `enableReinitialize : true` setting.

     ```javascript
     const InitializeFromStateForm = reduxForm({
       form: 'initializeFromState',
       enableReinitialize : true
     })(UserEdit)
     ```

     If your `initialValues` prop gets updated, your form will update too.

213. ### How React PropTypes allow different types for one prop?

     You can use `oneOfType()` method of `PropTypes`.

     For example, the height property can be defined with either `string` or `number` type as below:

     ```javascript
     Component.PropTypes = {
       size: PropTypes.oneOfType([
         PropTypes.string,
         PropTypes.number
       ])
     }
     ```

214. ### Can I import an SVG file as react component?

     You can import SVG directly as component instead of loading it as a file. This feature is available with `react-scripts@2.0.0` and higher.

     ```jsx harmony
     import { ReactComponent as Logo } from './logo.svg'

     const App = () => (
       <div>
         {/* Logo is an actual react component */}
         <Logo />
       </div>
     )
     ```

     **Note**: Don't forget about the curly braces in the import.

215. ### Why are inline ref callbacks or functions not recommended?

     If the ref callback is defined as an inline function, it will get called twice during updates, first with null and then again with the DOM element. This is because a new instance of the function is created with each render, so React needs to clear the old ref and set up the new one.

     ```jsx
     class UserForm extends Component {
       handleSubmit = () => {
         console.log("Input Value is: ", this.input.value)
       }


       render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={(input) => this.input = input} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

     But our expectation is for the ref callback to get called once, when the component mounts. One quick fix is to use the ES7 class property syntax to define the function

     ```jsx
     class UserForm extends Component {
      handleSubmit = () => {
        console.log("Input Value is: ", this.input.value)
      }

      setSearchInput = (input) => {
        this.input = input
      }

      render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={this.setSearchInput} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

216. ### What is render hijacking in react?

     The concept of render hijacking is the ability to control what a component will output from another component. It actually means that you decorate your component by wrapping it into a Higher-Order component. By wrapping you can inject additional props or make other changes, which can cause changing logic of rendering. It does not actually enables hijacking, but by using HOC you make your component behave in different way.

217. ### What are HOC factory implementations?
     There are two main ways of implementing HOCs in React. 1. Props Proxy (PP) and 2. Inheritance Inversion (II). They follow different approaches for manipulating the *WrappedComponent*.

     **Props Proxy**

     In this approach, the render method of the HOC returns a React Element of the type of the WrappedComponent. We also pass through the props that the HOC receives, hence the name **Props Proxy**.

     ```jsx

     function ppHOC(WrappedComponent) {
      return class PP extends React.Component {
        render() {
          return <WrappedComponent {...this.props}/>
        }
      }
     }
     ```
     **Inheritance Inversion**

     In this approach, the returned HOC class (Enhancer) extends the WrappedComponent. It is called Inheritance Inversion because instead of the WrappedComponent extending some Enhancer class, it is passively extended by the Enhancer. In this way the relationship between them seems **inverse**.

     ```jsx
     function iiHOC(WrappedComponent) {
      return class Enhancer extends WrappedComponent {
        render() {
          return super.render()
        }
      }
     }
     ```
218. ### How to pass numbers to React component?

     You should be passing the numbers via curly braces({}) where as strings inn quotes

     ```jsx
        React.render(<User age={30} department={"IT"} />, document.getElementById('container'));
     ```
219. ### Do I need to keep all my state into Redux? Should I ever use react internal state?
     It is up to developer decision. i.e, It is developer job to determine what kinds of state make up your application, and where each piece of state should live. Some users prefer to keep every single piece of data in Redux, to maintain a fully serializable and controlled version of their application at all times. Others prefer to keep non-critical or UI state, such as “is this dropdown currently open”, inside a component's internal state.

     Below are the thumb rules to determine what kind of data should be put into Redux
     1. Do other parts of the application care about this data?
     2. Do you need to be able to create further derived data based on this original data?
     3. Is the same data being used to drive multiple components?
     4. Is there value to you in being able to restore this state to a given point in time (ie, time travel debugging)?
     5. Do you want to cache the data (ie, use what's in state if it's already there instead of re-requesting it)?

220. ### What is the purpose of registerServiceWorker in React?

     React creates a service worker for you without any configuration by default. The service worker is a web API that helps you cache your assets and other files so that when the user is offline or on slow network, he/she can still see results on the screen, as such, it helps you build a better user experience, that's what you should know about service worker's for now. It's all about adding offline capabilities to your site.

     ```jsx
        import React from 'react';
        import ReactDOM from 'react-dom';
        import App from './App';
        import registerServiceWorker from './registerServiceWorker';

        ReactDOM.render(<App />, document.getElementById('root'));
        registerServiceWorker();
     ```
221. ### What is React memo function?

     Class components can be restricted from rendering when their input props are the same using **PureComponent or shouldComponentUpdate**. Now you can do the same with function components by wrapping them in **React.memo**.
     ```jsx
     const MyComponent = React.memo(function MyComponent(props) {
      /* only rerenders if props change */
     });
     ```
222. ### What is React lazy function?
     The React.lazy function lets you render an dynamic import as a regular component. It will automatically load the bundle containing the OtherComponent when the component gets rendered. This must return a Promise which resolves to a module with a default export containing a React component.
     ```jsx
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
      return (
        <div>
          <OtherComponent />
        </div>
      );
     }
     ```
     **Note:**
     React.lazy and Suspense is not yet available for server-side rendering. If you want to do code-splitting in a server rendered app, we still recommend React Loadable.
223. ### How to prevent unnecessary updates using setState?
     You can compare current value of the state with an existing state value and decide whether to rerender the page or not. If the values are same then you need to return **null** to stop rerendering otherwise return the latest state value. For example, the user profile information is conditionally rendered as follows,
     ```jsx
     getUserProfile = user => {
       const latestAddress = user.address;
       this.setState(state => {
         if (state.address === latestAddress) {
           return null;
         } else {
           return { title: latestAddress };
         }
       });
     };
     ```
224. ### How do you render Array, Strings and Numbers in React 16 Version?
     **Arrays**: Unlike older releases, you don't need to make sure **render** method return a single element in React16. You are able to return multiple sibling elements without a wrapping element by returning an array. For example, let us take the below list of developers,
     ```jsx
     const ReactJSDevs = () => {
       return [
         <li key="1">John</li>,
         <li key="2">Jackie</li>,
         <li key="3">Jordan</li>
       ];
     }
     ```
     You can also merge this array of items in another array component
     ```jsx
     const JSDevs = () => {
       return (
         <ul>
           <li>Brad</li>
           <li>Brodge</li>
           <ReactJSDevs/>
           <li>Brandon</li>
         </ul>
       );
     }
     ```
     **Strings and Numbers:** You can also return string and number type from the render method
     ```jsx
     render() {
      return 'Welcome to ReactJS questions';
     }
     // Number
     render() {
      return 2018;
     }
     ```
225. ### How to use class field declarations syntax in React classes?
     React Class Components can be made much more concise using the class field declarations. You can initialize local state without using the constructor and declare class methods by using arrow functions without the extra need to bind them. Let's take a counter example to demonstrate class field declarations for state without using constructor and methods without binding,
     ```jsx
     class Counter extends Component {
       state = { value: 0 };

       handleIncrement = () => {
         this.setState(prevState => ({
           value: prevState.value + 1
         }));
       };

       handleDecrement = () => {
         this.setState(prevState => ({
           value: prevState.value - 1
         }));
       };

       render() {
         return (
           <div>
             {this.state.value}

             <button onClick={this.handleIncrement}>+</button>
             <button onClick={this.handleDecrement}>-</button>
           </div>
         )
       }
     }
     ```
226. ### What are hooks?
     Hooks is a new feature that lets you use state and other React features without writing a class. Let's see an example of useState hook example,
     ```jsx
     import { useState } from 'react';

     function Example() {
       // Declare a new state variable, which we'll call "count"
       const [count, setCount] = useState(0);

       return (
         <div>
           <p>You clicked {count} times</p>
           <button onClick={() => setCount(count + 1)}>
             Click me
           </button>
         </div>
       );
     }
     ```
227. ### What are the rules needs to follow for hooks?

     You need to follow two rules inorder to use hooks
     1. Call Hooks only at the top level of your react functions. i.e, You shouldn’t call Hooks inside loops, conditions, or nested functions. This will ensure that Hooks are called in the same order each time a component renders and it preserves the state of Hooks between multiple useState and useEffect calls.
     2. Call Hooks from React Functions only. i.e, You shouldn’t call Hooks from regular JavaScript functions.

228. ### How to ensure hooks followed the rules in your project?
     React team released an ESLint plugin called **eslint-plugin-react-hooks** that enforces these two rules. You can add this plugin to your project using the below command,
     ```javascript
     npm install eslint-plugin-react-hooks@next
     ```
     And apply the below config in your ESLint config file,
     ```javascript
     // Your ESLint configuration
     {
       "plugins": [
         // ...
         "react-hooks"
       ],
       "rules": {
         // ...
         "react-hooks/rules-of-hooks": "error"
       }
     }
     ```
     **Note:** This plugin is intended to use in Create React App by default.

229. ### What are the differences between Flux and Redux?
     Below are the major differences between Flux and Redux

     | Flux | Redux |
     | ----- | ------- |
     | State is mutable | State is immutable |
     | The Store contains both state and change logic | The Store and change logic are separate |
     | There are multiple stores exist | There is only one store exist |
     | All the stores are disconnected and flat | Single store with hierarchical reducers|
     | It has a singleton dispatcher | There is no concept of dispatcher |
     | React components subscribe to the store | Container components uses connect function|
230. ### What are the benefits of React Router V4?
     Below are the main benefits of React Router V4 module,
     1. In React Router v4(version 4), the API is completely about components. A router can be visualized as a single component(<BrowserRouter>) which wraps specific child router components(<Route>).
     2. You don't need to manually set history. The router module will take care history by wrapping routes with  <BrowserRouter> component.
     3. The application size is reduced by adding only the specific router module(Web, core, or native)
231. ### Can you describe about componentDidCatch lifecycle method signature?
     The **componentDidCatch** lifecycle method is invoked after an error has been thrown by a descendant component. The method receives two parameters,
     1. error: - The error object which was thrown
     2. info: - An object with a componentStack key contains the information about which component threw the error.

     The method structure would be as follows
     ```javascript
     componentDidCatch(error, info)
     ```
232. ### In which scenarios error boundaries do not catch errors?
     Below are the cases in which error boundaries doesn't work
     1. Inside Event handlers
     2. Asynchronous code using **setTimeout or requestAnimationFrame** callbacks
     3. During Server side rendering
     4. When errors thrown in the error boundary code itself
233. ### Why do not you need error boundaries for event handlers?
     Error boundaries do not catch errors inside event handlers. Event handlers don't happened or invoked during rendering time unlike render method or lifecycle methods. So React knows how to recover these kind of errors in event handlers.
     If still you need to catch an error inside event handler, use the regular JavaScript try / catch statement as below
     ```javascript
     class MyComponent extends React.Component {
       constructor(props) {
         super(props);
         this.state = { error: null };
       }

       handleClick = () => {
         try {
           // Do something that could throw
         } catch (error) {
           this.setState({ error });
         }
       }

       render() {
         if (this.state.error) {
           return <h1>Caught an error.</h1>
         }
         return <div onClick={this.handleClick}>Click Me</div>
       }
     }
     ```
     The above code is catching the error using vanilla javascript try/catch block instead of error boundaries.
234. ### What is the difference between try catch block and error boundaries?
     Try catch block works with imperative code whereas error boundaries are meant for declarative code to render on the screen.
     For example, the try catch block used for below imperative code
     ```javascript
     try {
       showButton();
     } catch (error) {
       // ...
     }
     ```
     Whereas error boundaries wrap declarative code as below,
     ```javascript
     <ErrorBoundary>
       <MyComponent />
     </ErrorBoundary>
     ```
     So if an error occurs in a **componentDidUpdate** method caused by a **setState** somewhere deep in the tree, it will still correctly propagate to the closest error boundary.

235. ### What is the behavior of uncaught errors in react 16?
     In React 16, errors that were not caught by any error boundary will result in unmounting of the whole React component tree. The reason behind this decision is that it is worse to leave corrupted UI in place than to completely remove it. For example, it is worse for a payments app to display a wrong amount than to render nothing.
236. ### What is the proper placement for error boundaries?
     The granularity of error boundaries usage is up to the developer based on project needs. You can follow either of these approaches,
     1. You can wrap top-level route components to display a generic error message for the entire application.
     2. You can also wrap individual components in an error boundary to protect them from crashing the rest of the application.
237. ### What is the benefit of component stack trace from error boundary?
     Apart from error messages and javascript stack, React16 will display the component stack trace with file names and line numbers using error boundary concept. For example, BuggyCounter component displays the component stack trace as below,

     ![stacktrace](images/error_boundary.png)

238. ### What is the required method to be defined for a class component?
     The render() method is the only required method in a class component. i.e, All methods other than render method are optional for a class component.
239. ### What are the possible return types of render method?
     Below are the list of following types used and return from render method,
     1. **React elements:** Elements that instruct React to render a DOM node. It includes html elements such as `<div/>` and user defined elements.
     2. **Arrays and fragments:** Return multiple elements to render as Arrays and Fragments to wrap multiple elements
     3. **Portals:** Render children into a different DOM subtree.
     4. **String and numbers:** Render both Strings and Numbers as text nodes in the DOM
     5. **Booleans or null:** Doesn't render anything but these types are used to conditionally render content.

240. ### What is the main purpose of constructor?
     The constructor is mainly used for two purposes,
     1. To initialize local state by assigning object to this.state
     2. For binding event handler methods to the instance
     For example, the below code covers both the above cases,
     ```javascript
     constructor(props) {
       super(props);
       // Don't call this.setState() here!
       this.state = { counter: 0 };
       this.handleClick = this.handleClick.bind(this);
     }
     ```
241. ### Is it mandatory to define constructor for React component?
     No, it is not mandatory. i.e, If you don’t initialize state and you don’t bind methods, you don’t need to implement a constructor for your React component.
242. ### What are default props?
     The defaultProps are defined as a property on the component class to set the default props for the class. This is used for undefined props, but not for null props. For example, let us create color default prop for the button component,
     ```javascript
     class MyButton extends React.Component {
       // ...
     }

     MyButton.defaultProps = {
       color: 'red'
     };

     ```

     If props.color is not provided then it will set the default value to 'red'. i.e, Whenever you try to access the color prop it uses default value
     ```javascript
     render() {
        return <MyButton /> ; // props.color will be set to red
      }
     ```
     **Note:** If you provide null value then it remains null value.
243. ### Why should not call setState in componentWillUnmount?
     You should not call setState() in componentWillUnmount() because Once a component instance is unmounted, it will never be mounted again.
244. ### What is the purpose of getDerivedStateFromError?
     This lifecycle method is invoked after an error has been thrown by a descendant component. It receives the error that was thrown as a parameter and should return a value to update state. The signature of the lifecycle method is as follows,
     ```javascript
     static getDerivedStateFromError(error)
     ```
     Let us take error boundary use case with the above lifecycle method for demonistration purpose,
     ```javascript
     class ErrorBoundary extends React.Component {
       constructor(props) {
         super(props);
         this.state = { hasError: false };
       }

       static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

       render() {
         if (this.state.hasError) {
           // You can render any custom fallback UI
           return <h1>Something went wrong.</h1>;
         }

         return this.props.children;
       }
     }
     ```
245. ### What is the methods order when component re-rendered?
     An update can be caused by changes to props or state. The below methods are called in the following order when a component is being re-rendered.
     1. static getDerivedStateFromProps()
     2. shouldComponentUpdate()
     3. render()
     4. getSnapshotBeforeUpdate()
     5. componentDidUpdate()

246. ### What are the methods invoked during error handling?
     Below methods are called when there is an error during rendering, in a lifecycle method, or in the constructor of any child component.
     1. static getDerivedStateFromError()
     2. componentDidCatch()
247. ### What is the purpose of displayName class property?
     The displayName string is used in debugging messages. Usually, you don’t need to set it explicitly because it’s inferred from the name of the function or class that defines the component. You might want to set it explicitly if you want to display a different name for debugging purposes or when you create a higher-order component.
     For example, To ease debugging, choose a display name that communicates that it’s the result of a withSubscription HOC.
     ```javascript
     function withSubscription(WrappedComponent) {
       class WithSubscription extends React.Component {/* ... */}
       WithSubscription.displayName = `WithSubscription(${getDisplayName(WrappedComponent)})`;
       return WithSubscription;
     }
     function getDisplayName(WrappedComponent) {
       return WrappedComponent.displayName || WrappedComponent.name || 'Component';
     }
     ```
248. ### What is the browser support for react applications?
     React supports all popular browsers, including Internet Explorer 9 and above, although some polyfills are required for older browsers such as IE 9 and IE 10. If you use  **es5-shim and es5-sham** polyfill then it even support old browsers that doesn't support ES5 methods.
249. ### What is the purpose of unmountComponentAtNode method?
     This method is available from react-dom package and it removes a mounted React component from the DOM and clean up its event handlers and state. If no component was mounted in the container, calling this function does nothing. Returns true if a component was unmounted and false if there was no component to unmount.
     The method signature would be as follows,
     ```javascript
     ReactDOM.unmountComponentAtNode(container)
     ```
250. ### What is code-splitting?
     Code-Splitting is a feature supported by bundlers like Webpack and Browserify which can create multiple bundles that can be dynamically loaded at runtime. The react project supports code splitting via dynamic import() feature.
     For example, in the below code snippets, it will make moduleA.js and all its unique dependencies as a separate chunk that only loads after the user clicks the 'Load' button.
     **moduleA.js**
     ```javascript
     const moduleA = 'Hello';

     export { moduleA };
     ```
     **App.js**
     ```javascript
     import React, { Component } from 'react';

     class App extends Component {
       handleClick = () => {
         import('./moduleA')
           .then(({ moduleA }) => {
             // Use moduleA
           })
           .catch(err => {
             // Handle failure
           });
       };

       render() {
         return (
           <div>
             <button onClick={this.handleClick}>Load</button>
           </div>
         );
       }
     }

     export default App;

     ```
251. ### What is the benefit of strict mode?
     The <StrictMode> will be  helpful in the below cases

     1. Identifying components with **unsafe lifecycle methods**.
     2. Warning about **legacy string ref** API usage.
     3. Detecting unexpected **side effects**.
     4. Detecting **legacy context** API.
     5. Warning about deprecated findDOMNode usage
252. ### What are Keyed Fragments?
     The Fragments declared with the explicit <React.Fragment> syntax may have keys. The general usecase is mapping a collection to an array of fragments as below,
     ```javascript
     function Glossary(props) {
       return (
         <dl>
           {props.items.map(item => (
             // Without the `key`, React will fire a key warning
             <React.Fragment key={item.id}>
               <dt>{item.term}</dt>
               <dd>{item.description}</dd>
             </React.Fragment>
           ))}
         </dl>
       );
     }
     ```
     **Note:** key is the only attribute that can be passed to Fragment. In the future, there might be a support for additional attributes, such as event handlers.
253. ### Is it React support all HTML attributes?
     As of React 16, both standard or custom DOM attributes are fully supported. Since React components often take both custom and DOM-related props, React uses the camelCase convention just like the DOM APIs. Let us take few props with respect to standard HTML attributes,
     ```javascript
     <div tabIndex="-1" />      // Just like node.tabIndex DOM API
     <div className="Button" /> // Just like node.className DOM API
     <input readOnly={true} />  // Just like node.readOnly DOM API
     ```
     These props work similarly to the corresponding HTML attributes, with the exception of the special cases. It also support all SVG attributes.
254. ### What are the limitations with HOCs?

     Higher-order components come with a few caveats apart from its benefits. Below are the few listed in an order
     1. **Don’t Use HOCs Inside the render Method:**
        It is not recommended to apply a HOC to a component within the render method of a component.
        ```javascript
        render() {
          // A new version of EnhancedComponent is created on every render
          // EnhancedComponent1 !== EnhancedComponent2
          const EnhancedComponent = enhance(MyComponent);
          // That causes the entire subtree to unmount/remount each time!
          return <EnhancedComponent />;
        }
        ```
        The above code impact performance by remounting a component that causes the state of that component and all of its children to be lost. Instead, apply HOCs outside the component definition so that the resulting component is created only once
     2. **Static Methods Must Be Copied Over:**
        When you apply a HOC to a component the new component does not have any of the static methods of the original component
        ```javascript
        // Define a static method
        WrappedComponent.staticMethod = function() {/*...*/}
        // Now apply a HOC
        const EnhancedComponent = enhance(WrappedComponent);

        // The enhanced component has no static method
        typeof EnhancedComponent.staticMethod === 'undefined' // true
        ```
        You can overcome this by copying the methods onto the container before returning it
        ```javascript
        function enhance(WrappedComponent) {
          class Enhance extends React.Component {/*...*/}
          // Must know exactly which method(s) to copy :(
          Enhance.staticMethod = WrappedComponent.staticMethod;
          return Enhance;
        }
        ```
     3. **Refs Aren’t Passed Through:**
        For HOCs you need to pass through all props to the wrapped component but this does not work for refs. This is because ref is not really a prop similar to key. In this case you need to use the React.forwardRef API
255. ### How to debug forwardRefs in DevTools?

     **React.forwardRef** accepts a render function as parameter and DevTools uses this function to determine what to display for the ref forwarding component. For example, If you don't name the render function or not using displayName property then it will appear as ”ForwardRef” in the DevTools,
     ```javascript
     const WrappedComponent = React.forwardRef((props, ref) => {
       return <LogProps {...props} forwardedRef={ref} />;
     });
     ```
     But If you name the render function then it will appear as **”ForwardRef(myFunction)”**
     ```javascript
     const WrappedComponent = React.forwardRef(
       function myFunction(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }
     );
     ```
     As an alternative, You can also set displayName property for forwardRef function,
     ```javascript
     function logProps(Component) {
       class LogProps extends React.Component {
         // ...
       }

       function forwardRef(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }

       // Give this component a more helpful display name in DevTools.
       // e.g. "ForwardRef(logProps(MyComponent))"
       const name = Component.displayName || Component.name;
       forwardRef.displayName = `logProps(${name})`;

       return React.forwardRef(forwardRef);
     }
     ```
256. ### When component props defaults to true?
     If you pass no value for a prop, it defaults to true. This behavior is available so that it matches the behavior of HTML. For example, below expressions are equivalent,
     ```javascript
     <MyInput autocomplete />

     <MyInput autocomplete={true} />
     ```
     **Note:** It is not recommend using this approach because it can be confused with the ES6 object shorthand (example, {name} which is short for {name: name})
257. ### What is NextJS and major features of it?
     Next.js is a popular and lightweight framework for static and server‑rendered applications built with React. It also provides styling and routing solutions. Below are the major features provided by NextJS,
     1. Server-rendered by default
     2. Automatic code splitting for faster page loads
     3. Simple client-side routing (page based)
     4. Webpack-based dev environment which supports (HMR)
     5. Able to implement with Express or any other Node.js HTTP server
     6. Customizable with your own Babel and Webpack configurations
258. ### How do you pass an event handler to a component?
     You can pass event handlers and other functions as props to child components. It can be used in child component as  below,
     ```
     <button onClick={this.handleClick}>
     ```
259. ### Is it good to use arrow functions in render methods?
     Yes, You can use. It is often the easiest way to pass parameters to callback functions. But you need to optimize the performance while using it.
     ```javascript
     class Foo extends Component {
       handleClick() {
         console.log('Click happened');
       }
       render() {
         return <button onClick={() => this.handleClick()}>Click Me</button>;
       }
     }
     ```
     **Note:** Using an arrow function in render method creates a new function each time the component renders, which may have performance implications
260. ### How to prevent a function from being called multiple times?
     If you use an event handler such as **onClick or onScroll** and want to prevent the callback from being fired too quickly, then you can limit the rate at which callback is executed. This can be achieved in the below possible ways,
     1. **Throttling:** Changes based on a time based frequency. For example, it can be used using _.throttle lodash function
     2. **Debouncing:** Publish changes after a period of inactivity. For example, it can be used using _.debounce lodash function
     3. **RequestAnimationFrame throttling:** Changes based on requestAnimationFrame. For example, it can be used using raf-schd lodash function
261. ### How JSX prevents Injection Attacks?
     React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered. For example, you can embed user input as below,
     ```javascript
     const name = response.potentiallyMaliciousInput;
     const element = <h1>{name}</h1>;
     ```
     This way you can prevent XSS(Cross-site-scripting) attacks in the application.
262. ### How do you update rendered elements?
     You can update UI(represented by rendered element) by passing the newly created element to ReactDOM's render method. For example, lets take a ticking clock example, where it updates the time by calling render method multiple times,
     ```javascript
     function tick() {
       const element = (
         <div>
           <h1>Hello, world!</h1>
           <h2>It is {new Date().toLocaleTimeString()}.</h2>
         </div>
       );
       ReactDOM.render(element, document.getElementById('root'));
     }

     setInterval(tick, 1000);
     ```
263. ### How do you say that props are read only?
     When you declare a component as a function or a class, it must never modify its own props. Let us take a below capital function,
     ```javascript
     function capital(amount, interest) {
        return amount + interest;
     }
     ```
     The above function is called “pure” because it does not attempt to change their inputs, and always return the same result for the same inputs. Hence, React has a single rule saying "All React components must act like pure functions with respect to their props."
264. ### How do you say that state updates are merged?
     When you call setState() in the component, React merges the object you provide into the current state. For example, let us take a facebook user with posts and comments details as state variables,
     ```javascript
       constructor(props) {
         super(props);
         this.state = {
           posts: [],
           comments: []
         };
       }
     ```
     Now you can update them independently with separate setState() calls as below,
     ```javascript
      componentDidMount() {
         fetchPosts().then(response => {
           this.setState({
             posts: response.posts
           });
         });

         fetchComments().then(response => {
           this.setState({
             comments: response.comments
           });
         });
       }
     ```
     As mentioned in the above code snippets, this.setState({comments}) updates only comments variable without modifying or replacing posts variable.
265. ### How do you pass arguments to an event handler?
     During iterations or loops, it is common to pass an extra parameter to an event handler. This can be achieved through arrow functions or bind method. Let us take an example of user details updated in a grid,
     ```javascript
     <button onClick={(e) => this.updateUser(userId, e)}>Update User details</button>
     <button onClick={this.updateUser.bind(this, userId)}>Update User details</button>
     ```
     In both the approaches, the synthetic argument e is passed as a second argument. You need to pass it explicitly for arrow functions and it forwarded automatically for bind method.
266. ### How to prevent component from rendering?
     You can prevent component from rendering by returning null based on specific condition. This way it can conditionally render component.
     ```javascript
     function Greeting(props) {
       if (!props.loggedIn) {
         return null;
       }

       return (
         <div className="greeting">
           welcome, {props.name}
         </div>
       );
     }
     ```
     ```javascript
     class User extends React.Component {
       constructor(props) {
         super(props);
         this.state = {loggedIn: false, name: 'John'};
       }

       render() {
        return (
            <div>
              //Prevent component render if it is not loggedIn
              <Greeting loggedIn={this.state.loggedIn} />
              <UserDetails name={this.state.name}>
            </div>
        );
       }
     ```
     In the above example, the greeting component skips its rendering section by applying condition and returning null value.
267. ### What are the conditions to safely use the index as a key?
     There are three conditions to make sure, it is safe use the index as a key.
     1. The list and items are static– they are not computed and do not change
     2. The items in the list have no ids
     3. The list is never reordered or filtered.

268. ### Is it keys should be globally unique?
     Keys used within arrays should be unique among their siblings but they don’t need to be globally unique. i.e, You can use the same keys withtwo different arrays. For example, the below book component uses two arrays with different arrays,
     ```javascript
     function Book(props) {
       const index = (
         <ul>
           {props.pages.map((page) =>
             <li key={page.id}>
               {page.title}
             </li>
           )}
         </ul>
       );
       const content = props.pages.map((page) =>
         <div key={page.id}>
           <h3>{page.title}</h3>
           <p>{page.content}</p>
           <p>{page.pageNumber}</p>
         </div>
       );
       return (
         <div>
           {index}
           <hr />
           {content}
         </div>
       );
     }
     ```
269. ### What is the popular choice for form handling?
     Formik is a form library for react which provides solutions such as validation, keeping track of the visited fields, and handling form submission. In detail, You can categorize them as follows,

     1. Getting values in and out of form state
     2. Validation and error messages
     3. Handling form submission

     It is used to create a scalable, performant, form helper with a minimal API to solve annoying stuff.
270. ### What are the advantages of formik over redux form library?
     Below are the main reasons to recommend formik over redux form library
     1. The form state is inherently short-term and local, so tracking it in Redux (or any kind of Flux library) is unnecessary.
     2. Redux-Form calls your entire top-level Redux reducer multiple times ON EVERY SINGLE KEYSTROKE. This way it increases input latency for large apps.
     3. Redux-Form is 22.5 kB minified gzipped whereas Formik is 12.7 kB

271. ### Why do you not required to use inheritance?
     In React, it is recommend using composition instead of inheritance to reuse code between components. Both Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way.
     Whereas, If you want to reuse non-UI functionality between components, it is suggested to extracting it into a separate JavaScript module. Later components import it and use that function, object, or a class, without extending it.
272. ### Can I use web components in react application?
     Yes, you can use web components in a react application. Even though many developers won't use this combination, it may require especially if you are using third-party UI components that are written using Web Components. For example, let us  use Vaadin date picker web component as below,
     ```javascript
     import React, { Component } from 'react';
     import './App.css';
     import '@vaadin/vaadin-date-picker';
     class App extends Component {
       render() {
         return (
           <div className="App">
             <vaadin-date-picker label="When were you born?"></vaadin-date-picker>
           </div>
         );
       }
     }
     export default App;
     ```
273. ### What is dynamic import?
     The dynamic import() syntax is a ECMAScript proposal not currently part of the language standard. It is expected to be accepted in the near future. You can achieve code-splitting into your app using dynamic import(). Let's take an example of addition,
     1. **Normal Import**
     ```javascript
     import { add } from './math';
     console.log(add(10, 20));
     ```
     2. **Dynamic Import**
     ```javascript
     import("./math").then(math => {
       console.log(math.add(10, 20));
     });
     ```
274. ### What are loadable components?
     If you want to do code-splitting in a server rendered app, it is recommend to use Loadable Components because React.lazy and Suspense is not yet available for server-side rendering. Loadable lets you render a dynamic import as a regular component. Lets take an example,
     ```javascript
     import loadable from '@loadable/component'

     const OtherComponent = loadable(() => import('./OtherComponent'))

     function MyComponent() {
       return (
         <div>
           <OtherComponent />
         </div>
       )
     }
     ```
     Now OtherComponent will be loaded in a separated bundle
275. ### What is suspense component?
     If the module containing the dynamic import is not yet loaded by the time parent component renders, you must show some fallback content while you’re waiting for it to load using a loading indicator. This can be done using **Suspense** component. For example, the below code uses suspense component,
     ```javascript
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
       return (
         <div>
           <Suspense fallback={<div>Loading...</div>}>
             <OtherComponent />
           </Suspense>
         </div>
       );
     }
     ```
     As mentioned in the above code, Suspense is wrapped above the lazy component.
276. ### What is route based code splitting?
     One of the best place to do code splitting is with routes. The entire page is going to re-render at once so users are unlikely to interact with other elements in the page at the same time. Due to this, the user experience won't be disturbed. Let us take an example of route based website using libraries like React Router with React.lazy,
     ```javascript
     import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
     import React, { Suspense, lazy } from 'react';

     const Home = lazy(() => import('./routes/Home'));
     const About = lazy(() => import('./routes/About'));

     const App = () => (
       <Router>
         <Suspense fallback={<div>Loading...</div>}>
           <Switch>
             <Route exact path="/" component={Home}/>
             <Route path="/about" component={About}/>
           </Switch>
         </Suspense>
       </Router>
     );
     ```
     In the above code, the code splitting will happen at each route level.
277. ### Give an example on How to use context?
     **Context** is designed to share data that can be considered **global** for a tree of React components.  For example, in the code below lets manually thread through a “theme” prop in order to style the Button component.
     ```javascript
     //Lets create a context with a default theme value "luna"
     const ThemeContext = React.createContext('luna');
     // Create App component where it uses provider to pass theme value in the tree
     class App extends React.Component {
       render() {
         return (
           <ThemeContext.Provider value="nova">
             <Toolbar />
           </ThemeContext.Provider>
         );
       }
     }
     // A middle component where you don't need to pass theme prop anymore
     function Toolbar(props) {
       return (
         <div>
           <ThemedButton />
         </div>
       );
     }
     // Lets read theme value in the button component to use
     class ThemedButton extends React.Component {
       static contextType = ThemeContext;
       render() {
         return <Button theme={this.context} />;
       }
     }
     ```
278. ### What is the purpose of default value in context?
     The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This can be helpful for testing components in isolation without wrapping them. Below code snippet provides default theme value as Luna.
     ```javascript
     const MyContext = React.createContext(defaultValue);
     ```
279. ### How do you use contextType?
     ContextType is used to consume the context object. The contextType property can be used in two ways,
     1. **contextType as property of class:**
     The contextType property on a class can be assigned a Context object created by React.createContext(). After that, you can consume the nearest current value of that Context type using this.context in any of the lifecycle methods and render function.
     Lets assign contextType property on MyClass as below,
     ```javascript
     class MyClass extends React.Component {
       componentDidMount() {
         let value = this.context;
         /* perform a side-effect at mount using the value of MyContext */
       }
       componentDidUpdate() {
         let value = this.context;
         /* ... */
       }
       componentWillUnmount() {
         let value = this.context;
         /* ... */
       }
       render() {
         let value = this.context;
         /* render something based on the value of MyContext */
       }
     }
     MyClass.contextType = MyContext;
     ```
     2. **Static field**
     You can use a static class field to initialize your contextType using public class field syntax.
     ```javascript
     class MyClass extends React.Component {
       static contextType = MyContext;
       render() {
         let value = this.context;
         /* render something based on the value */
       }
     }
     ```
280. ### What is a consumer?
     A Consumer is a React component that subscribes to context changes. It requires a function as a child which receives current context value as argument and returns a react node. The value argument passed to the function will be equal to the value prop of the closest Provider for this context above in the tree. Lets take a simple example,
     ```javascript
     <MyContext.Consumer>
       {value => /* render something based on the context value */}
     </MyContext.Consumer>
     ```
281. ### How do you solve performance corner cases while using context?
     The context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. For example, the code below will re-render all consumers every time the Provider re-renders because a new object is always created for value.
     ```javascript
     class App extends React.Component {
       render() {
         return (
           <Provider value={{something: 'something'}}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```
     This can be solved by lifting up the value to parent state,
     ```javascript
     class App extends React.Component {
       constructor(props) {
         super(props);
         this.state = {
           value: {something: 'something'},
         };
       }

       render() {
         return (
           <Provider value={this.state.value}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```
282. ### What is the purpose of forward ref in HOCs?
     Refs will not get passed through because ref is not a prop. It handled differently by React just like **key**. If you add a ref to a HOC, the ref will refer to the outermost container component, not the wrapped component. In this case, you can use Forward Ref API. For example, we can explicitly forward refs to the inner FancyButton component using the React.forwardRef API.
     The below HOC logs all props,
     ```javascript
     function logProps(Component) {
       class LogProps extends React.Component {
         componentDidUpdate(prevProps) {
           console.log('old props:', prevProps);
           console.log('new props:', this.props);
         }

         render() {
           const {forwardedRef, ...rest} = this.props;

           // Assign the custom prop "forwardedRef" as a ref
           return <Component ref={forwardedRef} {...rest} />;
         }
       }

       return React.forwardRef((props, ref) => {
         return <LogProps {...props} forwardedRef={ref} />;
       });
     }
     ```
     Let's use this HOC to log all props that get passed to our “fancy button” component,
     ```javascript
     class FancyButton extends React.Component {
       focus() {
         // ...
       }

       // ...
     }
     export default logProps(FancyButton);
     ```
     Now lets create a ref and pass it to FancyButton component. In this case, you can set focus to button element.
     ```javascript
     import FancyButton from './FancyButton';

     const ref = React.createRef();
     ref.current.focus();
     <FancyButton
       label="Click Me"
       handleClick={handleClick}
       ref={ref}
     />;
     ```
283. ### Is it ref argument available for all functions or class components?
     Regular function or class components don’t receive the ref argument, and ref is not available in props either. The second ref argument only exists when you define a component with React.forwardRef call.
284. ### Why do you need additional care for component libraries while using forward refs?
     When you start using forwardRef in a component library, you should treat it as a breaking change and release a new major version of your library. This is because your library likely has a different behavior such as what refs get assigned to, and what types are exported. These changes can break apps and other libraries that depend on the old behavior.
285. ### How to create react class components without ES6?
     If you don’t use ES6 then you may need to use the create-react-class module instead. For default props, you need to define getDefaultProps() as a function on the passed object. Whereas for initial state, you have to provide a separate getInitialState method that returns the initial state.
     ```javascript
     var Greeting = createReactClass({
       getDefaultProps: function() {
           return {
             name: 'Jhohn'
           };
         },
       getInitialState: function() {
           return {message: this.props.message};
         },
       handleClick: function() {
          console.log(this.state.message);
       },
       render: function() {
         return <h1>Hello, {this.props.name}</h1>;
       }
     });
     ```
     **Note:** If you use createReactClass then autobinding is available for all methods. i.e, You don't need to use .bind(this) with in constructor for event handlers.
286. ### Is it possible to use react without JSX?
     Yes, JSX is not mandatory for using React. Actually it is convenient when you don’t want to set up compilation in your build environment. Each JSX element is just syntactic sugar for calling React.createElement(component, props, ...children). For example, let us take a greeting example with JSX,
     ```javascript
     class Greeting extends React.Component {
       render() {
         return <div>Hello {this.props.message}</div>;
       }
     }

     ReactDOM.render(
       <Greeting message="World" />,
       document.getElementById('root')
     );
     ```
     You can write the same code without JSX as below,
     ```javascript
     class Greeting extends React.Component {
       render() {
         return React.createElement('div', null, `Hello ${this.props.message}`);
       }
     }

     ReactDOM.render(
       React.createElement(Greeting, {message: 'World'}, null),
       document.getElementById('root')
     );
     ```
287. ### What is diffing algorithm?
     React needs to use algorithms to find out how to efficiently update the UI to match the most recent tree. The diffing algorithms is generating the minimum number of operations to transform one tree into another. However, the algorithms have a complexity in the order of O(n3) where n is the number of elements in the tree.
     In this case, for displaying 1000 elements would require in the order of one billion comparisons. This is far too expensive. Instead, React implements a heuristic O(n) algorithm based on two assumptions:
     1. Two elements of different types will produce different trees.
     2. The developer can hint at which child elements may be stable across different renders with a key prop.
288. ### What are the rules covered by diffing algorithm?
     When diffing two trees, React first compares the two root elements. The behavior is different depending on the types of the root elements. It covers the below rules during reconciliation algorithm,
     1. **Elements Of Different Types:**
        Whenever the root elements have different types, React will tear down the old tree and build the new tree from scratch. For example,  elements <a> to <img>, or from <Article> to <Comment> of different types lead a full rebuild.
     2. **DOM Elements Of The Same Type:**
        When comparing two React DOM elements of the same type, React looks at the attributes of both, keeps the same underlying DOM node, and only updates the changed attributes. Lets take an example with same DOM elements except className attribute,
        ```javascript
        <div className="show" title="ReactJS" />

        <div className="hide" title="ReactJS" />
        ```
     3. **Component Elements Of The Same Type:**
        When a component updates, the instance stays the same, so that state is maintained across renders. React updates the props of the underlying component instance to match the new element, and calls componentWillReceiveProps() and componentWillUpdate() on the underlying instance. After that, the render() method is called and the diff algorithm recurses on the previous result and the new result.
     4. **Recursing On Children:**
        when recursing on the children of a DOM node, React just iterates over both lists of children at the same time and generates a mutation whenever there’s a difference. For example, when adding an element at the end of the children, converting between these two trees works well.
        ```javascript
        <ul>
          <li>first</li>
          <li>second</li>
        </ul>

        <ul>
          <li>first</li>
          <li>second</li>
          <li>third</li>
        </ul>

        ```
     5. **Handling keys:**
     React supports a key attribute. When children have keys, React uses the key to match children in the original tree with children in the subsequent tree. For example, adding a key can make the tree conversion efficient,
     ```javascript
     <ul>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>

     <ul>
       <li key="2014">Connecticut</li>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>
     ```
289. ### When do you need to use refs?
     There are few use cases to go for refs
     1. Managing focus, text selection, or media playback.
     2. Triggering imperative animations.
     3. Integrating with third-party DOM libraries.
290. ### Is it prop must be named as render for render props?
     Even though the pattern named render props, you don’t have to use a prop named render to use this pattern. i.e,  Any prop that is a function that a component uses to know what to render is technically a “render prop”. Lets take an example with the children prop for render props,
     ```javascript
     <Mouse children={mouse => (
       <p>The mouse position is {mouse.x}, {mouse.y}</p>
     )}/>
     ```
     Actually children prop doesn’t need to be named in the list of “attributes” in JSX element. Instead, you can keep it directly inside element,
     ```javascript
     <Mouse>
       {mouse => (
         <p>The mouse position is {mouse.x}, {mouse.y}</p>
       )}
     </Mouse>
     ```
     While using this above technique(without any name), explicitly state that children should be a function in your propTypes.
     ```javascript
     Mouse.propTypes = {
       children: PropTypes.func.isRequired
     };
     ```
291. ### What are the problems of using render props with pure components?
     If you create a function inside a render method, it negates the purpose of pure component. Because the shallow prop comparison will always return false for new props, and each render in this case will generate a new value for the render prop. You can solve this issue by defining the render function as instance method.
292. ### How do you create HOC using render props?
     You can implement most higher-order components (HOC) using a regular component with a render prop. For example, if you would prefer to have a withMouse HOC instead of a <Mouse> component, you could easily create one using a regular <Mouse> with a render prop.
     ```javascript
     function withMouse(Component) {
       return class extends React.Component {
         render() {
           return (
             <Mouse render={mouse => (
               <Component {...this.props} mouse={mouse} />
             )}/>
           );
         }
       }
     }
     ```
     This way render props gives the flexibility of using either pattern.
293. ### What is windowing technique?
     Windowing is a technique that only renders a small subset of your rows at any given time, and can dramatically reduce the time it takes to re-render the components as well as the number of DOM nodes created. If your application renders long lists of data then this technique is recommended. Both react-window and react-virtualized are popular windowing libraries which provides several reusable components for displaying lists, grids, and tabular data.
294. ### How do you print falsy values in JSX?
     The falsy values such as false, null, undefined, and true are valid children but they don't render anything. If you still want to display them then you need to convert it to string. Let's take an example on how to convert to a string,
     ```javascript
     <div>
       My JavaScript variable is {String(myVariable)}.
     </div>
     ```
295. ### What is the typical use case of portals?
     React portals are very useful when a parent component has overflow: hidden or has properties that affect the stacking context(z-index,position,opacity etc styles) and you need to visually “break out” of its container. For example, dialogs, global message notifications, hovercards, and tooltips.
296. ### How do you set default value for uncontrolled component?
     In React, the value attribute on form elements will override the value in the DOM. With an uncontrolled component, you might want React to specify the initial value, but leave subsequent updates uncontrolled. To handle this case, you can specify a **defaultValue** attribute instead of **value**.
     ```javascript
     render() {
       return (
         <form onSubmit={this.handleSubmit}>
           <label>
             User Name:
             <input
               defaultValue="John"
               type="text"
               ref={this.input} />
           </label>
           <input type="submit" value="Submit" />
         </form>
       );
     }
     ```
     The same applies for `select` and `textArea` inputs. But you need to use **defaultChecked** for `checkbox` and `radio` inputs.
297. ### What is your favorite React stack?
     Even though the tech stack varies from developer to developer, the most popular stack is used in react boilerplate project code. It mainly uses Redux and redux-saga for state management and asynchronous side-effects, react-router for routing purpose, styled-components for styling react components, axios for invoking REST api, and other supported stack such as webpack, reselect, ESNext, Babel.
     You can clone the project https://github.com/react-boilerplate/react-boilerplate and start working on any new react project.
298. ### What is the difference between Real DOM and Virtual DOM?
     Below are the main differences between Real DOM and Virtual DOM,

     | Real DOM | Virtual DOM |
     | ----- | ------- |
     | Updates are slow | Updates are fast |
     | DOM manipulation is very expensive. | DOM manipulation is very easy |
     | You can update HTML directly. | You Can’t directly update HTML |
     | It causes too much of memory wastage | 	There is no memory wastage|
     | Creates a new DOM if element updates | It updates the JSX if element update|

299. ### How to add a bootstrap for a react application?
     Bootstrap can be added to your React app in a three possible ways
     1. Using the Bootstrap CDN:
        This is the easiest way to add bootstrap. Add both bootstrap CSS and JS resources in a head tag.
     2. Bootstrap as Dependency:
        If you are using a build tool or a module bundler such as Webpack, then this is the preferred option for adding Bootstrap to your React application
        ```javascript
        npm install bootstrap
        ``
     3. React Bootstrap Package:
        In this case, you can add Bootstrap to our React app is by using a package that has rebuilt Bootstrap components to work particularly as React components. Below packages are popular in this category,
        1. react-bootstrap
        2. reactstrap
300. ### Can you list down top websites or applications using react as front end framework?
     Below are the `top 10 websites` using React as their front-end framework,

     1. Facebook
     2. Uber
     3. Instagram
     4. WhatsApp
     5. Khan Academy
     6. Airbnb
     7. Dropbox
     8. Flipboard
     9. Netflix
     10. PayPal
301. ### Is it recommended to use CSS In JS technique in React?
     React does not have any opinion about how styles are defined but if you are a beginner then good starting point is to define your styles in a separate *.css file as usual and refer to them using className. This functionality is not part of React but came from third-party libraries. But If you want to try a different approach(CSS-In-JS) then styled-components library is a good option.
302. ### Do I need to rewrite all my class components with hooks?
     No. But you can try Hooks in a few components(or new components) without rewriting any existing code. Because there are no plans to remove classes in ReactJS.
303. ### How to fetch data with React Hooks?
     The effect hook called `useEffect` is used to fetch the data with axios from the API and to set the data in the local state of the component with the state hook’s update function.
     Let's take an example in which it fetches list of react articles from the API
     ```javascript
     import React, { useState, useEffect } from 'react';
     import axios from 'axios';

     function App() {
       const [data, setData] = useState({ hits: [] });

       useEffect(async () => {
         const result = await axios(
           'http://hn.algolia.com/api/v1/search?query=react',
         );

         setData(result.data);
       }, []);

       return (
         <ul>
           {data.hits.map(item => (
             <li key={item.objectID}>
               <a href={item.url}>{item.title}</a>
             </li>
           ))}
         </ul>
       );
     }

     export default App;
     ```
     Remember we provided an empty array as second argument to the effect hook to avoid activating it on component updates but only for the mounting of the component. i.e, It fetches only for component mount.
304. ### Is Hooks cover all use cases for classes?
     Hooks doesn't cover all use cases of classes but there is a plan to add them soon. Currently there are no Hook equivalents to the uncommon **getSnapshotBeforeUpdate** and **componentDidCatch** lifecycles yet.
305. ### What is the stable release for hooks support?
     React includes a stable implementation of React Hooks in 16.8 release for below packages
     1. React DOM
     2. React DOM Server
     3. React Test Renderer
     4. React Shallow Renderer
306. ### Why do we use square brackets in useState?
     When we declare a state variable with useState, it returns a pair — an array with two items. The first item is the current value, and the second is a function that lets us update it. Using [0] and [1] to access them is a bit confusing because they have a specific meaning. This is why we use array destructuring instead.
     For example, you can declare state variables for count
     ```javascript
      const [count, setCount] = useState(0);
     ```
     You can name anything for your own state variables.
307. ### What are the sources used for introducing hooks?
     Hooks got the ideas from several different sources. Below are some of them,
     1. Previous experiments with functional APIs in the react-future repository
     2. Community experiments with render prop APIs such as Reactions Component
     3. State variables and state cells in DisplayScript.
     4. Subscriptions in Rx.
     5. Reducer components in ReasonReact.
308. ### How do you access imperative API of web components?
     Web Components often expose an imperative API to implement its functions. You will need to use a **ref** to interact with the DOM node directly if you want to access imperative API of a web component. But if you are using third-party Web Components, the best solution is to write a React component that behaves as a **wrapper** for your Web Component.
309. ### What is formik?
     Formik is a small react form library that helps you with the three major problems,
     1. Getting values in and out of form state
     2. Validation and error messages
     3. Handling form submission

310. ### What are typical middleware choices for handling asynchronous calls in Redux?
     Some of the popular middleware choices for handling asynchronous calls in Redux eco system are `Redux Thunk, Redux Promise, Redux Saga`.
311. ### Is browsers understand JSX code?
     No, browsers can't understand JSX code. You need a transpiler to convert your JSX to regular Javascript that browsers can understand. The most widely used transpiler right now is Babel.
312. ### Describe about data flow in react?
     React implements one-way reactive data flow using props which reduce boilerplate and is easier to understand than traditional two-way data binding.
