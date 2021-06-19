## Servlet
- 클라이언트의 요청을 처리하고, 그 결과를 반환하는 
Servlet 클래스의 구현 규칙을 지킨 자바 웹 프로그래밍 기술
# 특징
- 클라이언트의 요청에 대해 동적으로 작동하는 웹 어플리케이션 컴포넌트
- HTML을 사용하여 요청에 응답한다.
- Java Thread를 이용하여 동작한다.
- MVC패턴에서 Controller로 이용된다.

# 동작방식
1. 사용자(클라이언트)가 URL을 입력하면 HTTP Request가 Servlet Container로 전송
2. 요청을 전송받은 Servlet Container는 HttpServletRequest, HttpServletResponse 객체를 생성
3. web.xml을 기반으로 사용자가 요청한 URL이 어느 서블릿에 대한 요청인지 찾음
4. 해당 서블릿에서 service메소드를 호출한 후 클리아언트의 GET, POST여부에 따라 doGet() 또는 doPost()를 호출
5. doGet() or doPost() 메소드는 동적 페이지를 생성한 후 HttpServletResponse객체에 응답을 보냄
6. 응답이 끝나면 HttpServletRequest, HttpServletResponse 두 객체를 소멸

