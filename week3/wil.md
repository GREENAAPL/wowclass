<3주차>

-MVC 패턴

        View(응답 내용 관리)
        |
user->Controller(흐름 제어)<->Model(데이터 저장,검색 관리)

-django 

        templates(응답 내용 관리)
        |
user->urls.py(view 목적지 찾아 전달)->view.py(흐름 제어)<->model.py(데이터 저장,검색 관리)

- 프로젝트 vs 어플리케이션

프로젝트는 우리가 장고로 만드는 소프트웨어 전체

어플리케이션은 프로젝트 내에서 기능별로 쪼개좋은 단위

하나의 프로젝트는 보통 여러개의 어플리케이션으로 이루어져있다

-settings.py 

장고 설정에 관한 내용을 담고 있음
DB setting 언어, 시간 설정

<p> My cat is very grumpy </p>
(opening tag)               (closing tag)

My cat is very grumpy = content
<p> My cat is very grumpy </p> = element

html은 우리가 보는 웹페이지가 어떻게 구조화되어 있는지 브라우저로 하여금 알 수 있도록 하는 마크업 언어

태그를 이용해 내용을 꾸미거나 기능을 추가한다.

-manage.py

터미널을 이용해 미리 작성된 명령을 실행할 수 있게 해준다 + sys.path에 managy.py가 위치한 경로를 추가한다


