# 🙌 DB정리!

## ❓ 데이터란 ❓

#### DATA(자료) : 관찰, 검색 또는 측정을 통해 수집되는 사실이나 값

#### 정보 : 자료의 유효한 해석, 지식

## ❓ DB는 어디에 쓰일까 ❓

![title](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRSRm-cIeMWdV-RGOctwzMTRHMX77mZSZqHZA&usqp=CAU)

#### 간단히 말해서 데이터를 전달해줍니다 !!

## ❓ 일괄 처리 시스템 ❓

#### 데이터를 수집해서 분류하고 정렬시킨 다음에 일괄 처리하는 데이터 처리 방법

## ❓ 온라인 처리 시스템 ❓

#### - 데이터가 생성되는 즉시 전송하여 컴퓨터가 즉시 처리하는 시스템

#### - 하나의 데이터베이스에서 처리

## ❓ 분산 처리 시스템 ❓

#### - 여러 개의 데이터베이스에서 처리하고 통신 네트워크로 공유하는 시스템

#### - 온라인 처리 시스템 보다 효율적인 시스템 !

## ❓ 데이터베이스란 ❓

#### 여러 응용 시스템들이 공용할 수 있도록 <span style="color:red">통합 저장된 운영 데이터</span>

## ❓ 데이터베이스의 정의 (SISO) ❓

### - 저장 데이터 (Stored Data)

### - 통합 데이터 (Integrated Data)

### - 공용 데이터 (Shared Data)

### - 운영 데이터 (Operational Data)

<hr>

### 저장 데이터 (Stored Data)

##### 문서 보관이 아닌 하드디스크나 서버에 저장되어 있는 데이터를 의미

### 통합 데이터 (Integrated Data)

##### - 여러 곳에서 사용하던 데이터가 하나로 저장된 데이터를 의미

##### - 똑같은 데이터가 중복되어 있지 않습니다

### 공용 데이터 (Shared Data)

##### - 공용으로 사용되는 데이터를 의미

##### - 여러 사용자들이 서로 다른 목적으로 데이터베이스의 데이터를 공동으로 이용합니다

##### - 데이터의 양 대규모화

### 운영 데이터 (Operational Data)

##### - 조직의 목적을 위해 사용되는 데이터를 의미

##### - 단순한 입출력 데이터나 일시적으로 생성된 임시 데이터는 운영데이터가 아니다

## ❓ 데이터베이스의 특정 (rccc) ❓

### - 실시간 접근성 (real-time accessibility)

### - 계속적인 변화 (continuous evolution)

### - 동시 공용 (concurrent sharing)

### - 내용에 의한 참조 (contents reference)

<hr>

### 실시간 접근성 (real-time accessibility)

##### - 데이터베이스는 실시간으로 서비스

##### - 사용자가 요청하는 순간 바로 서비스를 해준다

### 계속적인 변화 (continuous evolution)

##### - 데이터는 계속 바뀝니다

##### - 데이터베이스는 삽입, 삭제, 수정 등의 작업으로 바뀐 값을 저장

### 동시 공용 (concurrent sharing)

##### - 서로 다른 사용자에게 동시에 공유된다.

##### - 동시에 공유되기 때문에 여러 가지 문제점

##### - 따라서 문제점 해결을 위해 종속성, 중복성 해결해야 함

### 내용에 의한 참조 (contents reference)

##### - 저장된 데이터의 주소가 아닌 데이터 값을 참조한다

##### - 사용자가 조건(쿼리)을 제시하면 DB는 데이터 검색해서 보내줌

## ❓ 파일 시스템 ❓

#### 각 응용 프로그램이 독립적으로 자료를 파일형태로 관리

##### [1 - 3 담임선생님의 1-3학생들 파일과 ○○○선생님의 1-3학생들 파일은 다를 수 있다]

## ❓ 데이터 중복성 ❓

#### - 한 시스템 내의 자료가 중복 저장되어 추가적인 저장 공간이 필요하다

#### - 자료를 비효율적으로 관리하는 것이며, 비용이 증가됨

##### ==> 응용 프로그램마다 별도로 독립된 파일을 가지기 때문

## ❓ 데이터 종속성 ❓

