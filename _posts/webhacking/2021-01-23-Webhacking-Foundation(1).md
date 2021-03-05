---
layout: post
current: post
cover:  assets/built/images/Webhacking_logo.jpg
navigation: True
title: Webhacking_Foundation(1)
date: 2021-01-23 06:41:00 +0900
tags: [Webhacking]
class: post-template
subclass: 'post tag-python'
author: JoHo
---

{% include Webhacking-table-of-contents.html %}

---

> 오늘은 세팅을 하기위해 배우기로 한 언어들에 대해 알아보겠습니다.

<i class="fa fa-hand-o-right" style="color:#008080"></i> PHP?
===

<i class="fa fa-chevron-circle-right" style="color:black"></i>
서버측에서 해석되는 <span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> Script</span> 언어  

<i class="fa fa-search" style="color:#01077c"></i><mark> 'Script' 라고 불리는 이유?</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> 서버에서 해석되어지고, ServerSide가 쉽고 인터프리터 되기 때문에 'Script' 라고 불리우는 언어중에 하나가 바로 PHP인 것이다.  

<i class="fa fa-search" style="color:#01077c"></i><mark> 사용하는 이유(장점)</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> PHP언어는 오픈소스이다. 즉, 많은 개발자들에게 접근성이 높다는 의미이고, 누구든 PHP를 활용하여 작업할 수 있다.  
<i class="fa fa-envelope-o" style="color:red"></i> 운영 비용도 저렴하게 유지가 가능하다.  
<i class="fa fa-envelope-o" style="color:red"></i> 진입 장벽이 낮다. 개발 언어가 복잡하지 않기 때문에 보편적으로 개발자 입장에서 언어를 배우기 쉽고 간단하다. ==> <span style="color:red;" >효율성과 생산성 상승</span>

<i class="fa fa-search" style="color:#01077c"></i><mark> PHP의 단점</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> '안정성' 이 낮다. ==> PHP의 장점인 '접근성'떄문에 개발자 외 다른 프로그래머가 접근하기 쉬움 (PHP7.0 이후 많이 개선되었다.)  
<i class="fa fa-envelope-o" style="color:red"></i> 내장 함수나 인자 이름 규칙에 일관성이 없다. ==> 대형 웹사이트 제작에는 적합하지 않다.

<i class="fa fa-chevron-circle-right" style="color:black"></i><mark> 결론</mark>   
여러가지 근거에 의해 현재 PHP언어는 죽어가고 있는 추세이다. 하지만 현 시점에서는 시장에서 배제되고 있지는 않고, Webtutorial 이라는 사이트를 만드는 목적에 알맞는 언어라 생각하기 때문에 공부를 시작하게 되었다.

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> MySQL?
===

<i class="fa fa-chevron-circle-right" style="color:black"></i>
<span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> DateBase</span> 관리 시스템  

<i class="fa fa-search" style="color:#01077c"></i><mark> 사용하는 이유(장점)</mark>   
<i class="fa fa-envelope-o" style="color:red"></i> MySQL은 무료이며, 오픈소스이다.  
<i class="fa fa-envelope-o" style="color:red"></i> 호환성이 좋다. (어떠한 운영체제에서도 사용가능)   
<i class="fa fa-envelope-o" style="color:red"></i> 명령어 자체가 적어서 진입 장벽이 낮다. ==> <span style="color:red;" >효율성과 생산성 상승</span>

<i class="fa fa-search" style="color:#01077c"></i><mark> MYSQL의 단점</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> 깊숙히 자리 잡은 버그와 특이함  
<i class="fa fa-envelope-o" style="color:red"></i> 관계형 테이블의 비유연성  

<i class="fa fa-chevron-circle-right" style="color:black"></i><mark> 결론</mark>   
MYSQL에 대한 공부는 데이터 분석을 진행하기 위해 필요한 기술만큼이나 중요하다. 그 이유는 회사 업무를 하다보면 보통 데이터가 준비가 되어 있지 않으며 직접 데이터를 추출하고 정제해야 하는데 이 때 SQL을 사용한다. 또한 Webtutorial 이라는 사이트를 만드는 목적에 알맞는 언어라 생각하기 때문에 공부를 시작하게 되었다.

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> JavaScript?
===
<i class="fa fa-chevron-circle-right" style="color:black"></i>
웹을 풍부하게 만들어주는 작고 가벼운 언어 

<i class="fa fa-search" style="color:#01077c"></i><mark> 사용하는 이유(장점)</mark>   
<i class="fa fa-envelope-o" style="color:red"></i> 컴파일 과정이 없어서 다른 언어와 비교했을 때 빠른 시간 안에 스크립트 코드를 작성할 수 있게 도와준다.    
<i class="fa fa-envelope-o" style="color:red"></i> 호환성이 좋다. (어떠한 운영체제나 플랫폼에 상관없이 사용가능)   
<i class="fa fa-envelope-o" style="color:red"></i> 단순한 구조와 원칙을 가지고 있어서 진입 장벽이 낮다. ==> <span style="color:red;" >효율성과 생산성 상승</span>

<i class="fa fa-search" style="color:#01077c"></i><mark> JavaScript의 단점</mark>  
<i class="fa fa-envelope-o" style="color:red"></i> 한정된 객체와 객체 함수를 제공한다.  
<i class="fa fa-envelope-o" style="color:red"></i> 브라우저상에 소스가 노출되어서 보안에 취약하며 신경을 많이 써야한다.  

<i class="fa fa-chevron-circle-right" style="color:black"></i><mark> 결론</mark>   
기본적으로 웹사이트 개발을 할 때 필요한 3대장 (HTML, CSS, JavaScript) 중에 하나라서 배우고 싶었고, JS가 없이 만든 사이트는 단순한 웹 문서에 지나지 않는다는 말을 듣고, Webtutorial 이라는 사이트를 만드는 목적에 알맞는 언어라 생각하기 때문에 공부를 시작하게 되었다.

---

<i class="fa fa-hand-o-right" style="color:#008080"></i> HTML, CSS
===
<i class="fa fa-chevron-circle-right" style="color:black"></i>
웹사이트의 골격과 디자인  

이 부분은 기존에 한번 공부를 해보고 정리했던 부분이여서 블로그에 정리를 하는 것 보다 다시 동영상을 보고, 자신의 방식대로 따라한 것을 깃허브에 올리는것을 대체할 생각입니다!
<span style="color:#ff9b15; background-color:#2b2b2b; font-weight:bold;"> END</span>
---
