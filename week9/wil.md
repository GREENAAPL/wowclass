<9주차>
- 브라우저 캐싱

client      server
        -----> index.html 주세요
        <----- <h1> hello world </h1>

재요청시 결과가 동일한 정보를 전달한다

- 캐싱을 하면 안되는 요청
금융 서비스, 인증서, 대학원 모집 등

<요청 분류>

단순 조회 요청
여러번 요청해도 결과 동일
url에 정보를 넣어 전달해도 됨
캐싱 가능
GET METHOD- 웹 브라우저의 기본 http method / 브라우저 캐싱 기능 지원 / 정보 읽기, 검색 요청에 주로 사용함/ url에 정보를 넣어 전달

새로운 리소스 생성 요청
요청마다 결과 변경 가능
민감한 정보를 다룸
캐싱 불가능
POST METHOD- 기본 지원x / 캐싱 기능 지원x / 새로운 요소 생성, 로그인 등에 사용됨/ request body에 정보 들어감

<http request>

start-line
header
empty-line
message-body

프로젝트는 우리가 장고로 만드는 소프트웨어 전체
어플리케이션은 프로젝트 내에서 기능별로 쪼개놓은 단위

하나의 프로젝트는 여러개의 어플리케이션으로 이루어진다

model의 역할
1. models.py에 클래스를 생성하면, 장고가 클래스를 토대로 db 테이블을 생성해준다
2. db 테이블에서 값을 조회할 때 models.py에 만들어놓은 클래스의 객체에 값을 담아 반환해준다

model.objects.create()를 이용해 db에 내용을 저장할 수 있다

장고는 http 요청이 들어오면 해당 요청 정보를 python 객체인 httprequest 객체로 변환해 view함수의 인자로 넘겨준다



