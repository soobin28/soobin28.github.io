---
layout: post
title:  "Project #1"
date:   2019-04-15
description: 교내 물건 경매∙공유 시스템 
---

<p class="intro">교내 물건 경매∙공유 시스템 </p>
개발기간:  2017.09 ~ 2017.12 (약 3개월) 

#### 프로젝트 개요

* 대학생들의 비싼 교과서 값에 대한 부담감을 줄이고자, 안 쓰는 교재를 가진 사람들의 책을 중고로 사고 팔 수 있는 사이트의 개발
* 기존의 중고거래의 문제점인 1:1 방식 거래진행으로 인한 다른 사람의 참여 불가의 불편함을 해결하고자, 여러 명의 사람이 거래에 참여할 수 있는 방식인 경매 시스템을 합쳐 불편함을 해소
* 사용자들이 가지고 있는 물건 중 가끔 사용을 하여 팔기에는 아깝고 자주 쓰지 않는 물건의 경우, 소정의 대여료를 받고 그 물건이 필요한 사람에게 대여를 해주어 사용자들의 만족감을 높임

<br/>

#### 담당업무
* 프로젝트 설계 (공통) : 시스템구성, 업무기술, UI설계, DB설계 
* 클라이언트가 요구하는 사항에 대한 처리
* 페이지 별 필요한 데이터 관리
* 세션 처리

<br/>

#### 개발환경

* BE : Node.js (Express)
* FE : Html, CSS, JavaScript
* DBMS : MySQL
* IDE : Atom
* DB 설계 Tool : TDM(Toad Data Modeler Freeware)

<br/>

#### 프로젝트 설계

<figure>
    <img src="/assets/img/경매구성도.jpg" alt=""/>
    <figcaption>시스템 구성도</figcaption>
</figure>
 
* 각 시스템의 기능의 단위별로 구성도 제작
<a href="/asset/pdf/데이터베이스설계_시스템요구사항.pdf">시스템 요구사항 분석서</a>

 <figure>
    <img src="/assets/img/tdm.jpg" alt=""/>
    <figcaption>E-R Diagram</figcaption>
</figure>
 
 * 사용자 요구사항을 바탕으로 엔티티 도출 
 * 업무별로 도출된 엔티티와 그의 속성들을 보고 식별이 될 수 있는 속성들을 뽑아 PK 설정
 * 요구사항을 토대로 외래키 관계 지정 후, 외래키 관계에서 삽입, 삭제, 수정시의 업무규칙을 정의.
 * 도메인 정의 및 용어사전 정의를 토대로 속성의 이름 및 도메인 설정
 * 각 시스템의 기능의 단위별로 구성도 제작
<a href="/asset/pdf/데이터베이스설계_ERD.pdf">E-R 다이어그램 설계서</a>

 <figure>
    <img src="/assets/img/mainUI.jpg" alt=""/>
    <figcaption>Main UI 설계</figcaption>
</figure>

1. 사이트의 로고. 이 로고를 클릭하면 로그인이 안 되어있을 경우 이 화면으로 넘어가고 로그인이 되어있을 경우 M-01-02 화면으로 넘어간다.
2. 검색을 하기 전 경매물품을 검색할지 공유물품을 검색할지 정할 수 있다.
3. 검색 키워드를 입력하고 돋보기 버튼을 클릭해 검색을 할 수 있다.
4. 로그인이 안 되어있을 경우 나타나는 화면으로 로그인 화면으로 가거나 회원가입화면으로 가 회원가입을 할 수 있다.
로그인이 되었을 경우 로그아웃과 마이페이지로 넘어갈 수 있는 버튼이 표시된다.
5. 최근에 등록된 순으로 경매물품이 표시된다.
6. 최근에 등록된 순으로 대여물품이 표시된다.
7. 아이디와 비밀번호를 입력하고 로그인을 하거나 회원등록이 되어있지 않을 경우 회원가입버튼을 클릭해 회원가입을 할 수 있다.

또 다른 UI 설계는 <a href="/asset/pdf/데이터베이스설계_UI설계.pdf">UI 설계서</a> 를 참조 해주세요.


<br/>

#### 개발결과 
<br/>
###### Web 

<table>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/main.jpg" alt=""/>
                <figcaption>Main 화면</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            본 프로젝트의 웹 사이트에 접속 시 제일 먼저 보이게 되는 화면이다. 
            가장 최근에 올라온 물건의 순으로 가장 죄측에 올라와 보이게 된다. 상단에는 물건을 검색할 수 있는 검색창이 존재한다.
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/product.jpg" alt=""/>
                <figcaption>물건 리스트 화면</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
           웹 사이트에 올라온 물건리스트를 볼 수 있다. 좌측 스크롤을 통해 물건 리스트를 볼 수 있고, 물건의 사진을 클릭할 경우 우측에 물건에 대한 상세 정보가 나타난다.
           해당 사이트의 접속한 회원이 물건들을 올리면 여기에 올라가게 된다.
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/mypage.jpg" alt=""/>
                <figcaption>My Page 화면</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
           회원이 빌려주거나, 빌린 물건 또는 경매로 구입하거나, 판매하려고 올린 물건에 대한 히스토리를 열람할 수 있다.
           회원정보에 대한 수정이나 회원이 관심 물품으로 등록한 물건에 대한 정보를 볼 수 있다.
        </td>
    </tr>
</table>


<br/><br/><br/>

