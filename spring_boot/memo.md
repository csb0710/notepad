웹서비스는 클라이언트(크롬)의 요청과 서버(spring boot)의 응답으로 이루어진다  
  
-웹 주소의 뜻
```
Localhost : 주소  
8080 : 포트 번호  
이후 파일명 : resources/static 에서 찾음  
```

  
웹페이지의 변수를 활용하는 view templates  
분야별 담당자를 나누는 mvc 패턴  
```
Model  : 데이터담당  
View templates : 화면  
Controller : 처리과정 담당  
-> MCV 패턴  
```  
  
클라이언트 요청(ex. /hi) -> mapping을 통한 controller 호출 -> controller에서 특정 mustache 호출(변수도 같이 넘김) -> mustache에서 웹 페이지를 클라이언트에 전달  

템플릿 위치 : templates 폴더 아래에 폴더 하나를 만들고 원하는 템플릿을 mustache 형태로 만듬
템플릿 사용 : 원하는 위치에 원하는 템플릿을 {{>}}을 이용하여 경로 지정 후 사용

form 테그를 이용해서 입력받은 사용자 정보를 controller에서 객체 형태로 받아오는데 이때의 객체를 DTO라고 함
form 테그를 사용하는 mustache파일 또한 templates에 하위 폴더를 생성 후 작성   
위에서 만든 controller와 같은 위치에 controller를 하나 더 만든 후 주소 mapping
form 태그에서 입력받은 정보를 어디로 보낼지(action), 어떻게 보낼지(method)가 중요
method가 post일 경우 GetMapping이 아닌 PostMapping을 이용해서 url을 mapping 해줘야함
form에서 데이터를 입력받는 컨트롤러의 메소드의 경우 DTO를 이용해서 받아와야하기 때문에 매개변수로 따로 만들어논 DTO를 가짐
DTO는 자바 클래스가 위치한 프로젝트 패키지 바로아래에 폴더하나를 생성한 후 만듬
DTO내에 존재하는 클래스 필드와 동일한 이름으로 form 내에서 name을 지정해줘야함 

처음 프로젝트를 만들 때 체크한 JPA의 역할은 자바가 db를 이해할 수 있도록 하는 역할
