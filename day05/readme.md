# DAY5✨

> VUE.JS(5/4)
 ---
 * todoMaster

> REACT.JS(1/2)
 --- 

 * 핵심
    - Virtual DOM

 * JSX : **Javascript XML**
    - 열면 닫아야한다.
    - Babel 필요
    - render() 함수에 코드를 완성한다. 
    - 표기법
      + 카멜
      + 표기법 : class>className / for>htmlFor / value>defaultValue
    - 표현식 **{}**
      + {this.props.name} : 부모태그의 정보
      + {this.props.children} : 부모태그 사이의 모든 정보를 넘길 수 있다.
      + {this.state.msg}
      + 문자열만 예외적으로 블락대신 ''로 표현 가능
    - 특수문자는 이스케이프 처리
    - 조건부 렌더링 > 태그상에서 처리하기보다 컴포넌트 안에서 처리하자. 또는 adress연산자를 사용하여 처리**
    - 반복문
    - 주석 {/**/}

 * 컴포넌트
    - 클래스 컴포넌트(웹+앱)
       + state *(vue에서의 this.$set() >  react에서 this.setState())*
       + props
       + creatRef()
    - 함수 컴포넌트
       + 구조가 조금 다르기 때문에 pass..한다.
    - 고차 컴포넌트
       + 함수+클래스
    - 컴포넌트 관계
       + 부모/자식
       + 컨테이너/프로세스 *(데이터용/화면용)*

 * 컴포넌트 라이프 사이클
   | 마운트 | **업데이트** | 언마운트 |
   |:-------:|:----------:|:----------:|
   |componentDidMount()|componentDidUpdate()||
   

 * 개발환경설정
   - vscode : react / redux 플러그인 설치
   - chrome : react developer tools / redux developer tools
   
 * es6를 기본 문법으로 사용
    | ES5 | **ES6(2016)** |ES2018|
   |:-------:|:----------:|:---:|
   |var|let/const||
   |function함수|화살표함수(this)||
   ||분해할당<br>(Destructure assignment)<br>**[]** =[]/ **{}**={}||
   ||rest(...=)/spread(=...)||
   |생성자로 객체 생성|class로 객체 생성<br>(상속,extends)||
   |콜백|프로미스(Promise>|async, await<br>(redux의 외부라이브러리에서 사용)|

 * Babel 필요
    - ```<script type="text/babel">```

 * 변수선언
    - var
    - let
      + 읽기쓰기
    - const
      + 읽기전용

 * 템플릿 리터럴
    - 여러줄 문자열
    - 백틱, `표시

 * 디폴트 매개변수
    - 함수 호출 시 값을 지정하지 않으면 디폴트 값이 들어간다.

 * 가변 매개변수
    - Variable Parameter
    - rest 연산자(...=)(배열)
      + **배열을 만들기 위해 사용되는 연산자**
      + arguments(유사 배열 객체)를 대체 가능
      + arguments와 본질은 다르나 사용법은 동일함

    - spread 연산자(=...)
      + **개별요소로 분리할 때 사용**
      + Array, String, Object, Map, Set 에서만 사용 가능
      ```
      function aaa(...rest){}
      var abc = aaa(...spread);
      ```

   
 * 화살표 함수 (=>)
   ```
      var func1 = function(a,b){
         return a+b;
      }
      let func2 = (a,b) => { return a+b;}
      let func3 = (a,b) => a+b;
   ```

 * 개선된 객체 표현식
    - 생략이 많아짐 *(예제참고)*

 * 분해할당
    - 배열 분해 할당 
      + 순서가 같아야 한다.
      + [분해할당연산자] = [배열리터럴] 

    - 객체 분해 할당
      + 이름이 같아야 한다.
      + {분해할당연산자} = {객체리터럴} 

 * 클래스 (Class)
    - 객체지향 프로그래밍
    - 클래스 상속 extends

 * React
    - 싱글 페이지 라이브러리
    - 빠른 화면 처리
    - SPA 개발에 유리
    - WEB+APP
    - 빌드방식/플러그인방식
   
 * React 동작원리
    - Virtual DOM
      + Component
      + JSX *(화면)*
      + render()
      + 상태관리:state/setState()
      + JSX코드 > render() 함수 >  실제 DOM트리에 추가
    - Component
      + 화면 블락
      + 화면을 여러 단위로 나눠 개발

 * 작성 순서
    1. 플러그인추가 or 임포트선언
    2. 리액트 객체 임포트 확인
    3. 컴포넌트 만들기   ```React.Component```
    4. DOM에 컴포넌트 주입

 * **JSX 조건문**
 * **JSX 반복문**
    - for in
    - for of
    - **map** : 이어서 뭔가를 더 할 수 있기 때문에 추천..!

 * [함수형 프로그래밍 참고](https://www.zerocho.com/category/JavaScript/post/5acafb05f24445001b8d796d)
 
 * Component
    - 재사용
    - 화면블록
    - javascript, css, html 을 한 곳에 넣는다.
    - 생성 : 클래스형/함수형/고차(하이어오더)
    - 화면처리 : 단순/복합/사용자
    - 패턴 : 컨테이너(클래스형,공유데이터) / 프레젠테이션(함수형,view)

 * 상태관리
    - props
       + 읽기 전용
       + 상태, 메서드, 스타일을 내릴 수 있다.
    - state
       + 읽기, 쓰기
    - redux : 외부객체에 저장하는 방식

 * 생명주기 == 라이프사이클
    - 마운트 ```componentDidMount```
      + DOM 노드 생성
    - 업데이트 ```componentDidUpdate```
      + DOM 노드 변경
    - 언마운트 ```componentWillUnmount```
      + DOM 노드 제거
      
