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

 * COMPUTED
    - 자동실행 + 동기
    - 반드시 값을 반환해야 한다 *RETURN*
    - data속성 값의 변화에 따라 자동으로 연산한다.
    - 캐싱기능이 있다.

 * 라이프사이클
    - created > **mounted** > **updated** > destroyed
        + mounted : 페이지 로딩시 한번만
        + updated : 리렌더링 될 때마다

 * 템플릿
    - 만드는 방법
        + Plain strings : ""
        + *Template literals : `` (ES6에서 도입된 백틱(`)을 사용)*
        + x-template
        + *Inline templates*
        + Render functions
        + JSX
        + *SFC(Single-file components)*

* dfdfdfdf
 
```
```
