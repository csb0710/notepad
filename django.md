### 가상 환경 생성(venv)

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

### django 초기 설정 (Mac)

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

###django 프로젝트 디렉토리 내 .py 파일

