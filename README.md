### **Anaconda와 Python을 이용한 django Rest API를 만들고 Nextjs에서 사용하기**
1. 아나콘다에서 새 가상환경을 만들고 모듈들을 설치
```
pip install Django==3.1
pip install django-cors-headers==3.4.0
pip install djangorestframework==3.11.1
pip install djangorestframework-simplejwt==4.6.0
pip install python-decouple
pip install dj-database-url
pip install dj_static
```
2. 파이챰에서 아나콘다에서 만든 가상환경을 토대로 새 프로젝트를 만듦
```
django-admin startproject rest_api
django-admin startapp api
```
3. 생성한 rest_api 폴더 내 settings에서 설치한 모듈들과 미들웨어, 그 외 설정들을 추가

4. Task, Post 등의 모델을 설정

5. 각 모델의 View와 Serializer를 설정 후 urlpattern으로 등록

6. 만들어진 REST api를 헤로쿠에 deploy ([해당 페이지](https://nextjs-api-harry.herokuapp.com/api))

* 주의: 무료 계정이므로 장시간 미사용 시 sleep 처리되고 이후에 다시 접속하려면 30초 정도의 delay가 필요합니다
