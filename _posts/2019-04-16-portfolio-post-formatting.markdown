---
layout: post
title:  "Project #3"
date:   2019-04-17
description: 비콘을 이용한 건강검진 관리 시스템의 설계와 개발
---

<p class="intro">비콘을 이용한 건강검진 관리 시스템의 설계와 개발</p>
개발기간 : 2018.03 ~ 2018.06 (약 3개월) 

#### 프로젝트 개요

일반적으로 사람들은 정기적으로 건강검진을 실시하여 건강 상태를 확인합니다. 그러나 검사실의 간호사들은 검사자들의 도착을 알지 못하기 때문에 검사자들이 스스로 도착을 알려야 합니다. 본 프로젝트에서는 검사자가 검사실의 사전 정의된 반경내에 있을 때, 이를 식별하여 자동으로 검사 접수를 해주고, 검사자에게 대기에 대한 정보를 제공합니다.

<br/>

#### 담당업무
<p> 프로젝트 설계 및 개발 </p>

<br/>

#### 개발환경

* BE : Node.js (Express)
* FE : Html, CSS, JavaScript
* App : Android Studio
* DBMS : MySQL

<br/>

#### 프로젝트 설계

<table frame=void>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/diagram.jpg" alt=""/>
                <figcaption>시스템 모듈 구성도</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            각 클라이언트와 서버에는 여러 모듈이 존재하며, 클라이언트-서버 간 연결을 위한 모듈과 요청과 응답이 발생할 때마다 데이터 처리가 모듈에 의해 이루어진다.
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/개념도.jpg" alt=""/>
                <figcaption>시스템 개념도</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            본 프로젝트에서는 검사를 받으러 온 사용자들을 비콘을 통해 자동으로 검사 접수를 해 주는 시스템을 설계하고 구현한다.
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/class.jpg" alt=""/>
                <figcaption>클래스다이어그램</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            클래스 다이어그램은 회원 클래스, 관리자 클래스, 의사 클래스, 건강검진 어플 클래스로 구성된다. 
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/erd.jpg" alt=""/>
                <figcaption>E-R 다이어그램</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            데이터베이스는 총 8개의 테이블로 구성된다.
        </td>
    </tr>
</table>

<br/>

#### 개발결과 
##### Web 

<table>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/watinglist.jpg" alt=""/>
                <figcaption>건강검진 관리 홈화면 (img)</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/list.jpg" alt=""/>
                <figcaption>건강검진 리스트 안내 화면(회원), </figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/watinglist.jpg" alt=""/>
                <figcaption>건강검진 대기자화면</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/list.jpg" alt=""/>
                <figcaption>건강검진 리스트 안내 화면</figcaption>
            </figure>
        </td>
    </tr>
</table>

웹페이지에서는 **각 사용자별로 안내**를 해준다. **회원**에게는 건강검진에 대한 정보와 예약을 할 수 있는 페이지를 제공한다. **의사**로 로그인을 할 경우에는 본인이 담당하고있는 검사들의 내용을 보여주고, 현재 진행중인 검사에 대한 대기자 리스트와 검사완료 처리를 할 수 있는 기능이 제공된다. **관리자**에게는 회원과 의사에게 보여지는 내용에 대한 것들을 관리한다. 

##### App

<table>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/watinglist.jpg" alt=""/>
                <figcaption>건강검진 관리 홈화면 (img)</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/list.jpg" alt=""/>
                <figcaption>건강검진 리스트 안내 화면(회원), </figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/watinglist.jpg" alt=""/>
                <figcaption>건강검진 대기자화면</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/list.jpg" alt=""/>
                <figcaption>건강검진 리스트 안내 화면</figcaption>
            </figure>
        </td>
    </tr>
</table>

어플에서는 현재 받아야 하는 검사에 대한 안내를 받는다. **검사 이름과 검사실의 위치, 예상 소요 시간** 등을 안내한다. 만약 핸드폰이 **비콘과 통신**을 할 경우, 사용자가 받으러 온 검사에 **대기 중인 사람의 수**를 보여주고 회원이 대기를 해야 하는 **대기 예상 시간**을 보여준다.

<br/>
### 논문

* 2018년도 한국컴퓨터정보학회 하계학술대회 구술발표 참여, 우수논문상 수상

 <figure>
    <img src="/assets/img/ksci.jpg" alt=""/>
    <figcaption>KSCI 우수논문상</figcaption>
</figure> 

<br/><br/><br/>

