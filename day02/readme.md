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
         ```
         <style scoped></style>
         ```
    - 1개의 root element만 가질 수 있다. (2개 이상이면 div로 감싼다.) 

 * 디렉티브 directive
    - 종류
       + **v-if**
       + v-else-if
       + v-else
       + v-show
       + **v-for**
       + **{{}}**
       + v-text
       + v-html
       + **v-on**
       + **v-bind**
       + **v-model**

 * 데이터 바인딩
    - 표현식 방식 
       + {{}}(콧수염ㅋ.ㅋ) : 자바스크립트 사용가능 but 쓰지마라고 하셨다. 
    - 지시자 방식
       + v-text
       + v-html(보안상의이유로 default로 사용하지않음)

 * 이벤트 바인딩
    - 이벤트 바인딩 지시자
       + v-on
       + @
    - when ___ happens, do ____
    - DOM 생성시점 : css로딩 이후 생성된다.
    - 이벤트 핸들러 설정
       + **인라인 이벤트 모델 (Vue,React)**
       + 고전 이벤트 모델 (1:1)
       ```
         jQuery.click(function(){})
       ```
       + 표준 이벤트 모델 (1:N)
       ```
         jQuery.on('click dbclikc mouseover',function(){})
       ```
    - 이벤트취소
      + cancleable = true 면 취소! 
      + stopPropagation()
      + preventDefault() 
      + 브라우저마다 먹히는게 다르다. 둘 다 쓰시오.

    - 이벤트객체
      + 키보드 이벤트
      + 마우스 이벤트
   
    - phase 3단계
      + capturing : 쭉 내려감
      + targeting : 버튼 찾음
      + **bubbling : 버튼 찾아서 window까지 올라옴**
      + _이벤트 취소는 bubbling 과정 중 이벤트가 위로 올라가지 못하게 하는 것_ 
