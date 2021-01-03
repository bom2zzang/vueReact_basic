# DAY6✨

> REACT.JS(2/2)
 --- 

 * 목표
    - 생명주기
    - 스타일링
    - 이벤트
    - 상태관리 (state/props)
    - crud

 * 생명주기
    - componentDidMount
      + 페이지 load 될 때 한번
    - componentDidUpdate
      + state 가 변경될 때마다
    - componentWillUnmount
      + **redux구독해제**, 이벤트해제

 * 스타일링
    - 분리형 스타일링
      + 뼈대와 장식 분리
      + 웹표준
    - 통합형 스타일링
      + 뼈대와 장식 통합
      + react는 인라인 스타일링을 사용 > 컴포넌트의 **재사용**을 위하여

 * 스타일링 기법
    - css module
    - sass
    - styled-component

 * 스타일 상속
    - self참조 :  get함수 사용
    - spread연산자

 * React 이벤트 객체 **syntheticEvent**
    - [참고](https://reactjs.org/docs/events.html)

 * 상태관리
    - props : 속성전달 -읽기전용
    - state : 컴포넌트 변수 선언 (데이터보관) - 읽기쓰기

 * 단방향 데이터 흐름

 * ref (reference)
    - **입력태그에서 값을 get/set 할 때**
    - **focus**
    - 스크롤 박스 조작
    - canvas에 그림 그릴 때
    - **부모컴포넌트에서 자식컴포넌트 함수 호출시**
   
 * ref 사용법
    - 콜백 ref방식
      + ```ref={(el)=>this.ref이름=el}```
    - **React.createRef()방식** (z속도가 빠르지만 크게 차이 없음)

 * CRUD
    - 즐거웠다!
 ---
