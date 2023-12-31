# Transition
## 1. transition
- 애니메이션을 줄 수 있는 방법 중 하나
- CSS 속성을 이용한 변화의 전/후 사이에 애니메이션을 추가해서 움직임을 부드럽게 만들어 줌

## 2. transition-property
- 어떠한 속성(property)에 transition을 적용할 것인지 지정한다.
- 예시) `transition-property : color, transform`

## 3. transition-duration
- transition에 걸리는 시간을 지정한다.
- 예시) `transition-duration : 0.2s`
- 단위 : s(초), ms(밀리 초)

## 4. transition-timing-function
- transition의 속도 패턴을 지정한다.
- 예시) `transition-duration : ease-in-out`
    - linear : 일정한 속도로 변화한다
    - ease : 시작할 때에는 빨라지다 느려진다
    - ease-in : 천천히 시작했다가, 속도를 높여 끝난다.
    - ease-out : 빠른 속도로 시작했다가, 천천히 끝난다.
    - ease-in-out : 천천히 시작했다가, 정상 속도가 됐다가, 빠르게 끝난다.
    - [예시링크](https://codepen.io/Joogumi/full/eYMgrKO)

## 5. transition-delay
- transition 요청을 받은 후, 실제로 실행되기까지 기다려야하는 시간의 양을 지정한다.
- 예시) `transition-delay : 2s`

## 6. transition 단축 속성
- transition : [property] [duration] [timing function] [delay]
- `transition : color 0.4s ease-in-out 1s`

## 7. [실습](./5-3-index.html)
<img src="./1.png">