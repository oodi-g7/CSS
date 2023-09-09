# CSS 단위
## 1. 절대단위
- **px(pixel)** : 화소
    - 화면을 구성하는 가장 기본이 되는 단위 

## 2. 상대단위
- **%** : 부모 요소의 해당 속성 값에 비례하여 지정한 비율의 값을 적용
- **em** : 스타일 지정 요소`(em을 지정한 해당 요소 자신!)`의 font-size 속성 값에 비례하여 값을 결정
    - % 와 크게 다르진 않지만, 그 기준이 되는 값이 부모 요소가 아닌 스타일이 지정된 요소 당사자의 폰트 사이즈라는 점!
    - [예시] font-size : 16px인 경우 (요소당사자)
        - 1em → 16 x 1 = 16px
        - 0.8em → 16 x 0.8 = 12.8px
        - 3em → 16 x 3 = 48px
- **rem** : 최상위 html 요소의 font-size 속성 값에 비례하여 값을 결정
    - rem 과 달리, 그 기준이 요소 당사자의 폰트 사이즈가 아닌 최상위 html요소라는 점!
    - [예시] font-size : 16px인 경우 (최상위 html요소 : body또는 html)
        - 1rem → 16 x 1 = 16px
        - 0.8rem → 16 x 0.8 = 12.8px
        - 3rem → 16 x 3 = 48px
- **vw/vh** : 요소의 규격을 viewport의 너비값과 높이값에 비례하여 결정
    - viewport : 브라우저 안에서 실제로 화면이 그려지는 영역
    - 반응형 웹을 제작할때 많이 사용됨
    - [예시] viewport : 1200(px) x 920(px)인 경우
        - 10vw → 1200 x 0.1 = 120px
        - 50vh → 920 x 0.5 = 460px
        - 100vw → 1200 x 1 = 1200px

## 3. 단위심화
- **calc** : 괄호 안의 사칙연산을 수행하여 그 결과를 속성값으로 사용한다.
    - [예시]
        ```css
        .item1 {
            background : red;
            width : calc(50px + 50px); /*덧셈 사용시 '+' 앞뒤 공백 필수*/
            height : 50px;
        }
        .item2 {
            background : blue;
            width: calc(100% - 120px); /*뺄셈 사용시 '-' 앞뒤 공백 필수*/
            height : 50px;
        }
        .item3 {
            background : green;
            width : calc(2*100px); 
            height : 50px;
        }
        .item4 {
            background : orange;
            width : calc(100%/4);
            height : 50px;
        }
        ```