# [Disclosure (Show/Hide) Pattern](https://www.w3.org/WAI/ARIA/apg/patterns/disclosure/)

Disclosure는 컨텐츠가 감춰질 수도(collapsed) 드러날 수도(expanded) 있는 위젯입니다.

두 개의 요소로 이루어집니다: disclosure 버튼과, 이 버튼에 의해 보임 여부가 컨트롤되는 컨텐츠 영역입니다.

일반적으로 버튼은 대상 영역이 감춰진 상태에서 push 버튼(오른쪽 방향 화살표 또는 삼각형, ⏵)으로 스타일링되어 활성화 시 추가 컨텐츠를 드러낼 것임을 암시합니다. 대상 영역이 보여지게 되면 스타일링 방향이 아래쪽(⏷)으로 바뀝니다.

### 키보드 상호작용

disclosure 버튼에 포커스가 있을 때,

- `Enter`, `Space`: disclosure control을 활성화하고 컨텐츠 가시성을 토글합니다.

### WAI-ARIA Roles, States, Properties

- 가시성을 조작하는 요소는 `role="button"`을 가집니다.

- 컨텐츠가 드러났을 때 해당 요소에 `aria-expanded="true"`가 설정됩니다. 감춰지면 `"false"`로 변경됩니다.

- (optional) 버튼 역할을 하는 요소의 `aria-controls` 값으로 보여지거나 가려질 모든 컨텐츠를 포함하는 요소를 참조합니다.
