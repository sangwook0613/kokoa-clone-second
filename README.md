# Second Kokoa Clone v.2020

HTML & CSS 복습용

시작일자: 21. 2. 2

## 1. Index Screen

not 사용

- not(속성)은 '해당 속성을 제외한 나머지에 적용하고 싶다'는 의미
- 기존 id나 class와 중복 적용하면 안된다!
  var 사용
  transition 적용
  id나 class 내 특정 속성값을 갖는 자손들에 접근하는 자손 결합자
- `#id값 자손태그명[속성="속성값"]`

## 2. Friends Screen

1. Navigation Bar

- `box-sizing: border-box`의 필요성
- `position: absolute`의 유용성

## 3. Chat Screen

- `z-index`의 유용성
  - poistion이 `absolute`이거나 `fixed`일 때 각 layer가 쌓이는 순서를 조정
- `order`의 사용
  - 형식은 똑같으나 순서만 바꾸고 싶을 때, 덮어씌워서 바꾸자.
  - 단, flexbox 자손들에게만 적용된다.
  - 이 때 같은 block 내에 모든 클래스에 `order`를 적용해줘야한다.
- 위 `order`의 대체품으로 `flex-direction: row-reverse`가 있다!! (부모에서 적용)

## 4. Animation

- `animation: forward` 를 통해 가져온 애니메이션의 마지막 장면을 유지한다.

- 만약 한 장면을 fade-out 하면서 완전히 살아지게 하고 싶다면, `visibility: hidden`을 이 때 사용하자!

  - `none`과 `hidden`의 차이는 항상 신경쓰자

- 애니메이션이 다소 부자연스럽다면 `will-change`를 쓰자.

  - will-change는 애니메이션이 좀 더 부드럽게 동작할 수 있게 한다. → 브라우저에게 어떤 것이 변할 것인지 예고해주는 것
  - will-change는 그래픽 카드를 이용해서 애니메이션을 가속화 한다.

- focus가 가능한 element에만 특정 animation을 적용하고 싶다면 state 선택자 `focus-within`을 사용하자.
  - 만약 `transform` 속성을 사용하고 싶다면, 부모에 `transition`이 선언되어 있는지 확인하자.
