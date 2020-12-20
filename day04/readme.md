# DAY4

> VUE.JS(4/4)
 --- 
 * Vue 상태관리 : 데이터 전달
    - **props**(부모>자식)
    - **이벤트**(자식>부모)
    - **Vuex**(Flux모델)

 * 이벤트발생
    - this.$emit(이벤트명,인자1,인자2,...)

 * Vuex
    - 단방향 데이터 전달
    - Flux 모델을 구현한 라이브러리
    - 화면과 데이터의 분리
    - **복잡한  state up(props)/down(event) 을 없애기 위해서 사용해야한다**
    - 구성요소
      + component(=view)
      + actions : dispatcher()
      + mutations : commit()
      + state
      + getters

 * axios : 외부함수호출
    - vuex의 actions에 넣어서 처리한다.
    ```
    import axios from "axios";

    axios({
        url: "./item.html",  // 호출되는 서버 주소.
        method: "get",       // request method: get, post, delete, put
        params: null,  // 서버로 보내는 데이터. { data1:"test1", data2:"test2" }
        timeout: 30000,    // 최대 대기 시간: 30초. 30초 이상이 되면 fail 부분이 실행됨.
        responseType: "html",  // response로 넘어오는 데이터 형태: text, html, xml, json, jsonp, script
    })
    .then( (res) => {
        console.log(res.data);
        this.message1 = res.data;
    })
    .catch((error) => {
        console.log(error);
    });

    ``` 
 * ref
    - DOM에 직접 접근
    - 

