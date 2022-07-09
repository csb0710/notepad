## Mac os 기반
### 가상 환경 생성 (venv)
-------------------------------------------------------

-가상 환경을 만들 디렉토리 생성후 이동
```
$ cd 디렉토리네임
```

-.venv 디렉토리 생성
```
$ python -m venv .venv
```

-가상 환경 활성화
```
$ . .venv/bin/active        or        $ source .venv/bin/active
```

-가상 환경 비활성화
```
$ deactivate
```



### django 초기 설정
---------------------------------------------------------

-django 설치
```
$ pip3 install django
```

-django 버전 확인
```
$ python -m django --version
```

-project 생성
```
$ django-admin startproject 프로젝트네임
```

-app 생성
```
$ python3 manage.py startapp app네임
```

-migrations 설정
```
$ python3 manage.py makemigration
$ python3 manage.py migrate
```

-server 열기
```
$ python3 manage.py runserver
```

-server 닫기
```
control + c
```

### django 프로젝트 디렉토리 하위 .py 파일
-----------------------------------------------------

-app 디렉토리 하위
* admin.py : 장고 관리자 웹을 구성하기 위해 필요한 파일
* apps.py : 장고 웹앱에 대한 설정을 위한 파일
* models.py : 데이터베이스에 정의하기 위한 모델들을 정의해두는 코드를 위한 파일
* views.py : 웹 페이지나 웹 요청등을 처리하는 코드를 작성하는 파일
