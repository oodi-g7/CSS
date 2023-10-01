# 선택자2
## 1. 가상 클래스 선택자
- 실제로 html 요소를 수정하지 않고, css만으로 가상 요소를 추가해 선택할 수 있다.
    ```css
    선택자:가상클래스 {
        property : value;
    }
    ```
### 1-1. :first-child
- 첫번째 자식요소를 선택
    ```css
    .box1 p:first-child {
        background : red;
    }
    ```
    ```html
    <div class="box1">
        <p>첫번째</p> <!--background : red-->
        <p>두번째</p>
        <p>세번째</p>
        <p>네번째</p>
        <p>다섯번째</p>
        <p>여섯번째</p>
        <p>일곱번째</p>
    </div>
    ```

### 1-2. :last-child
- 마지막 자식요소를 선택
    ```css
    .box1 p:last-child {
        background : blue;
    }
    ```
    ```html
    <div class="box1">
        <p>첫번째</p>
        <p>두번째</p>
        <p>세번째</p>
        <p>네번째</p>
        <p>다섯번째</p>
        <p>여섯번째</p>
        <p>일곱번째</p> <!--background : blue-->
    </div>
    ```

### 1-3. :nth-child(n)
- n번째 자식요소를 선택
    ```css
    .box1 p:nth-child(2) {
        background : green;
    }
    ```
    ```html
    <div class="box1">
        <p>첫번째</p>
        <p>두번째</p> <!--background : green-->
        <p>세번째</p>
        <p>네번째</p>
        <p>다섯번째</p>
        <p>여섯번째</p>
        <p>일곱번째</p>
    </div>
    ```
- n대신 연산자도 가능
    ```css
    .box1 p:nth-child(2n) {
        background : green;
    }
    ```
    ```html
    <div class="box1">
        <p>첫번째</p>
        <p>두번째</p> <!--background : green-->
        <p>세번째</p>
        <p>네번째</p> <!--background : green-->
        <p>다섯번째</p>
        <p>여섯번째</p> <!--background : green-->
        <p>일곱번째</p>
    </div>
    ```