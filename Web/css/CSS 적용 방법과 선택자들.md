### CSS 적용 방법과 선택자들  
#### 시작 전 예제 코드  

```
<h1>기본 &amp; 그룹 선택자</h1>
<span>span 요소</span>
<p>p 요소</p>
<p class="blue">p 요소, class는 blue</p>
<span class="blue">span 요소, class는 blue</span>
<p class="blue dark">p 요소, class는 blue와 dark</p>
<p class="blue" id="red">p 요소, class는 blue, id는 red</p>
```

<br>

#### 모든 태그 지정  
```
* {
    color: blue; 
}
```
전체 컬러를 파란색으로 지정한다.   
- 만약 똑같이 전체 태그에 대하여 색상을 지정하는 코드가 있다면 맨 마지막에 있는게 우선순위가 제일 높다.  

<br>

#### 태그 선택자    
```
p {
    color: blue;
}
```
특정 태그 (p 태그)를 지정하여 색상을 파란색으로 변경한다.  

<br>

#### class 선택자  
```
  .blue {
    color: orange;
  }
```
class 선택자는 .으로 선택한다.  

```
  p.blue {
    color: orange;
  }
```
p 태그이면서 class가 blue인 것을 선택  

<br>

#### id 선택자  
```
#red {
    color: red; 
}
```
class보다 우선순위가 높으며 id는 페이지상에서 요소마다 고유해야한다.  

<br>

#### 자식 결합자  
```
<ul class="outer>
    <li></li>
    <li></li>
    <ul>
        <li></li>
        <li></li>
    </ul>
</ul>
```
이러한 코드가 있다고 가정할 때, 맨 처음에 나오는 li는 다음과 같이 css를 지정해줄 수 있다.  

```
.outer > li 
```

<br>

#### 마우스오버 가상 클래스  
```
li:hover {
    color: pink;
}
```