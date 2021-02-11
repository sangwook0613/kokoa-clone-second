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
