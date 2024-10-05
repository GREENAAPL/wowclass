<4주차>

-동적 html 생성

views.py

def index(request):
    name='kim'
    context = {'name': name}
    return render(request, 'index.html', context)

qustions.template

<p>{{name}}씨 반갑습니다</p>

-질문 게시판 만들기

models.py

from django.db import models


class Question(models.Mode):
    subject = models.CharFiels(max_length=200)
    content = models.TextField()
    created_date = models.DateTimeField()

makemigrations
> python manage.py makemigrations
> inside questions folder migrations/0001_initial.py 생성
> python manage.py migrate
> inside project folder db.sqlite3 생성

<cmd입력키>
cd.. 상위집단으로 이동
cd project project 폴더로 이동
cd == change direction

activate-가상환경 ON
deactivate- 가상환경 OFF

DB에 PK(point key)가 만들어지지 않는다면 DB가 임의로 INPUT 순서대로 일련번호를 생성한다


