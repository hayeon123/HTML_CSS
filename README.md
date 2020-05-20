# HTML,CSS, javascript
https://hayeon123.github.io/HTML_CSS
--- 
float: left 
- 왼쪽으로 정렬됨.-- 
- inline구조로 변함
- height 값이 0으로 바뀜 
- clear: none, left, right, both 
  - left: float left의 값이 사라짐 
  - right: float right의 값이 사라짐 
  - both: float 양쪽의 값이 사라짐 

---

#### 참고 사이트 

 https://webzz.tistory.com/category/REFERENCE



- 이미지를 표현하는 방법 

  - img 태그로 표현( 의미가 있을 때 ) alt 태그 - 대체 문자 표현 

  - backround 속성으로 표현 (의미가 없을 때)

  - 이미지를 backround 속성  - 웹 표준을 준수하기 위해서는 

    가상으로 대체 문자를 만들어 줌 (IR 효과)

    - 이미지 스프라이트 

### Position 

---------------

position 속성은 상속되지 않음 

#### static 

- 기본 상태 
- 왼쪽에서 오른쪽, 위에서 아래로 쌓임

#### relative

- static의 원래 위치를 기준으로 움직임

#### absolute

- 가장 가까운 상위 요소를 기준으로 위치가 결정 
- 상위 요소가 없으면 html을 기준으로 설정

#### fixted 

- 웹페이지에 항상 따라다니는 광고 


### IR효과
```/* IR효과 */
/* 의미있는 이미지의 대체 텍스트를 제공하는 경우  */
.ir_pm{display: block; overflow: hidden; font-size:0; line-height:0; text-indent:-9999px;}
/* 의미있는 이미지의 대체 텍스트로 이미지가 없어도 대체 텍스트를 보여주고자 할 때 */
.ir_wa{display:block; overflow: hidden; position: relative; z-index: -1; width: 100%;height: 100%;}
/* 대체 텍스트가 아닌 접근성을 위한 숨김 텍스트를 제공할 때  */
.ir_su{overflow: hidden; position: absolute; width:0; height: 0;line-height: 0; text-indent: -9999px;}
```




