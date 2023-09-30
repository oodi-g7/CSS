# CSS 단위심화
## 1. calc 
- 괄호 안의 사칙연산을 수행하여 그 결과를 속성값으로 사용한다.
- 예시
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