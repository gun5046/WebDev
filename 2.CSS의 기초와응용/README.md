
### Introduction
  CSS는 Cascading StyleSheet의 약자입니다. 웹브라우저에 표시되는 HTML 문서의 스타일을 지정하는 (거의) 유일하지만 다루기 쉽지 않은 언어입니다.

+ CSS를 HTML에 적용하는 세 가지 방법은 무엇일까요?
  ```
    External css - 외부 css 파일을 참조하는 방법
    Internal css - HTML 내부에서 css style을 지정하는 방법. style태그를 사용해 지정한다.
    Inline css -  태그 내부에서 style을 지정하는 방법
  ```
  <br/>
  
  + 세 가지 방법 각각의 장단점은 무엇일까요?
  ```
    External css -  장점 : 일일이 태그 마다 style을 지정하지 않고 일괄적으로 style 지정이 가능. 다른 HTML에도 적용가능
                    단점 : Style 시트 파일이 지나치게 복잡해지면 곤란하기 때문에 css파일을 관리하는 노하우가 필요
                    
    Internal css -  장점 : HTML 문서 안 여러가지 태그에 한번에 style 지정 가능.
                    단점 : 다른 HTML 파일에는 적용 불가.
                    
    Inline css - 장점 : 직관적으로 사용이 가능.
                 단점 : 태그마다 style을 지정해야 하므로 코드가 복잡해지고 중복된 코드가 많아진다.
  ```
  <br/>
+ CSS 규칙의 우선순위는 어떻게 결정될까요?
  ```
    1. 사용자 스타일 시트 - 특별한 환경이 필요한 사용자에 맞게 구성한 스타일 시트.
                           보통 운영체제 혹은 시스템을 통해 미리 작성된 것으로 개발자가 제어하지 못한다.
    
    2. 중요 스타일 - 시간이 지나도 변경할 수 없게 스타일. 다른 스타일보다 우선적으로 적용되어야 할 스타일 
                    작성 부분 뒤에 "!important'를 붙여주면 중요 스타일이 된다.
    
    3. 일반 스타일 - 일반적으로 적용되는 스타일로 적용 범위에 따라 우선 순위를 적용. 범위가 좁을 수록 가장 우선적으로 
                    적용되며 넓을수록 우선순위에 밀려난다.
      
      + 일반 스타일에서의 우선 순위
        1. Inline style
        2. Id style
        3. Class style
        4. Tag style
  ```
  <br/>
  
+ CSS의 박스모델은 무엇일까요? 박스가 화면에서 차지하는 크기는 어떻게 결정될까요?
  ```
    브라우저의 렌더링 엔진은 표준 CSS 기본 박스 모델에 따라 각각의 요소를 사각형 박스로 표현한다.
    하나으 박스는 4영역으로 나누어진다. 각 영역을 Content 영역, Padding 영역, Border 영역, Margin 영역이라 한다.
  ```
  ![asdafasf](https://user-images.githubusercontent.com/48385816/136521692-3646121b-9d6b-4eb4-a24f-ad2de8957f45.png)
  
  ```
    Content area - 영역글이나 이미지, 비디오 등 요소의 실제 내용을 포함한다. box-sizing 속성의 값이 기본값인 content-box 일 경우
                   width, height, max-height, max-width, min-height, min-width 속성으로 content 박스의 사이즈를 지정할 수 있다.
  
    Padding area - Content area를 둘러싼 영역, 안쪽 여백.
                   padding, padding-top, padding-bottom, padding-right, padding-left 속성 값으로 사이즈 지정.
                   length(px, em, pt,cm 등)과 %을 속성 값으로 넣을 수 있다.
                   padding은 속성 값으로 여러개를 둘 수 있다.
                   
                   1개 : padding = 1px; -> top, bottom, right, left = 1px
                   2개 : padding = 1px, 2em; -> top, bottom = 1px / right, left = 2em
                   3개 : padding = 1px, 2em, 2px; -> top = 1px / right, left = 2em / bottom = 2px
                   4개 : padding = 1px, 2em, 2px, 4em -> top = 1px / right = 2em / bottom = 2px / left = 3em
                   
    Border area - Padding area를 둘러싼 영역, 경계선.
                  padding과 같이 top, bottom, left, right 속성과 color, style, radius 등을 조합하여 사용할 수 있다.
                  
                                             size style color
                  기본 Border 사용 - border = 4px solid brown;
    
    Margin area - Border area를 둘러싼 영역, 바깥 여백.
                  Padding 과 동일하게 사이즈 지정 가능.
                  
  ```
  <br/>
+ float 속성은 무엇일까요?
  ```
    float 속성은 레이아웃에 관련된 속성이다. 특정 요소를 떠있게, 흐르도록, 부유하게 하도록 하는 속성.
    속성값으로는 right, left가 올 수 있고, 블럭 위치에 따라 알맞은 값을 넣으면 된다.
    다시 말해, float 속성을 사용해 박스를 왼쪽(left) 또는 오른쪽(right)으로 "부유"시키는 레이아웃 기법이다.
    여기서 '부유하다' 라는 의미는 요소가 기본적인 문서 배치의 흐름에서 벗어나 요소의 모서리가 페이지의 왼쪽이나 오른쪽으로 이동하는 것을 말함.
  ```
  <br/>
+ Flexbox(Flexible box)와 CSS Grid의 차이와 장단점은 무엇일까요?
  ```
    
  ```
  <br/>
+ CSS의 비슷한 요소들을 어떤 식으로 정리할 수 있을까요?
  ```
  
  ```
