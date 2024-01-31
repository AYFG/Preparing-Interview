## React의 라이프 사이클에 대해 설명해주세요.
> <p>React의 라이프 사이클에는 클래스형 컴포넌트 라이프 사이클 메서드와 함수형 컴포넌트 라이프 사이클 관리 Hook이 있습니다.
> 먼저 클래스형 컴포넌트 라이프 사이클은 마운팅, 업데이팅, 언마운팅 단계로 나뉩니다.
> 마운팅은 컴포넌트가 생성되고 DOM에 삽입되는 과정입니다.
> 업데이팅은 마운팅 된 컴포넌트의 상태값(state)이나 속성값(props)이 변경 되었을 때 발생합니다.
> 언마운팅은 마운팅 된 컴포넌트가 DOM에서 제거되는 과정입니다.
> 
> 함수형 컴포넌트 라이프 사이클 관리 Hook은 useEffect를 통해 클래스형 컴포넌트 라이프 사이클과 같은 동작을 할 수 있습니다.
> useEffect에 두 번째 매개변수에 state를 넣으면 첫 렌더링 될 때 한 번 실행, 그 다음부터는 state 값이 바뀔 때마다 실행됩니다.
> useEffect에 두 번째 매개변수에 배열을 아예 넣지 않으면 데이터와 관련 없이 리렌더링 시마다 실행됩니다.
> useEffect에 두 번째 매개변수에 빈 배열을 넣으면 컴포넌트가 마운트 될 때만 실행됩니다.(한 번만 실행)
> useEffect에 componentWillUnmount에 해당하는 역할은 useEffect에 return으로 함수를 제공하면 되는데, 이 함수를 clean-up 함수라고도 합니다.

</br>

<p>$\scr{\normalsize{\color{#69A65A}👇참고 \ 링크 👇}}$</p>

[Function형 React의 라이프 사이클](https://velog.io/@ahsy92/%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91-React%EC%9D%98-%EB%9D%BC%EC%9D%B4%ED%94%84-%EC%82%AC%EC%9D%B4%ED%81%B4-09q2s7uw)<br/>
[React의 생명 주기 Life Cycle](https://www.zerocho.com/category/React/post/579b5ec26958781500ed9955)<br>
[리액트 라이프 사이클](https://velog.io/@remon/React-%EB%A6%AC%EC%95%A1%ED%8A%B8-%EB%9D%BC%EC%9D%B4%ED%94%84-%EC%82%AC%EC%9D%B4%ED%81%B4)<br>
[useEffect와 hook 생명주기](https://killu.tistory.com/44)

</br>
