# 웹해킹 3주차 

1. 실행방법과 실습환경
- 자바 스크립트는 <script> </script> 사이에 위치  
  => 여기서 alert('Hello world!"); 가 자바스크립트  
  => Ctrl + O 로 파일 열기
- 개발자 도구  
  => 크롬 개발자 도구: Ctrl + Shift + J  
  => 에디터 도구: IDE - 통합 개발자 도구 - sublime text 추천  
  ![image](https://user-images.githubusercontent.com/58950184/79058014-1c07ad00-7ca3-11ea-8bd4-046902ae5b3f.png)  
#
2. 숫자와 문자 - 데이터의 종류  
- 숫자 = 정수, 실수  
- alert 함수가 경고창 띄우는거 귀찮을 때 -> "console.log()" 이용. 크롬에서는 생략 가능.  
- 계산 기호  
  - Math.pow(3,2); - 3의 2제곱
  - Math.round(10.6); - 10.6을 반올림  
  - Math.ceil(10.2); - 10.2를 올림  
  - Math.floor(10.6); - 10.6을 내림  
  - Math.sqrt(9); - 9의 제곱근  
  - Math.random(); - 0에서 1.0사이 랜덤 숫자 -> (변형) 0에서 100까지 난수?: 100*Math.random()  
- '\' : '역슬래쉬' = escape(역할을 없애줌) - (ex) alert('I\'m fine'): m 앞의 '를 문자 그대로 읽음  
- 'typeof ?' : ?의 데이터 형은? - string: 문자열, 
- '\n' : 줄 바꿈
- 생활코딩 자바스크립트 사전 애용하기!  
#
3. 변수(variable) - 값을 담는 컨테이너  
- 'var' a = 1 -> a라는 변수의 값을 1로 한다. 변수에 문자 들어가도 무관. (cf) 변수 여러개 할당: var a=1, b=2  
- 변수를 통해 코드의 효용성 높일 수 있어. 유지보수가 수월한 코드  
![image](https://user-images.githubusercontent.com/58950184/79057997-cc28e600-7ca2-11ea-9693-c8fb2a102d75.png)  

#
4. 주석(comment) - 실행 안되는 레퍼런스 용  
- '//이것은 주석임ㅎ'
- /* 여러줄 (줄바꿈)(줄바꿈) 여러줄 */  
![image](https://user-images.githubusercontent.com/58950184/79057984-9a178400-7ca2-11ea-9f84-642a59a5f097.png)  
#
5. 
