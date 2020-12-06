# DAY2

> VUE.JS(2/4)

 * Vue 인스턴스
    - 컴포넌트 조합기
    - edtmc*2 life cycle
        + **el**
        + **data**
        + template
        + **methods(수동 이벤트)**
        + computed(자동 동기식, 기존 값 처리)
        + **components**
        + watch(자동 비동기식 처리, 외부 함수 처리)

 * DATA속성
    - **data 속성의 값을 직접 바꾸면 안된다**
    - 직접 바꾸면 화면 rendering이 되지 않음
    - 얕은복사:=(x) / 깊은복사(o) => 불변객체
    - 방법
        + **this.$set(object, key, value)**
        + **Vue.set(object, key, value)**
        + spliece()
        + spread(react.js)
 * **<u>this.$set</u>**
    - value 변경  
        +  this.$set(this.$data,"msg1","")
    - array, obeject 변경
        +  this.$set(this.$data.msg4, 0, 300);
 * 재할당
    - 기본타입변수 > stack
    - 참조타입변수 > heap
    - 참조타입의 값을 복사하여 값을 바꾼후 기본타입의 값에 넣어준다. (?)

 * WATCH속성
    - 자동실행 + 비동기

 * ㅋㅋㅋㅋ

 * ㅜ
13-15








 * 설치
    - VSCODE
        + vetur
        + vue 2 snippets
        + live server
        + open in browser 
        + code snippet(설정)
    - node.js
    - git / tortoiseGit
    - 나눔고딕코딩
    - vue.js dev tools(크롬Vue개발자도구)

* git 사용
    - create repo
    - git clone
    - git commit / push
    - git pull
    - .gitignore

*  기초
    - html과 javascript
    - object와 array
        +  CRUD
    - 절차지향C/객체지향JAVA/함수형PYTHON,R
    - 함수
        + **표현식함수(선호)** 
        + 선언식함수(호이스팅)
        + 화살표함수(this 처리방식의 차이, ES6)
    - DOM API (Jquery에서 사용하는 것:  document.querySelector("") )
    - DEBUGGING(개발자도구의 Sources탭)
        + BREAK POINT or debugger;
        + F8 : 다음 BREAK POINT
        + F10 : 한 줄
        + F11 : 메서드 안으로
    - ES6 변수선언
        + var > let,const : 호이스팅을 막음
    - ES6 문법 필수

*  Babel (https://babeljs.io/repl/)
    - JS컴파일러

*  Webpack (파일결합)
    - jquery : load(), ajax()
    - node.js : import(ES6), require(CommonJS)

* Vue.js란
    - 프론트엔드프레임워크    
    *함수<모듈(파일)<패키지(디렉토리)<라이브러리<프레임워크*
    - 주요기능
        + 클라이언트 화면 렌더링
        + **데이터 바인딩** 
        + **컴포넌트(복제)**
        + 라우팅(페이지 내 위치이동)
        + 상태관리(변수)
    - 웹'만' 만들때는 뷰가 리엑트보다 빠름
    - react와 angular의 장점을 결합

* 작업순서
    1. 스트립트 플러그인 임포트
        + vueplugin < snippets에 추가해둔 것을 불러옴
    2. **Vue인스턴스 생성html**
    3. **el, data, method**에 프로퍼티 설정
        + el : 태그 찾기
        + data : 변수(상태) 설정
        + method : 이벤트 처리
    4. 파일에 dom컨테이너 추가  

* 디자인패턴 : 데이터와 화면을 분리하는 방법
    - MVP
    - MVC(Spring)
    - **MVVM (Angular1,Vue(*입력태그에서만*))**
        + v-model 설정만 하면 양방향 처리됨
    - MVW
    - **FLUX (Redux, VueX)**
        + 단방향처리 
        
* Vue.js 동작원리
    - Angular의 two-way binding
        + MVVM패턴을 사용하여 데이터 바인딩
    - Component
        + 화면을 여러개의 작은 단위로 쪼개어 개발( 수정없이 재사용 가능 )
    - React의 Vitrual DOM
        
* Vue.js 구성요소
    - 인스턴스
        + 화면 개발시 필수로 생성해야 하는 단위(땅)
        + new Vue({})
        + edtmc*2w life cycle
    - 데이터바인딩
    - 컴포넌트
    - 라우터



```
```