#### 자료 간의 상호 의존도가 높아서 하나의 파일을 변경하면 관련된 파일도 변경해야 한다

## ❓ DBMS ❓

### 장점 ❓

##### 1 - 데이터를 공유하기 때문에 종속성 문제해결

##### 2 - 중복 제거로 데이터 일관성 유지

##### 3 - 데이터 복구, 보안이 쉬움

##### 4 - 하나의 갱신 작업만 수행해도 되기 때문에 경제성 좋음

### 단점 ❓

##### 1 - DBMS, CPU, 메모리 용량 등 비용 발생

##### 2 - 복잡한 백업과 회복 -> 처음부터 잘 해야함 !!

##### 3 - 시스템 취약성 -> DB 공격 당하면 끝..

## ❓ DBMS의 기능 ❓

### - 데이터 정의

### - 데이터 조작

### - 데이터 제어

<hr>

### 데이터 정의

##### 데이터의 구조를 정의하고 데이터 구조에 대한 삭제 및 변경 기능 수행

### 데이터 조각

##### 데이터의 검색, 삽입, 수정, 삭제 작업을 지원

### 데이터제어

##### 데이터베이스 사용자를 생성하고 모니터링하며 접근을 제어

##### <span style="color:red">백업과 회복, 동시성 제어</span>

## ❓ 데이터 정의어 (DDL) ❓

#### SQL의 CREATE, ALTER, DROP과 같이 구조를 정의

## ❓ 데이터 조작어 (DML) ❓

#### SQL의 SELECT, INSERT, DELETE, UPDATE문과 같이 데이터를 검색, 삽입, 삭제, 수정하는 데 사용

## ❓ 데이터 제어어 (DCL) ❓

#### SQL의 GRANT, REOKE 문과 같이 데이터의 사용 권한을 관리

<hr>

## ❓ DBMS의 사용자들 ❓

### - 일반 사용자

### - 응용 프로그래머

### - DBA

<hr>

### 일반사용자

##### 데이터의 검색, 삽입, 수정 작업을 하는 사용자 Web이나 App에서 클릭만을 조회하는 사람

### 응용 프로그래머

##### - 일반 사용자가 사용할 수 있도록 프로그램 만드는 사람

##### - SQL 번역해서 일반사용자가 원하는 데이터를 DBMS에 접근하도록 도와주는 사람

### DBA (Database Administrator)

##### - 데이터베이스 총괄 책임자

##### - 데이터 <span style="color:red">설계</span>, <span style="color:red">구현</span>, <span style="color:red">유지보수</span> 전 과정 담당

##### - 사용자 통제, 보안, 성능 모니터링, 데이터 관리

## ❓ 사용자 별 갖추어야 할 지식 ❓

#### 일반사용자는 SQL 언어, 프로그래밍 언어, DBMS 지식, 데이터구성을 몰라도 됩니다

#### 응용 프로그래머는 SQL 언어, DBMS 지식, 데이터 구성은 알아야 하지만 프로그래밍 언어는 몰라도 됩니다

#### DBA는 SQL 언어, 프로그래밍 언어, DBMS 지식, 데이터 구성 모두 다 알아야합니다.

## ❓ 스키마 ❓

#### 데이터베이스의 구조와 제약조건에 대해 나타낸 대략적인 계획이나 도식

## ❓ 스키마의 종류 ❓

### - 개념 스키마

### - 내부 스키마

### - 외부 스키마

<hr>

### 개념 스키마

##### 전체 데이터베이스의 정의를 말하며 하나만 존재

### 내부 스키마

##### 물리적 저장 위치에 데이터베이스의 저장 위치를 알려준다

### 외부 스키마

##### 각 사용자나 응용 프로그래머가 각자 필요한 논리적 구조를 정의 (=뷰)

#### 개념 스키마, 내부 스키마, 외부 스키마 구성

##### ![title](https://t1.daumcdn.net/cfile/tistory/132497364F600AF40B)

<hr>

## ❓ 릴레이션 ❓

#### 릴레이션 : 테이블(표)

#### 릴레이션 스키마 : 속성들의 집합

#### 릴레이션 인스턴스 : 데이터들의 집합

### 릴레이션 각종 용어들 정리

##### ![title](data:image/png;base64,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)
