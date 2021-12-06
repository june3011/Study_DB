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

## ❓ KEY ❓

#### 식별한다는 의미 !!!

#### 키로 인해 특정 튜플을 식별할 때 사용하는 속성을 말한다

## ❓ 키의 종류 ❓

### - 슈퍼키

### - 후보키

### - 기본키

### - 대체키

### - 외래키

<hr>

### 슈퍼키 (Super Key)

##### 튜플을 유일하게 식별할 수 있는 <span style="color:red">최소한</span>의 속성 집합

### 후보키 (Candidate Key)

##### 튜플을 유일하게식별할 수 있는 속성의 <span style="color:red">최소</span> 집합

### <span style="color:red">기본키 (Primary Key) </span>

#### 여러 후보키 중 하나를 선정하여 사용하는 대표 키

##### - 후보키 중 마음대로 선택 가능 <span style="color:red">잘 선택하기 !!!</span>

##### - 튜플을 식별할 수 있는 고유한 값

##### - <span style="color:red">NULL값 허용 X</span>

##### - 키 값 변동

##### - 최대한 적은 수의 속성을 가진 것

### 대체키 (Alternate Key)

##### 기본키를 제외한 나머지 후보키

![title](https://mblogthumb-phinf.pstatic.net/20151215_173/hj_veronica_1450161230641pj2HE_JPEG/4.png?type=w800)

### 외래키 (Foreign Key)

##### 다른 릴레이션을 참조할 때 참조하는 기본키

<hr>

## ❓ DBA (Database Administrator) ❓

#### 데이터베이스 총괄 책임자

#### 데이터 <span style="color:red">설계</span>, <span style="color:red">구현</span>, <span style="color:red">유지보수</span> 전 과정 담당

#### 사용자 통제, 보안, 성능 모니터링, 데이터 관리

## ❓ 릴레이션 ❓

### - 릴레이션 : 테이블(표)

### - 릴레이션 스키마 : 속성들의 집합

### - 릴레이션 인스턴스 : 데이터들의 집합

### <span style="color:royalblue">용어 정리표</span>

![title](https://t1.daumcdn.net/cfile/tistory/21073B4C5891F91D11)

## ❓ 무결성 제약조건 ❓

### - 도메인 무결성 제약조건

### - 개체 무결성 제약조건

### - 참조 무결성 제약조건

<hr>

### 도메인 무결성 제약조건

##### - 각 애트리뷰트들의 도메인에 지정된 값만을 가져야 한다는 조건

##### - SQL문을 작성할 때 Type, Null, default, check 등을 사용하여 지정

### 개체 무결성 제약조건

##### 기본키의 조건을 지켜야 한다는 제약조건

### 참조 무결성 제약조건

#### 외래키의 조건을 지켜야 한다는 제약조건

##### - 부모 릴레이션의 기본키를 그대로 사용해야함

##### - 부모 릴레이션과 다른 값을 삽입, 수정할 때 거부

##### ==> 옵션 붙음 (RESTRICTED(거부), CASCADE(연쇄), DEFAULT(초기값), NULL(NULL값으로))

###### <span style="color:royalblue">무결성 제약 조건</span>

![title](https://t1.daumcdn.net/cfile/tistory/9943B5365B36449C2F)

## ❓ 관계대수 ❓

#### 관계형 데이터베이스 내에서 원하는 정보를 어떻게 찾아 낼 수 있는가를 기술하는 절차적인 언어

![title](https://mblogthumb-phinf.pstatic.net/20111010_13/albertx_1318217617115XbJRz_PNG/relational_algebra_01.png?type=w2)

![title](https://mblogthumb-phinf.pstatic.net/20111010_82/albertx_131821947000295a57_PNG/relational_algebra_02.png?type=w2)

## ❓ 셀렉트 ❓

#### - 릴레이션에서 주어진 조건에 만족하는 튜플을 선택하는 연산자

#### - 셀렉트, 시그마라고 읽음

![title](https://mblogthumb-phinf.pstatic.net/data18/2006/5/25/47/select_01-jinsol1.gif?type=w420)

![title](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTit5GvDtEoJREOitY-WjxY-FveePZ9AHYnMZLeTVP47ba_IoitcTRpMIX78sJ-djYAsA&usqp=CAU)

##### 셀렉트 예시

![title](https://mblogthumb-phinf.pstatic.net/data17/2006/5/25/100/select_03-jinsol1.gif?type=w420)

## ❓ 프로젝트 ❓

#### - 필요한 속성들만 추출하는 연산

#### - <span style="color:red">중복 제거</span>

![title](https://datacadamia.com/_media/algebra_of_tables.jpg?cache=)

## ❓ 디비전 ❓

#### 2개의 릴레이션에서 피연산 릴레이션의 속성값을 모두 가진 연산 릴레이션의 속성을 제외한 속성만을 구하는 연산

![title](https://media.vlpt.us/images/odh0112/post/6898db84-185a-46c5-8b13-79a031bcb09a/%EB%94%94%EB%B9%84%EC%A0%84.PNG)

## ❓ 합집합 (유니온, U) ❓

#### - 두 릴레이션을 합하여 하나의 릴레이션으로 반환

#### - <span style="color:red">중복 제거</span>

##### <span style="color:red">중복을 제거한 모든 것</span>

## ❓ 교집합 (U거꾸로) ❓

#### 두 릴레이션 모두 속한 튜플들로 이루어진 릴레이션

##### <span style="color:red">두개 중에 겹치는 것만</span>

![title](https://t1.daumcdn.net/cfile/tistory/277BF03D592068A82E)

## ❓ 차집합 (-) ❓

#### 피연산, 릴레이션에 속하지 않은 튜플들로 이루어진 릴레이션

![title](https://blog.kakaocdn.net/dn/ey3ZNn/btqwFRebZmF/vKcbhTDwBKhvTeBocqMWYK/img.png)

## ❓ 카티션프로덕트 (X) ❓

#### - 연산 릴레이션과 피연산 릴레이션을 곱하는 것

#### - <span style="color:red">중복 허용</span>

<hr>

##### <span style="color:royalblue">카티션프로덕트 예시</span>

![title](https://mblogthumb-phinf.pstatic.net/data18/2006/5/26/14/cartProd_01-jinsol1.gif?type=w210)

<hr>

## ❓ 조인이 필요한 이유 ❓

#### - 카티션 프로덕트를 하면 매우 많은 튜플이 생성됨

#### - 필요한 자료만 보기 위해 조인 사용

### 자연조인

##### - 동등 조인 결과로 얻어진 불필요한 애트리뷰트 제외한 조인

##### - <span style="color:red">중복 애트리뷰트 제거</span>

### 세미조인

##### - 자연조인을 한 후 두 릴레이션 중 한쪽 릴레이션 결과만 반환

##### - <span style="color:red">기호가 닫힌 쪽 튜플만 반환</span>

#### <span style="color:royalblue">자연조인 세미조인 예시</span>

![title](https://slidesplayer.org/slide/15518863/93/images/17/%EF%83%B8+%EC%9E%90%EC%97%B0%EC%A1%B0%EC%9D%B8%EA%B3%BC+%EC%84%B8%EB%AF%B8%EC%A1%B0%EC%9D%B8+p108+R+S+%EF%81%90X%E2%88%A9Y%28S%29+A+B+C+B+C+D+B+C+a1+b1+c1+b1+c1+d1+b1+c1.jpg)

### 세타조인

##### - 조인 연산 시 조건이 붙는 조인

##### - ex) <, >, =, <>, <=, >=

### 동등조인

##### - 세타조인의 종류 중 조건이 =일 경우

### 외부조인

##### - 조인연산 시 외부조인 하는 릴레이션의 정보를 버리지 않고 보여줌

##### - <span style="color:red">꼭 필요한 정보들을 남겨두기 위해 사용</span>

##### - 해당 정보가 없는 곳은 null값 채움

###### <span style="color:royalblue">외부조인 예시) (^은 null)</span>

![title](https://media.vlpt.us/images/ieed0205/post/046f61f0-900e-4ce3-8a82-c431232eb2ca/1252152151.PNG)

## 관계대수 정리

![title](https://slidesplayer.org/slide/15713578/88/images/6/%EA%B4%80%EA%B3%84+%EB%8C%80%EC%88%98+%EC%97%B0%EC%82%B0%EC%9E%90.jpg)
