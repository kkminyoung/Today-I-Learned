# Part01

"소프트웨어융합창의설계", "소프트웨어공학" 수업시간에 배우는 내용도 등장하지만, 익숙하지 않은 개념들이 있어 따로 정리하였다!!

# Chapter01
### 애자일 방법론
1-23p
- 애자일 방법론은 고객의 요구사항 변화에 유연하게 대응할 수 있도록 일정한 주기를 반복하면서 개발 과정을 진행하는 방법론이다.
- 애자일 방법론의 절차
     - 사용자 스토리 -> (계획 -> 개발 -> 승인 테스트)(반복)
       
- 종류
   ```
   1. XP
     - 의사소통 개선과 즉각 피드백으로 품질 향상 
     - 반복 개발 주기
     - 기본 원리 : Pair Programming, 공동코드 소유, 지속적인 통합(CI), 계획세우기, 작은 릴리즈, 메타포어(공통적인 이름 체계와 시스템 서술서를 통해 고객과 개발자 간의 의사소통 원활하게), 간단한 디자인, TDD(테스트 기반 개발), 리팩토링, 40, 고객상주, 코드 표준
 
   2. 스크럼
     - 정해진 시간, 장소에 개발하는 방법
     - 주요 개념 
        - 백로그: 제품과 프로젝트에 대한 요구사항
        - 스프린트 : 짧은 개발 기간으로 반복적 수행
        - 스크럼 미팅 : 데일리미팅
        - 스크럼 마스터 : 리더
        - 스프린트 회고
        - 번 다운 차트 : 남아있는 백로그 대비 시간을 그래픽 적으로 표현한 차트

   3. 린
       - 낭비 요소를 제거하여 품질 향상
       - JIT(Just In Time), 칸반(Kanban) 보드 사용
       - 낭비제거, 품질 내재화, 지식창출, 늦은 확정, 빠른 인도, 사람존중, 전체 최적화
  ```

### 요구사항 분석 자동화 도구
CASE : 소프트웨어, 하드웨어, 데이터베이스, 테스트 등을 통합하여 소프트웨어를 개발하는 환경을 조성
- Upper CASE
   - 계획 수립, 요구분석, 기본설계 단계를 다이어그램으로 표현
   - 모델들 사이의 모순 검사 및 모델의 오류 검증, 일관성 검증 지원
   - 자료 흐름도 프로토타이핑 작성 지원 및 UI 설계 지원
- Lower CASE
   - 구문 중심 편집 및 정적.동적 테스트 지원
   - 시스템 명세서 생성 및 소스코드 생성 지원
- Integrated CASE

### 요구사항 관리도구
```
1-34p

1.상용제품
- 헬릭스 RM
- 지라
- 오르카노스
- 리큐테스트

2.오픈소스
- 레드마인
- 테스트링크
```

# Chapter02
### 용어정리
```
- 리치 클라이언트(X-internet)
- 씬 크라이언트(JSP, HTML 기반)

- 3C 분석(Customer, Company Competitor)
- SWOT 분석(Strength, Waekness, Opportunity, Weakness)

- 시나리오 플래닝
- 페르소나 정의(사용자 요구사항 도출시 잠재적 사용자의 다양한 목적과 관찰된 행동 패턴을 응집시켜놓은 사용자)
- 액츄에이터기술(유체 에너지 이용 기계작업), 마이크로 머시닝(집적회로 제조기술 -> 3차원 구조의 센서를 미세가공), 퍼지 뉴럴 네트워크 기술

- 와이어프레임 : 이해관계자들과의 화면구성을 협의하거나 서비스의 간략한 흐름을 공유하기 위해 화면 단위의 레이아웃을 설계하는 작업
- 스토리 보드 : 정책, 프로세스, 콘텐츠구성, 와이어프레임, 기능정의, 데이터베이스 연동 등 서비스 구축을 위한 모든 정보가 담겨있는 설계 산출물

- GOMS(Goals, Operators, Methods, Selection rules)
```

### UI 설계도구
- 화면 설계 도구
  - 파워 목업, 발사믹 목업, 카카오 오븐
- 프로토타이핑 도구
  - UX핀, 액슈어, 네이버 프로토나우
- UI 디자인 도구
  - 스케치, Adobe XD
- UI 디자인 산출물로 작업하는 프로토타이핑 도구
  - 인비전, 픽사에이트, 프레이머

