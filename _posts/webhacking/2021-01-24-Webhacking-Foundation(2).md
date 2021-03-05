---
layout: post
current: post
cover:  assets/built/images/Webhacking_logo.jpg
navigation: True
title: Webhacking_Foundation(2)
date: 2021-01-24 18:25:00 +0900
tags: [Webhacking]
class: post-template
subclass: 'post tag-python'
author: JoHo
---

{% include Webhacking-table-of-contents.html %}

---

> PHP , MYSQL , JS , CSS+HTML 순으로 진행하겠습니다.

<i class="fa fa-hand-o-right" style="color:#008080"></i> PHP  
===  

<br>

### <mark>PHP 원리</mark>

![PHP 원리](https://user-images.githubusercontent.com/76092057/105626610-e6b7fe80-5e73-11eb-884c-8d8ae14bb8e5.PNG){: width="100%" height="100%"}

<i class="fa fa-chevron-circle-right" style="color:black"></i> 만약 확장자가 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> HTML</span>파일을 만들었다면 언제나 같은 정보를 출력하는 웹페이지를 출력한다.    그러나 확장자가 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> PHP</span>가 되면 리로드할 때마다 달라지는 동적인 웹페이지 생성이 가능하다.  

### <mark>PHP Number & Operator</mark>

```html
<!doctype html>
<html>
<body>
    <h1>1+1</h1>  <!-- 1 + 1 출력 --> 
<?php
echo 1+1;         // 2 출력 
?>
    <h1>2-1</h1>  <!-- 2 - 1 출력 --> 
<?php
echo 2-1;         // 1 출력 
?>
    <h1>2*2</h1>  <!-- 2 * 2 출력 --> 
<?php
echo 2*2;         // 4 출력 
?>
    <h1>4/2</h1>  <!-- 4 / 2 출력 --> 
<?php
echo 4/2;         // 2 출력 
?>    
<body>
</html>
```

<i class="fa fa-search" style="color:#01077c"></i> Arithmetic operator   
<i class="fa fa-envelope-o" style="color:red"></i> 산술적인 계산에 사용되는 연산자를 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> Arithmetic operator</span> 라고 한다.  

### <mark>PHP String</mark>

```html
<!doctype html>
<html>
<body>
    <h1>String & String Operator</h1>
<?php
echo 'Hello word';    // Hello word 출력
echo "Hello 'w'ord";  //  작은 따옴표와 큰 따옴표를 이용해 Hello 'w'ord 출력
echo "Hello \"w\"ord";  //  escape('\') 를 사용하면 일시적으로 순수한 문자로 사용가능
?>
    <h2>concatenation Operator</h2> <!-- 좌항과 우황의 문자열을 합치고 싶을 떄 -->
<?php
echo "Hello "."world";  // . 을 이용해 좌항과 우항을 합칠 수 있다.
?>
    <h2>String length function</h2> <!-- 문자의 개수를 알고 싶을 때 -->
<?php
echo strlen("Hello world") // 11 출력
?>
</body>
</html>
```
<i class="fa fa-search" style="color:#01077c"></i> concatenation Operator  
<i class="fa fa-envelope-o" style="color:red"></i> 좌항과 우황의 문자열을 합치기 위해 사용한다. 

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> MySQL 
===  

<br>

### <mark>MySQL 구조</mark>

![MySQL 구조](https://user-images.githubusercontent.com/76092057/105628668-89c34500-5e81-11eb-845e-4e63b89ed214.PNG){: width="100%" height="100%"}

<i class="fa fa-chevron-circle-right" style="color:black"></i>
MySQL 설치 == DateBase Server 설치 의미<br> MySQL 이라는 프로그램이 가지고 있는 기능성을 이용해서 데이터와 관련된 작업을 하는 것이다.  

### <mark>Root 계정으로 접속하고, 스키마 만들기</mark>  
<br>

1. cmd에서 명령어를 이용해 mysql 프로그램이 있는 장소로 이동  
> cd C:\Bitnami\wampstack-7.4.12-0\mysql\bin

2. 명령어를 이용해 sql을 관리자 계정을 실행
> mysql -uroot -p

3. 관리자 비밀번호를 입력하면 접속 성공!

4. 명령어 입력
> CREATE DATABASE opentutorials;

5. 잘 만들어졌는지 확인하기 위해 명령어 입력
> SHOW DATABASES;
![DateBase 확인창](https://user-images.githubusercontent.com/76092057/105629249-36eb8c80-5e85-11eb-95e3-00f03ba2d1f9.PNG){: width="100%" height="100%"}
 
---

 <i class="fa fa-hand-o-right" style="color:#008080"></i> JavaScript
===  

<br>

<i class="fa fa-search" style="color:#01077c"></i><mark> JavaScript의 특징</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> JavaScript는 사용자와 상호작용하는 언어이다.  
<i class="fa fa-envelope-o" style="color:red"></i> 웹 브라우저는 한번 화면에 출력되면 자신을 바꿀 수 없지만, JavaScirpt를 이용해서 JavaScirpt의 코드에 따라 속성이 추가되면서 디자인을 바꾸는 등의 효과를 줄 수 있다.


### <mark>SCRIPT</mark>  

```javascript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        document.write(1+1);  //  2를 출력
    </script>
    <h1>html</h1>
    1+1                      <!-- 1 + 1 출력 -->
</body>
</html>
```

<i class="fa fa-chevron-circle-right" style="color:black"></i> 스크립트 태그 안에 있는 코드는 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> JavaScript</span>로 해석한다.  

### <mark>EVENT</mark>  

```javascript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <input type="button" value="hi" onclick="alert('hi')">   <!-- 'hi' 라는 버튼을 만들고 누르면 'hi' 라고 출력-->
    <!-- onclick 속성의 속성값으로는 JavaScript가 와야한다. | onclick의 속성에 속성값은 웹 브라우저가 기억하고 있다.-->
    <input type="text" onchange="alert('changed')">
    <!-- 텍스트 칸에 값을 적고 웹페이지에서 빠져 나오는 순간 메세지 출력 -->
    <input type="text" onkeydown="alert('key down')">
    <!-- 텍스트 칸에 키를 아무거나 누르면 메세지 출력 -->
</body>
</html>
```

<i class="fa fa-search" style="color:#01077c"></i><mark> Event?</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> 웹브라우저 위에서 일어나는 일을 의미한다. (ex :: onclick, onchange, onkeydown)

### <mark>Console</mark>  
<i class="fa fa-chevron-circle-right" style="color:black"></i> 개발자 도구에 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> Console</span> 창에서 JavaScirpt를 즉석해서 만들어서 사용이 가능하다.

![콘솔 JS](https://user-images.githubusercontent.com/76092057/105638220-d3795300-5eb4-11eb-9002-05ed8189d49a.PNG){: width="100%" height="100%"}

<i class="fa fa-chevron-circle-right" style="color:black"></i> JS는 이미 만들어진 사이트에서 JS를 통해 자신에게 필요에 맞는 코드를 작성해 원하는 정보를 얻을 수 있다.

<span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> END</span>
---