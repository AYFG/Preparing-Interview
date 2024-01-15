## Reflow와 Repaint가 실행되는 시점에 대해 설명해주세요.
> <p>reflow는 생성된 DOM 노드의 레이아웃 수치(너비, 높이, 위치 등) 변경 시 영향 받은 모든 노드의(자신, 자식, 부모, 조상(결국 모든 노드) ) 수치를 다시 계산하여(Recalculate),
> 렌더 트리를 재생성하는 과정으로 DOM 노드의 추가/제거, DOM 노드의 위치/크기 변경 (width, margin, border 등), Window 창 크기 조절 (위치/크기 값이 상대 값일 경우)
> CSS 애니메이션과 트랜지션 사용, 계산된 css 정보 요청(offset, scrollTop 등), 폰트 변경, 이미지 크기 변경, 텍스트 변경 등
> 웹 페이지의 위치와 기하학적 구조를 다시 계산하는 경우 발생합니다.</br></br>
> repaint는 reflow 과정이 끝난 후 재생성된 렌더 트리를 다시 그리는 작업으로 화면의 구조가 변경이 될 때는 reflow와 repaint가 모두 발생합니다.
> 다만, repaint가 발생하기 위해서 항상 reflow가 발생해야 하는 것은 아닙니다. 
> 수치와 상관없는 color, background-color, visibility 등의 속성 변경 시에는 reflow 과정을 생략한 repaint 작업만 실행됩니다.</p></br>
> 그리고 GPU가 관여할 수 있는 속성이 변경될 때는 리플로우와 리페인트 과정을 생략할 수 있는데 transform, opacity 속성이 이에 해당됩니다.

</br>
<p>$\scr{\normalsize{\color{#69A65A}👇참고 \ 링크 👇}}$</p>

[MDN - Reflow](https://developer.mozilla.org/ko/docs/Glossary/Reflow)<br>
[MDN - Repaint](https://developer.mozilla.org/ko/docs/Glossary/Repaint)<br>
[Reflow와 Repaint](https://k0102575.github.io/articles/2020-11/reflow-repaint)<br>
[효율적인 애니메이션 - GPU 사용하기](https://velog.io/@kskim625/%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9D%B8-%EC%95%A0%EB%8B%88%EB%A9%94%EC%9D%B4%EC%85%98-CSS-vs.-JavaScript)<br>


</br>

### 💡GPU란?
컴퓨터 그래픽을 처리하는 장치로, 그래픽 카드를 구성하는 가장 중요한 핵심 요소입니다.<br>
[나무위키 - GPU](https://namu.wiki/w/GPU)<br>
[웹 애니메이션 GPU 가속](https://iropke.com/archive/animation-gpu.html)
