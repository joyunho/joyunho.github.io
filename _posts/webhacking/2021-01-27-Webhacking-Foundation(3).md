---
layout: post
current: post
cover:  assets/built/images/Webhacking_logo.jpg
navigation: True
title: Webhacking_Foundation(3)
date: 2021-01-28 18:07:00 +0900
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

### <mark>PHP의 변수</mark>

```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<?php
    $a = 10;        // 변수 지정할 떄 사용하는 기호 :: '$'
    echo $a+1;      // 10(a) + 1 == 11 출력
?>
</body>
</html>
```

<i class="fa fa-chevron-circle-right" style="color:black"></i> 변수를 지정할 때는 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> '$'</span> 를 사용하여 지정한다.  

### <mark>++ 변수의 사용 이유</mark>  

<br>
> Lorem ipsum dolor sit amet consectetur adipisicing elit.
Pariatur explicabo joho labore assumenda, ipsum ad illum accusamus. 
Consectetur animi, reiciendis expedita maiores tempore error dolores, 
illo deserunt est joho distinctio!Dolorem doloremque consectetur 
earum voluptatem molestias laborum sit quas, magni autem joho porro et neque! 
joho ducimus corrupti ex quo aliquam eum sit, joho, impedit dicta, 
aliquid reprehenderit suscipit.

<i class="fa fa-chevron-circle-right" style="color:black"></i>
'joho' 라는 글자를 'yunho' 라고 고치고 싶지만, 하나씩 수정해야 해서 효율성이 떨어지고, 
모두 제대로 변환되었는지 확신하기 힘들다.  

```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<h1>Variable</h1>
<?php
$name = "yunho";
echo "Lorem ipsum dolor sit amet consectetur adipisicing elit.
Pariatur explicabo $name labore assumenda, ipsum ad illum accusamus. 
Consectetur animi, reiciendis expedita maiores tempore error dolores, 
illo deserunt est $name distinctio!Dolorem doloremque consectetur 
earum voluptatem molestias laborum sit quas, magni autem $name porro et neque! 
$name ducimus corrupti ex quo aliquam eum sit, $name, impedit dicta, 
aliquid reprehenderit suscipit $name?"  // 아무 의미 없는 텍스트 :: Lorem 
?>
</body>
</html>
```

<i class="fa fa-chevron-circle-right" style="color:black"></i>
이와 같이 변수를 만들어서 변환을 시키면 간단하고 확실하게 변환 시킬 수 있다.  

### <mark>PHP의 URL 파라미터</mark>

<br>

<i class="fa fa-search" style="color:#01077c"></i> 
<mark>URL 파라미터에 값을 넣어 페이지에 반영하는 방법</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> 
GET 메소드를 이용하여 PHP 코드를 만든 다음, URL 파라미터에 형식을 맞추어서 값을 넣는다.  

```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    안녕하세요. <?php echo $_GET['address']; ?>에 사시는   <!-- GET 메소드 이용 -->
    <?php echo $_GET['name']; ?>님.  
</body>
</html>
```

> URL 파라미터 값 :: http://127.0.0.1/parameter.php?name=yunho&address=%EC%84%9C%EC%9A%B8

