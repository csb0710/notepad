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

### django 디렉토리 하위 파일
-----------------------------------------------------
-Project 디렉토리 하위
* settings.py : 프로젝트의 환경 및 구성을 저장, 웹사이트 관련 설정을 하는 파일
* urls.py : 사용자가 url 접근을 시도하면 path 형식에 따라 views.py 파일의 해당 메소드에 연결시키는 파일

      path 형식 : path('address', views.py의 메소드 경로, path 이름)

-App 디렉토리 하위
* admin.py : admin page에 대한 설정을 하는 파일
* apps.py : app에 대한 기본 설정을 하는 파일
* models.py : model에 대한 정보를 정의하는 파일 (테이블 필드 생성 및 정의)
* views.py : html 페이지에서 발생하는 정보들의 input, output에 대해 관리하는 파일
