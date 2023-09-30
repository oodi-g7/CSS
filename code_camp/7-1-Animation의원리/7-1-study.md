# Animation의 원리
## 1. animation이란?
- 여러 이미지를 연결해서 자연스럽게 움직이는 것처럼 보이게 만드는 기법

## 2. CSS를 이용하여 애니메이션을 만드는 두가지 방법
1. transition속성 활용
2. animation속성과 keyframe활용

### 2-1. transition VS animation
- transition
    - 특정한 이벤트를 기점으로 작동한다. (hover 등)
- animation
    - 시작하기 위한 이벤트가 필요 없다.
    - 시작, 정지, 반복까지 제어할 수 있다.

### 2-2. animation 속성은,
- @keyframes로 애니메이션을 정의하고, 정의한 애니메이션을 불러와서 제어해주어야 한다.
- 제어해주어야 할 부분이 많다보니 transition에 비해 다루기가 상당히 까다롭다.
    - 때문에 transition으로 만들 수 있는 것은 transition안에서 해결한다.
    - transition으로 만들 수 없는 애니메이션을 animation과 keyframes로 만든다.
