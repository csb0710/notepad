웹서비스는 클라이언트(크롬)의 요청과 서버(spring boot)의 응답으로 이루어진다  
  
- 웹 주소의 뜻  
Localhost : 주소  
8080 : 포트 번호  
이후 파일명 : resources/static 에서 찾음  
  
  
웹페이지의 변수를 활용하는 view templates  
분야별 담당자를 나누는 mvc 패턴  
Model  : 데이터담당  
View templates : 화면  
Controller : 처리과정 담당  
-> MCV 패턴  
  
  
클라이언트 요청(ex. /hi) -> mapping을 통한 controller 호출 -> controller에서 특정 mustache 호출(변수도 같이 넘김) -> mustache에서 웹 페이지를 클라이언트에 전달  