<i class="fa fa-hand-o-right" style="color:#008080"></i>  <**결과**>
![PHP URL 파라미터](https://user-images.githubusercontent.com/76092057/106120927-50008000-619a-11eb-91b3-6a1cf77cf1f6.PNG){: width="100%" height="100%"}

### <mark>++ URL 파라미터 활용</mark>  

```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>WEB</h1>
    <ol>
        <li><a href="index.php?id=HTML">HTML</a></li>
        <li><a href="index.php?id=CSS">CSS</a></li>
        <li><a href="index.php?id=JavaScript">JavaScript</a></li>
    </ol>
    <h2>
        <?php
        echo $_GET["id"];
        ?>
    </h2>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
    Error nostrum architecto, ut amet ratione voluptatum veritatis 
    accusamus eos voluptatem ex cum quo magnam consequatur obcaecati corporis 
    culpa consequuntur totam esse!Officia quasi debitis ex possimus porro tempora qui harum nisi. 
    Veniam rerum minima ut eius consequatur cum accusamus id saepe nesciunt tempore sequi, 
    aspernatur sint tempora natus, iure sed nobis!
</body>
</html>
```

<i class="fa fa-hand-o-right" style="color:#008080"></i>  <**결과**>
![PHP URL 파라미터 최종본](https://user-images.githubusercontent.com/76092057/106130362-96f37300-61a4-11eb-9125-d1459a94ee90.PNG)
{: width="100%" height="100%"}

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> MySQL  
===  

<br>

### <mark>MySQL 테이블의 구조</mark>

![MySQL 테이블 구조](https://user-images.githubusercontent.com/76092057/106236468-49c4df00-6240-11eb-9500-89627b098901.PNG){: width="100%" height="100%"}

<i class="fa fa-chevron-circle-right" style="color:black"></i>
이 테이블은 2행과 4열로 이루어져 있다.

### <mark>++ MySQL 테이블 생성</mark>  

<br>

> 내가 만들 테이블
![MySQL 테이블 만들기](https://user-images.githubusercontent.com/76092057/106237891-1e8fbf00-6243-11eb-87f7-4986f4ce1ec9.PNG)

```SQL
mysql> CREATE TABLE topic(
    ->   id INT(11) NOT NULL AUTO_INCREMENT,  --  (1)
    ->   title VARCHAR(100) NOT NULL,         --  (2)
    ->   description TEXT NULL,               --  (3)
    ->   created DATETIME NOT NULL,           --  (4)
    ->   author VARCHAR(30) NULL,             --  (5)
    ->   profile VARCHAR(100) NULL,           --  (6)
    ->   PRIMARY KEY(id));                    --  (7)
```

1. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> id 칼럼</span>은, 식별칼럼으로서, 보통 11자리수 까지 반영하며, 빈칸이어선 안되며, 자동적으로 1씩 증가하도록 설정해야한다.
2. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> title 칼럼</span>은, 제목은 길지 않아도 되며(100), 빈칸이어선 안된다.
3. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> description(본문)</span> 칼럼은, 길어야 하므로(65,000 문자를 허용하는 TEXT), 내용이 없는 것도 허용함.
4. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> create(생성시간)</span> 칼럼은, 날짜 시간을 모두 허용하는(DATETIME)을 사용하고, 빈칸이어선 안된다.
5. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> author(저자)</span> 칼럼은, 문자인데 30글자 안으로 자르면 좋다.(VARCHAR(30))
6. <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> profile(프로필)</span> 칼럼은, 길 필요가 없으니 100글자 정도로 허용하고, 빈칸 허용.

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> JavaScript 
===  

<br>

### <mark>JS 문자열과 숫자</mark>

![JS 문자열과 숫자](https://user-images.githubusercontent.com/76092057/106241608-af699900-6249-11eb-9d06-f9aeab22620f.PNG){: width="100%" height="100%"}

<i class="fa fa-chevron-circle-right" style="color:black"></i>
개발자 도구 콘솔창에서 문자열과 숫자 입력 및 출력<br>(**포인트** :: 구글링으로 문법을 검색해서 형식을 알아볼 것!)

### <mark>JS 변수와 대입 연산자</mark>  

<br>

<i class="fa fa-search" style="color:#01077c"></i> 
<mark>변수(Variable)</mark>   
<i class="fa fa-envelope-o" style="color:red"></i>
변수는 데이터를 저장하는 장소이며, 데이터를 읽고 수정할 수도 있다.

> var name = "joho";

<i class="fa fa-search" style="color:#01077c"></i> 
<mark>대입 연산자(Operator)</mark>   
<i class="fa fa-envelope-o" style="color:red"></i>
대입 연산자("=")는 오른쪽의 값을 왼쪽의 변수에 저장한다. 대입 연산자 왼쪽에는 값을 저장할 수 있는 변수가 위치하고 대입연산자의 오른쪽에는 변수에 저장할 값이 위치한다.

> int x = 100;  

<span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> END</span>
---