# Chapter03
- 코드 설계 종류(연상코드, 블록코드, 순차코드, 표의 숫자코드, 십진코드, 그룹 분류식 코드)
- HIPO(Hierarchy Input Process Output) : 하향식 소프트웨어 개발을 위한 문서도구 / 차트(가시적도표, 총체적 도표 세부적 도표)
### 소프트웨어 아키텍처 비용 평가 모델 종류(74p)

![image](https://user-images.githubusercontent.com/61506233/104844809-a1487e00-5915-11eb-8fec-a3e49d9187c0.png)

```
 1. ATAM(Architecture Tradeoff Analysis Method)
 - 아키텍처의 품질속성에 초점을 맞춘 평가기법으로 품질속성 간의 상충관계를 평가
 - 특징
   -> 명확한 분석, Legacy System 분석에 활용가능
   -> 비기능적 요구사항(신뢰성, 사용성, 유지보수성 등) 중심분석
   -> 아키텍처 스타일, 품질속성은 SAAM 영향을 받음
   
 2. CBAM(Cost Benefit Architecture Method)
 - 아키텍처의 경제적 측면에 초점을 맞춘 평가기법
 - 특징
   -> ATTAM의 결과물을 기반으로하여 아키텍처의 경제성을 분석
   -> ROI 측면의 의사결정을 위한 기준 제시

 3. SAAM(Software Architecture Analysis Method)
 - 사용자의 요구사항 시나리오와 아키텍처 간의 매핑을 통한 적합성 분석
 - 특징
   -> 아키텍처의 Modifiability와 Functionality 집중분석
   -> 평가 경험이 없는 조직에서도 활용가능
   
 4. ADR
 - 아키텍처의 구성요소 간의 응집도를 평가하는 기법

 5. ARID(Architecture Reviews for Intermediate Design)
 - 전체 아키텍처가 아닌 특정 부분에 대한 품질요소에 집중하여 평가
```

### 객체지향 설계 원칙 SOLID
- S(Single Responsibility)
- O(open close)
- L(리스코프 치환) : 서브타입은 어디서나 자신의 기반타입으로 교채할 수 있어야한다.
- I(interface segregation)
- D(Dependency Inversion)

### 객체지향 방법론
- OOSE(object oriented software engineering) : 야콥슨 / 유스케이스
- OMT(object modeling technology) : 럼바우 / 객체-동적-기능 모델링
- OOD(object oriented design) : 부치 / 설계부분만, 미시적/거시적 모두 사용
- Coad와 Yourdon 방법론 : E-R 다이어그램
- Wirfs-Brock 방법론 : 분석설계 구분 없음 고객명세서 평가로 설계작업까지 연속적으로 수행

### 디자인패턴종류(85p)
GoF(Gang of Four) 가 만든 디자인 패턴
#### 생성 패턴(Creational Pattern)
```
'캡슐화'하여 프로그램의 '구조에 영향을 받지 않도록' 하여 '유연성'을 더해준다.

1. 추상 팩토리(Abstract Factory) - 서로 다른 부품을 조립만 하는 조립공장
서로 연관, 의존하는 객체들의 그룹으로 생성하여 추상적으로 표현.
연관된 서브 클래스를 묶어 한 번에 교체 가능.

2. 빌더(Builder) - 건축가가 블록을 조립하는 모습
분리된 인스턴스(객체)를 건축하듯이 조합하여 객체를 생성.
동일한 객체 생성에서도 다른 결과 나올 수 있음.

3. 팩토리 메소드(Factory Method) - 부품부터 완성품까지 통째로 찍어내는 공장
상위 클래스에서 인터페이스만 정의, 실제 생성은 서브 클래스가 담당.

4. 프로토타입(Prototype) - 원형을 두고 복제품을 만드는 것
원본 객체를 복제하는 방법.
비용이 큰 경우 주로 이용.

5. 싱글톤(Singleton) - 식당에서 누구나 사용하지만 하나뿐인 정수기
객체를 어디서든 참조할 수 있지만, 여러 프로세스가 동시에 참조하는 것은 불가능.
인스턴스가 하나뿐이기 때문에 불필요한 메모리 낭비를 최소화 할 수 있음.
```
#### 구조 패턴(Structural Pattern)
```

구조가 복잡한 시스템을 개발하기 쉽도록 도와준다.

1. 어댑터(Adaptor) - 호환성을 맞춰주는 변압기
클래스들의 호환성이 맞도록 변환해주는 패턴.
기존의 클래스를 이용하고 싶은데 인터페이스가 일치하지 않을 때 사용.

2. 브리지(Bridge) - 두 섬을 연결하는 다리
서로가 독립적으로 확장할 수 있도록 구성한 패턴.
기능과 구현을 별도의 클래스에서 구현.

3. 컴포지트(Composite) - 폴더와 파일을 합성한 것
복합 객체와 단일 객체를 구분 없이 다루고자 할 때 사용.
복합 객체 안에 복합 객체가 포함되는 구조 구현 가능.(폴더 안의 폴더)

4. 데코레이터(Decorator) - 온갖 것으로 장식된 눈사람
객체 간의 결합으로 기능을 확장할 수 있음.
부가적인 기능 추가를 위해 다른 객체들을 덧붙이는 방식.

5. 퍼싸드(Facade) - 리모컨만으로 복잡한 명령을 수행하는 것
상위에 인터페이스를 구성하여 서브 클래스들의 기능을 수행할 수 있음.
서브 클래스들 사이의 통합 인터페이스를 제공하는 Wrapper 객체 필요.

6. 플라이웨이트(Flyweight) - 부담을 가볍게 하기 위해 물품 공유
인스턴스를 가능한 공유해서 사용하여 메모리를 절약.
다수의 유사 객체를 생성하거나 조작할 때 유용함.

7. 프록시(Proxy) - 하기 어려운 업무를 대리로 해주는 사람
접근이 어려운 객체와 여기 접근하려는 객체 사이의 인터페이스 역할.
네트워크 연결, 메모리의 대용량 객체로의 접근에 이용.
```
#### 행위 패턴(Behavioral Pattern)
```

하나의 객체로 수행할 수 없는 작업을 여러 객체로 분배하여 결합도를 최소화 하도록 도와준다.

1. 책임 연쇄(Chain of Responsibility) - 연속해서 나눠받는 물레방아
한 객체가 처리하지 못하면 다음 객체로 넘어가는 패턴.
요청이 해결될 때까지 고리를 따라 책임이 넘어감.

2. 커맨드(Command) - 명령어를 하나로 합쳐둔 것
요청을 캡슐화하여 재이용하거나 취소할 수 있도록 저장하거나 로그로 남김.
추상클래스와 구체클래스로 나뉨.

3. 인터프리터(Interpreter) - 언어 번역가
언어에 문법 표현을 정의함.
SQL이나 통신 프로토콜에 사용.

4. 반복자(Iterator) - 같은 명령의 반복
접근이 잦은 객체에 대해 동일한 인터페이스를 사용하도록 함.
내부 표현 방법의 노출 없이 순차적인 접근 가능.

5. 중재자(Mediator) - 매매를 중개해주는 중개사이트
객체들 간의 복잡한 상호작용을 캡슐화하여 객체로 정의.
객체 사이의 결합도를 감소시킴.

6. 메멘토(Memento) - 기억 속의 그 때로 돌아감.
객체를 특정 시점의 상태로 돌릴 수 있는 기능.
ctrl+z 와 같은 기능 개발시 사용.

7. 옵서버(Observer) - 변화를 지켜보고 알려주는 것
한 객체의 상태 변화시 상속되어 있는 다른 객체들에게 알림.
시스템간에 이벤트를 생성하고 수신할 때 사용.

8. 상태(State) - 상태에 따라 다른 방법을 사용함
객체의 상태에 따라 동일한 동작을 다르게 처리해야 할 때 사용.
객체 상태를 캡슐화하고 이를 참조함.

9. 전략(Strategy) - 여러 전략을 정하고 필요할 때 선택하여 씀
동일한 계열의 알고리즘을 캡슐화하여 상호 교환할 수 있게 정의함.
원하는 알고리즘을 선택하여 사용하며 클라이언트에 영향 없이 알고리즘 변경 가능

10. 템플릿 메소드(Template Method) - 방법들을 큰 틀로 묶는 것
상위 클래스에서 골격 정의, 하위 클래스에서 세부 처리를 구체화.
유사한 서브 클래스의 공통된 내용을 상위 클래스에서 정의. (유지보수 용이하게 함)

11. 방문자(Visitor) - 책을 만들기 위해 저자, 편집자를 번갈아가며 방문
각 클래스들의 데이터 구조에서 처리 기능을 별도의 클래스로 구성.
분리된 기능은 각 클래스를 방문하여 수행.
```
# Chapter04
```
1.요구사항 도출단계
- 인터뷰, 브레인스토밍, 롤플레잉, 워크숍, 설문조사
- 델파이기법 : 전문가의 경험적 지식을 통한 문제해결 및 미래예측을 위한 기법

2.요구사항 분석단계 : 요구사항 분류, 개념 모델링 생성 및 분석, 요구사항 할당, 요구사항 협상, 정형 분석
- 자료흐름지향분석, 객체지향 분석 기법이 있다.

3.요구사항 명세단계
- 비정형 명세기법, 정형 명세기법(Z-스키마, Petri Nets, 상태 차트 활용)

4.요구사항 확인 및 검증 단계
- 요구사항검토, 정형 기술 검토 활용(동료검토, 워크스루, 인스펙션), 프로토타이핑 활용, 모델 검증, 테스트, CASE도구 활용, 베이스라인, 요구사항 추적표(RTM)
```

### 미들웨어 솔루션 125p
- 서로 다른 프로토콜이나 시스템 운영체제, 데이터베이스와 애플리케이션 간에 통신을 지원해주는 소프트웨어. 어떤 정보시스템환경에서도 작동할 수 있도록 지원.
  - 유형

```
◎ DB(DataBase) 미들웨어
DB는 데이터베이스 벤더에서 제공하는 클라이언트에서 원격의 데이터베이스와 연결하기 위해 만든 미들웨어
- DB를 사용하여 시스템을 구축하는 경우 보통 2-Tier 아키텍처라고 함
- 대표적인 DB 종류 : 마이크로소프트의 ODBC, 볼랜의 IDAPI, 오라클의 Glue

◎ RPC(Remote Procedure Call) 원격 프로시저 호출
응용 프로그램의 프로시저를 사용하여 원격 프로시저를 마치 로컬 프로시저처럼 호출하는 방식

◎ MOM(Messgae Oriented Middleware) 메세지 지향 미들웨어
메시지 기반의 비동기형 메시지를 전달하는 방식의 미들웨어
- 온라인 업무보다는 이기종 분산 데이터 시스템의 데이터 동기를 위해 많이 사용

◎ TP-Monitor(Transaction Processing Moniter) 트랜잭션 처리 모니터
항공기나 철도 예약 업무 등과 같은 온라인 트랜잭션 업무에서 트랜잭션을 처리 및 감시하는 미들웨어
- 사용자 수가 증가해도 빠른 응답속도를 유지해야 하는 업무에 주로 사용

◎ 레거시웨어
- 기존의 애플리케이션이나 DB기반에 새로운 업데이트된 기능을 덧붙이고자 할 때 사용되는 미들웨어

◎ ORB 객체기반 미들웨어
코바(CORBA) 표준 스펙을 구현한 미들웨어
- 최근에는 TP-Monitor의 장점인 트랜잭션 처리와 모니터링 등을 추가로 구현 가능

◎ WAS(Web Application Server)
정적인 콘텐츠를 처리하는 웹 서버와 달리 사용자의 요구에 따라 변하는 동적인 콘텐츠를 처리하기 위해 사용되는 미들웨어 
 ```
 
### EAI와 ESB

[참고](https://jsdevlog.tistory.com/entry/%EC%A0%95%EB%B3%B4%EC%B2%98%EB%A6%AC%EA%B8%B0%EC%82%AC-%EC%8B%A4%EA%B8%B0-%ED%86%B5%ED%95%A9-%EA%B5%AC%ED%98%84%EB%82%B4%EC%99%B8%EB%B6%80-%EC%97%B0%EA%B3%84-%EB%AA%A8%EB%93%88-%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0
)

1)EAI/ESB의 개념
- EAI와 ESB는 애플리케이션 통합이라는 측면에서 같은 기능을 수행
- 이기종 간 상호 데이터를 통합함으로써 각 시스템 별로 독자적인 비즈니스 로직을 수행할 수 있을 뿐만 아니라, 필요하다면 타 시스템에서 필요한 정보를 취득하여 다양한 서비스를 사용자에게 제공할 수 있음

|구분 |	EAI(Enterprise Application Integration)|	ESB(Enterprise service bus)|
|----|---|---|
|목적 |	어플리케이션 통합	|어플리케이션 및 프로세스 통합|
|방식 |	Native Adapter	|웹 서비스, JMS, IIOP 등|
|표준 |	대부분 표준(부분적 벤더 종속)|	개발형 표준|
|통합 범위 |	기업 내 이기종 어플리케이션	|기업 내외 어플리케이션|
|유지 비용 |	높음(연계 시 adapter 구매, 개발)|	상대적 낮음(서비스 단위 재사용)|
|확장성|	높음(지원 adapter 내 확장 가능)|	매우 높음(서비스 오케스트레이션|
|활용|	E-Biz 인프라	|SOA 인프라 구현 핵심 플랫폼|

