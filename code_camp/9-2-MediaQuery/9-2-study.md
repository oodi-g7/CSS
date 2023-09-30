# Media Query
## 1. Media Query
- 뷰포트의 너비에 따라 웹 사이트의 스타일 시트를 수정할 수 있다.
- 뷰포트 너비 이외에도 단말기의 종류, 해상도 등을 기준으로 설정할 수 있다.

### @media Media Query
```css
@media screen and (max-width : 500px){
    /*스크린의 viewport너비가 500px이하일 경우 
      적용시킬 스타일 시트를 작성*/
}
```
```css
@media screen and (min-width : 500px){
    /*스크린의 viewport너비가 500px이상일 경우 
      적용시킬 스타일 시트를 작성*/
}
```

## [실습](./9-2-index.html)