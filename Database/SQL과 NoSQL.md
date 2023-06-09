# RDB (Relational DataBase)
스키마가 존재하는 관계형 데이터베이스


- 행과 열로 이루어진 테이블 형태
- MariaDB, MySQL, Oracle, PostgreSql

<br>

## 특징
1. 데이터 중복이 없어 UPDATE에 유리함
2. Forign키 사용
   - 외래키를 통해 다른 테이블과 데이터를 공유하며 관계를 맺음
3. 연산 속도보다 트랜잭션 시 ACID가 중요

<br>

## 성능 높이는 방법
고성능의 하드웨어를 사용하는 Scale-Up(수직적 확장) 방식을 이용함.  
하지만 비용이 많이 들어 RDB는 확장성이 안 좋음

<br><br>

# NoSQL (Not Only SQL)
스키마가 존재하지 않는 비관계형 데이터베이스

- Key-value 형태
- MongoDB, redies

<br>

## 특징
1. 스키마 없음
    - 구조 변경이 자유로워 데이터 분산이 용이함
    - 데이터 중복 문제와 데이터 변경이 오래 걸림  
    → UPDATE가 적고 SELECT가 잦은 환경에서 사용하기 적합함

<br>

2. RDBMS의 단점인 확장성 향상
    - 빅데이터의 등장으로 인해 데이터 일관성은 포기하되 비용을 고려하여 Scale-Out을 목표로 등장

<br>

3. 트랜잭션 관리 안 됨

<br>

## 성능 높이는 방법
여러 대의 컴퓨터에 데이터를 분산하여 저장하는 Scale-Out(수평적 확장)

<br><br>

> ### 내 마음대로 요약
> - RDB는 스키마가 있는 관계형 DB로, 데이터 중복을 허용하지 않아 데이터 수정이 잦은 환경에 적합하다.
> - NoSQL은 스키마가 없는 Key-Value 형태의 DB로 빅데이터를 분산하고, 데이터 조회가 잦은 환경에 적합하다. 확장성이 안 좋은 RDB의 단점을 위해 등장했다.