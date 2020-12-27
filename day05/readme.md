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
    - 조건부 렌더링
    - 반복문

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
    - rest(...=)/spread(=...)
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
   
