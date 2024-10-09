
>>> 동적 html 생성 

Ex)

def index(request):
    name='kim'
    context={'name' : name}
    return render(request,'index.html',context)


render 함수 html 파일 경로 뒤에는 html 내에 넣고 싶은 정보를 딕셔너리에 담아 넘겨줄 수 있음

render 함수 앞의 request는 장고에서 만들어서 넣어준 HTTP Request 객체

render 함수 두 번째 인자는 응답할 html파일 이름

render 함수 세 번째 인자는 html 파일에서 사용할 딕셔너리

>>> 간단한 태그 알아보기
h1,h2,h3
p
a
li,ul,ol
div
form,input

>>> 장고 템플릿 

장고는 HTML을 동적으로 생성할 수 있다
태그를 만들 수는 없음, 태그 안의 내용을 동적으로 바꿔주기 가능

render 함수 마지막 인자에 원하는 데이터를 담은 딕셔너리를 넣어준다 

딕셔너리의 key 값은 문자열이어야 함
value에는 문자열, 숫자, 딕셔너리, 객체 등등 가능

탬플릿 안의 html파일에서 key 값을 이용해 꺼내쓸 수 있다

{{key}} 와 같이 중괄호 안에 key 값을 넣어 사용한다

>>>장고 ORM 사용법

클래스이름.object를 이용해 DB에 저장된 값에 접근한다.

클래스이름.object.all()이라는 함수를 사용하면 모든 테이블 정보를 객체로 만들어 리스트에 넣어 반환한다

클래스이름.object.get()이라는 함수를 사용하면 조건에 맞는 데이터를 객체로 만들어 반환한다

클래스이름.object.filter()이라는 함수를 사용하면 조건에 맞는 정보들을 객체로 만들어 리스트에 넣어 반환한다

Template에서 객체 내부 데이터에 접근하려면 'key.객체변수이름'으로 사용한다

그외에도 {% %}안에 if,for 같은 파이썬의 제어문을 넣는 것도 가능하다

다만 자료의 크기를 모르므로 {% endfor%}와 같이 마무리해야한다

