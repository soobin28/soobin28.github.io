---
layout: post
title:  "Project #4"
date:   2019-04-18
description: 홀로그램을 활용한 헬스케어 서비스
---

<p class="intro">홀로그램을 활용한 헬스케어 서비스</p>
개발기간 : 2018.09 ~ 2018.12 (약 3개월)

#### 프로젝트 개요

* 꾸준한 운동으로 인해 변화되어지는 모습을 데이터로 쌓고, 쌓아 놓은 데이터를 바탕으로 향후 달라질 모습을 예측하여 보여주는 프로그램을 개발.
* 본 연구는 기존의 체성분 분석기를 이용하여 사용자의 체성분을 분석한 뒤 이를 Unity에서 Morph 기술을 통해 3D 콘텐츠에 반영하고 그 결과를 홀로그램을 이용하여 가시적으로 나타내줌으로써, 이를 이용하는 사용자에게 보다 명확한 가이드를 제공하며, 운동을 지속적으로 할 수 있게 동기 부여 해주는 서비스를 구현하는 것을 목표로 함.
<br/>

#### 담당업무

* 데이터베이스
    * 체성분 측정 시 나오는 결과 데이터를 기반으로 데이터 저장
    * 엑셀파일로 저장된 측정 값을 서버를 통해 Json 형태로 변환 후, 파이어베이스 저장
    * 데이터베이스(Firebase)와 Unity 연동

<br/>

#### 개발환경

* Contents : Unity
* DMBS : Firebase
* server : Node.js
<br/>

#### 프로젝트 설계

<figure>
    <img src="/assets/img/urp개념.jpg" alt=""/>
    <figcaption>시스템 개념도</figcaption>
</figure>

* 사용자의 ­체성분 측정 데이터를 데이터베이스에 저장한다.
* 저장한 데이터를 통해 사용자의 체형을 유니티를 통해 모델링 한다.
* 사용자 체형을 3D 모델링한 결과를 홀로그램을 통해 시각적으로 보여주도록 한다.

<figure>
    <img src="/assets/img/인바디.jpg" alt=""/>
    <figcaption>인바디 결과지 샘플</figcaption>
</figure>

* ­체성분 측정 시 나오는 결과 데이터를 기반으로 데이터 저장

<figure>
    <img src="/assets/img/json.jpg" alt=""/>
    <figcaption>데이터베이스 구조</figcaption>
</figure>

* ­Unity와 연동하여 사용하기 위해 서버구축이 필요 없는 클라우드 호스팅 데이터베이스인 Firebase 실시간 데이터베이스를 이용
* Firebase의 데이터 구조는 Json의 형태로 저장이 되기 때문에 체성분 측정을 하는 사용자의 회원번호로 데이터를 구분하며, 회원번호 밑에 날짜를 하위노드로 지정하여 날짜 별로 신체의 변화를 볼 수 있도록 함


<br/>

#### 개발결과 
<br/>

<figure>
    <img src="/assets/img/글리치효과.jpg" alt=""/>
    <figcaption>글리치효과 적용한 남/녀 기본모델</figcaption>
</figure>

* Asset Store 내의 무료 에셋을 통해 뼈대를 구성하고, 글리치 효과를 입혀 남/녀 모델을 제작함.

<figure>
    <img src="/assets/img/컨텐츠.jpg" alt=""/>
    <figcaption>컨텐츠 구현결과</figcaption>
</figure>

* Unity를 작동시켰을 때 바로 Firebase DB에 연동이 되고, Firebase DB내의 데이터 파일들을 불러와 사용자의 데이터를 원하는 morph 기능에 연결시켜 바로 변화 된 모습을 보여줄 수 있게 구현함.

<figure>
    <img src="/assets/img/db값.jpg" alt=""/>
    <figcaption>DB 사용자 예시</figcaption>
</figure>

* Firebase DB에 사용자별(1,2)로 데이터를 저장시키고 사용자 안에서 날짜별로 데이터를 저장시킴
* 초기 MySQL Database를 이용하여 데이터베이스를 구축하려 했으나, 실시간 연동이란 장점과 서버가 필요 없는 장점을 가진 Firebase DB로 변경함.

<figure>
    <img src="/assets/img/excel.jpg" alt=""/>
    <figcaption><br/>excel 파일 -> Firebase DB 웹을 통한 삽입</figcaption>
</figure>

* 사용자가 체성분분석 후 저장된 엑셀 형식의 파일을 json으로 변환 후 DB로 보내야하는 불편함을 해소하기 위해, NodeJS를 통해서 엑셀파일을 지정하면 Firebase DB에 엑셀파일이 사진과 같이 삽입할 수 있도록 별도의 프로그램을 구현함.

<br/>


