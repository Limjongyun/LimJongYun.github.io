# LimJongYun.github.io
Resume (이력서)
JongYun Lim, Software Engineer 

 
 

Contacts 
vavau1993@naver.com 

지원 직무  

Junior Backend Engineer  

 

보유 역량 요약 

Backend Engineering 

9개의 개인, 협업 프로젝트 개발 경험 

MSA, Agile 프로젝트 경험 

Spring framework, JPA or MyBatis  기반으로  Backend API 서버 자체 개발 가능 

Jquery,JSP,JavaScript,WebSquare 로 화면 개발 가능 

Oracle,Mysql(MariaDB) RDBMS 사용 가능 

소규모 프로젝트 DB설계 경험. 

Junit5, DevOnTester 등을 이용한 테스트 코드 수행 경험 

Linux를 이용한 서버 배포 경험 

Query 복잡도로 인하여 지연시간 발생을 감소시키기 위한 쿼리 튜닝 경험 

서비스 개발 후, 실 사용자에게 배포 및 유지보수 경험 

Jenkins 통한 (CI/CD) 자동화 배포 및 통합 테스트 환경 수행 경험 

수십만건의 데이터로 인하여 자바기능은 그대로 하면서 속도를 빠르게 하는 Refactoring 경험 

Git/SVN 형상관리 툴 환경설정 및 수행 경험 

Swagger Rest Docs를 이용한 REST API 문서화 경험 

JIRA등 업무 툴 사용 가능 

데이터 마이그레이션 경험 
 
 

 

 

 

Careers  

 
 

IEA/ Junior Backend Engineer @ LGCNS_모바일 가입팀 협력사(2021.12~ 현재) 

LG U+ MSA 차세대 프로젝트 

기존의 하나의 프로젝트(Monolithic Architecture)  JAVA와 Oracle JDBC(Ibatis)로 이루어진 Legacy 소스를  마이크로 서비스 아키텍처(MSA)로 바꾸고 도메인주도설계(DDD)로 프로젝트를 구성한 것에 SpringBoot,Spring Data JPA를 이용하였으며, 대규모 데이터 이동을 필요로 할때는 Kafka를 이용하여 구성하였습니다.   

해당 프로그램의 완성도 및 일정 완수를 위해 Agile 방식으로 하며 아침,저녁으로는  Scrum을 진행하였습니다. 또한 해당 프로그램이 끝나면 코드리뷰를 하는 등 업무 품질을 높이는 방식으로 진행하였습니다. 

항상 테스트 코드를 체크하여 코드의 완성도를 높였습니다. 

      

< BackEnd > 

> 공직선거법 제공 요청 및 결과 개발 

4500만건의 공직선거 가상번호 요청, 결과,매핑 테이블을 Spring Data JPA를 이용했을 때, 엄청난 시간 대로 TimeOut 이 발생하였고, 또한 컬럼 값이 커 Integer이 아닌 BigDecimal을 이용하였으며,QueryDSl을 이용해서 집계함수를 이용해도 TimeOut이 발생해서  따로 테이블 모델을 만들어 그룹핑된 것을 따로 만들어 해당 건수 타임아웃 해결했습니다. 

Legacy 소스에서 Ibatis로 이루어져 있는 동적쿼리를   Java Stream 로 처리하기에는 소스가 너무 길어져 QueryDSL을 사용하여 매개 변수를 받을 떄는 작동하고, 안 받을 때는 Null로 처리하는 동적쿼리로 쓸 수 있게끔 개발했습니다. 

해당하는 데이터가 많아서  빠른 데이터 조회를 하기 위해 Cardinality가 높고 조회 활용도가 높고 수정 빈도가 거의 없는 것을  인덱스 설정했습니다. 

> 명의변경 선후불회선수 및 외국인 선호번호 건수 개발 

 타파트의 경우 MSA를 사용하기에 DB가 분리되어 있어, 해당하는 파트의 프로젝트의 API 가 없을 경우, 만들어 달라는 요청을 하였으며,  만들어졌을 경우 해당하는 REST API 를 통해 가져오고 1.8 의 Stream filter 를 이용해서 해당하는 건의 Where 절 조건을 대신하여 개발했습니다. 

