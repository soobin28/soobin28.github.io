---
layout: post
title:  "Project #3"
date:   2019-04-17
description: 대용량 DB를 이용한 클라이언트 개발
---

<p class="intro">대용량 DB를 이용한 클라이언트 개발</p>
개발기간 : 2017.09 ~ 2017.12 (약 3개월)

#### 프로젝트 개요

대용량 데이터베이스를 이용하여 대학교학사관리시스템의 클라이언트를 응용 개발하는 것을 목표로 함.

<br/>

#### 담당업무

1. 요구사항에 따라 필요한 데이터를 찾아 쿼리 작성.
2. 각 페이지 마다 필요한 데이터를 불러오기 위해 페이지에 해당되는 Service파일에서 Dao파일로 객체 전송
3. Dao 파일에서 객체에 대한 데이터 코드를 작성하여 처리결과 객체를 Service 파일로 전송


<br/>

#### 개발환경

<table>
    <tr>
        <td>구분</td>
        <td>버전</td>
        <td>비고</td>
    </tr>
    <tr>
        <td>JAVA</td>
        <td>JDK1.8 이상</td>
        <td>기본 JAVA Compiler 버전을 정의함.</td>
    </tr>
    <tr>
        <td>Development Tool</td>
        <td>Eclipse Neon 4.6x</td>
        <td></td>
    </tr>
    <tr>
        <td>형상관리</td>
        <td>SVN</td>
        <td>형상관리를 위한 도구로, SVN을 사용한다.</td>
    </tr>
    <tr>
        <td>라이브러리 관리</td>
        <td>Maven3.3.9</td>
        <td>표준 라이브러리 관리를 위해 Maven3.3 이상 버전을 사용하도록 한다.</td>
    </tr>
    <tr>
        <td>표준 Framework</td>
        <td>eGovFramework3.5.1</td>
        <td>전자 정부 표준 프레임워크 3.5.1 버전을 적용한다.
        (주요 구성항목 : Spring Framework)</td>
    </tr>
    <tr>
        <td>RDBMS</td>
        <td>Oracle 11g</td>
        <td>Database는 제안 DBMS인 Oracle 11g 버전을 적용한다.</td>
    </tr>
</table>


<br/>

#### 프로젝트 설계

<table>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/diagram.jpg" alt=""/>
                <figcaption>시스템 모듈 구성도</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/개념도.jpg" alt=""/>
                <figcaption>시스템 개념도</figcaption>
            </figure>
        </td>
    </tr>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/class.jpg" alt=""/>
                <figcaption>클래스다이어그램</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/erd.jpg" alt=""/>
                <figcaption>E-R 다이어그램</figcaption>
            </figure>
        </td>
    </tr>
</table>

<br/>

#### 개발결과 
<br/>
###### Web 

<table>
    <tr>
        <td>
            <figure>
                <img src="/assets/img/년도.jpg" alt=""/>
                <figcaption>년도-교수 별 개설 교과목 수강학생 학점 현황</figcaption>
            </figure>
        </td>
        <td>
            <figure>
                <img src="/assets/img/학과.jpg" alt=""/>
                <figcaption>학과(학부)별 학생 성적 그래프 </figcaption>
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

<br/>


<br/><br/>

