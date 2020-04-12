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

5. 줄바꿈과 여백
- ;(세미클론) : '명령이 끝났습니다~' but, JS는 줄바꿈을 ;로 이해하기도 함. 
- 가독성을 위해 띄어쓰기, 세미클론, 들여쓰기 습관화!  

#

6. 연산자 - 컴퓨터에 지시하기 위한 기호
- 대입연산자
  - 'a = 2' -> 변수 a에 2를 대입하라
- 비교연산자
  - 'alert(1 == 2) //false' - 동등 연산자(equal operator) - 좌항과 우항 비교해서 true 또는 false 출력
  - 'alert(1 === '1') //false' - 일치 연산자(strict equal operator) - 좌항은 숫자고 우항은 문자임 데이터 형식도 일치해야만 true 출력
  - 'null': 값이 없다. 'undefined': 정의되지 않음(변수가 선언만 되고 대입 없음)
  - 5가지 데이터 형식(string, number, boolean, null, undefined)
  - NaN: 계산할 수 없음. 숫자가 아님. (Ex) 0/0
  - 일치 연산자를 이용할 것을 권장함.
- 부정과 부등호
  - 'alert(1 != 2) //true' - '같지 않다'
  - 'alert(1 !== '1') //true' - '정확하게 같지 않다'
  - 그 외 딱봐도 아는거: > , >= , <= , <  
  ![image](https://user-images.githubusercontent.com/58950184/79058358-f16c2300-7ca7-11ea-958e-0d3d0abfd6fb.png)  
  
#
7. 조건문(Condtional Statement)  
- 
7.