또한 처음 forEach문으로 SQL 의 GroupBy기능을 만드려고 했으나, forEach때 마다 Repository를 통한 DB연결이 수없이 반복 되다 보니 TimeOut이 빈번하였으며, 해당 건에서 Repository를 한번에 갖고 와와서 Repository DB연결을 한번만 하니 속도는 빨라졌을지 언정 ForEach 문이 반복적으로 돌기에 Stream으로 속도를 빠르게 하는 Refactoring도 했습니다. 

>  초소형중계기 설치정보 전달 개발 

초소형중계기 설치정보의 경우에는 대외의 타회사 Ntoss에게 정보를 보내줘야 하기에 Kafka Topic 을 신청 양식을 작성한 후 Pub을 보내 해당하는 데이터를 전송하는 건을 개발했습니다. 

< FrontEnd > 

솔루션 PID 로 이루어진 Legacy 화면을 WebSquare로 바꾸는 작업, 위의 백엔드 API를 만들고, 웹스퀘어를 통하여 화면개발했습니다. 

자바스크립트의 경우 비동기식 처리이기에 순서 보장을 위해async,await,promise 등을 이용하여 동기식으로 움직이게 하는 비동기식 처리로 개발했습니다. 

단위테스트 케이스를 따로 만들어 해당하는 기능이 빼먹지 않았는지 하나씩 검토하면서 개발했습니다. 
 

월드소프트 /  선임연구원 @ 개발 1팀 (2020.02 ~ 2021.10) 

< BackEnd & FrontEnd > 

> 근태관리 시스템 

업무협의, 개발, 보고서 작성 전반적인 공공기관 관련 업무 프로세스 경험을 했습니다. 

Spring Frame Work,JSP,Jquery,Oracle,MyBatis, Java1.6 을 사용했습니다. 

세콤의 지문 시스템이 해당 DB에 쏴주어 PL/SQL Trigger (Update or Insert) 해당하는 출 퇴근 시간을 이용하여, 연차 계산 시스템, 초과근무 계산 시스템을 만들었습니다. 

공통적으로 사원별 출퇴근 시간을 지정할 수 있게끔 만들어, 지정한 출퇴근 시간을 기준으로 선택적 출퇴근제를 시스템화 할 수 있게끔 만들었습니다. 

해당하는 근무자가 근무일정을 선택하여, 초과근무 및 연차 계산이 따로 되도록 하는 것을 PL/SQL로 개발했습니다. (하지만 PL/SQL로 개발할 경우 이력관리를 하질 못 해 현재는 안하는 방법) 

근무자가 연차, 초과근무, 출장근무 기안을 상신하면 HandyGroupWare라는 툴과 연동하여 기안에 데이터를 넣고 기안 상신을 하고, 해당하는 그룹웨어에서 결재완료가 되면 데이터를 받아, 근태관리 시스템에도 결재처리를 완료하는 시스템을 만들었습니다. 

해당 제품의 기본 틀을 완성하여, 해당 프로그램을 기본 기준을 잡아 각 공공기관이 원하는 요구사항에 대해 개발가능한지 협의를 통하여 납품하였으며, 해당 시스템을 지속적인 유지보수를 했습니다. 

공공기관 해당 Server 컴퓨터에 Linux를 통해 tomcat폴더를 옮겨 놓은 후에, 해당 프로젝트를 war로 압축한다음 자바를 설치하여 실 사용하게 끔 운영 했습니다. 

 

>차량관리 시스템 

다른 회사 프로그램에서 전직장인 월드소프트 회사 프로그램에 맞춰 DB설계를 진행했습니다. 

데이터 마이그레이션 경험했습니다. 

권한별로 메뉴를 다르게 볼 수 있고, Iframe(크롬에서는 보안이슈로 인해 중단)로 멀티탭으로 설정했습니다. 

>건축도시공간 연구원 

Internet explorer 에서만 작동하던 것을 Chrome에서도  작동하도록 하는 Cross Browsing 작업을 진행했습니다. 
