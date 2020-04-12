# 웹해킹 3주차 

## 1. 실행방법과 실습환경
- 자바 스크립트는 <script> </script> 사이에 위치  
  => 여기서 alert('Hello world!"); 가 자바스크립트  
  => Ctrl + O 로 파일 열기
- 개발자 도구  
  => 크롬 개발자 도구: Ctrl + Shift + J  
  => 에디터 도구: IDE - 통합 개발자 도구 - sublime text 추천  
  ![image](https://user-images.githubusercontent.com/58950184/79058014-1c07ad00-7ca3-11ea-8bd4-046902ae5b3f.png)  
#
## 2. 숫자와 문자 - 데이터의 종류  
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
## 3. 변수(variable) - 값을 담는 컨테이너  
- 'var' a = 1 -> a라는 변수의 값을 1로 한다. 변수에 문자 들어가도 무관. (cf) 변수 여러개 할당: var a=1, b=2  
- 변수를 통해 코드의 효용성 높일 수 있어. 유지보수가 수월한 코드  
![image](https://user-images.githubusercontent.com/58950184/79057997-cc28e600-7ca2-11ea-9693-c8fb2a102d75.png)  

#
## 4. 주석(comment) - 실행 안되는 레퍼런스 용  
- '//이것은 주석임ㅎ'
- /* 여러줄 (줄바꿈)(줄바꿈) 여러줄 */  
![image](https://user-images.githubusercontent.com/58950184/79057984-9a178400-7ca2-11ea-9f84-642a59a5f097.png)  

#

## 5. 줄바꿈과 여백
- ;(세미클론) : '명령이 끝났습니다~' but, JS는 줄바꿈을 ;로 이해하기도 함. 
- 가독성을 위해 띄어쓰기, 세미클론, 들여쓰기 습관화!  

#

## 6. 연산자 - 컴퓨터에 지시하기 위한 기호
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
## 7. 조건문(Condtional Statement) - 주어진 조건에 따라 애플리케이션이 다르게 동작  
- if 문
![image](https://user-images.githubusercontent.com/58950184/79058395-75260f80-7ca8-11ea-9dcd-e8962ef2201f.png)
  - 'if(Boolean 타입 데이터)' - (ex) if(true) 또는 if(false), if(1=2), if(1=1)
  - true일 경우 순차적으로 1, 2, 3, 4 alert 띄우고, true false 상관 없이 5 alert 띄우기
- else, else if
  - else if는 if나 else와는 달리 여러개 올 수 있다
  - else if의 모든 조건이 false일 경우 else가 실행됨
![image](https://user-images.githubusercontent.com/58950184/79058547-680a2000-7caa-11ea-8f69-dd29205ac7d8.png)
- 조건문 응용
  -if문끼리 중첩이 가능하다는 사실!
![image](https://user-images.githubusercontent.com/58950184/79058702-3db96200-7cac-11ea-9aa4-f3b230d94b7d.png)
- 논리 연산자
  - AND: && - 좌항과 우항 모두 true여야 실행
  - OR: || - 둘 중 적어도 하나만 true면 실행 (키보드 위치: Shift + '\'키)
  - NOT: ! - !false는 true !true는 false
![image](https://user-images.githubusercontent.com/58950184/79058793-56764780-7cad-11ea-9641-8deed8fc15b4.png)
- Boolean의 대체제
  - 1: true, 나머지 숫자: false
  - false로 간주되는 데이터 형: 사진 참고 
  ![image](https://user-images.githubusercontent.com/58950184/79058833-c1c01980-7cad-11ea-8ede-ad5be48c17c9.png)
  
#

## 8. 반복문(loop, iterate)
- 무한루프: 반복문에 반복조건이 없어 끊임없이 반복문을 실행
- while문
- 반복조건
![image](https://user-images.githubusercontent.com/58950184/79060505-b75b4b00-7cc0-11ea-82f1-a82f36d4b48b.png)
  - 컴퓨터는 숫자 셀 때 0부터 세는 것이 관습
- for문
  - for(초기화; 반복조건; 반복이 될 때마다 실행되는 코드)
  - 'i=i+1' = 'i++' / '++I'와 달라
![image](https://user-images.githubusercontent.com/58950184/79060586-e0c8a680-7cc1-11ea-9a9d-4a58ccaf7bdf.png)  
- 반복문 제어
  - break: 반복을 중간에 중단
  - continue: 실행을 중단하되 반복은 지속
![image](https://user-images.githubusercontent.com/58950184/79060667-b0353c80-7cc2-11ea-8539-bff0b438468c.png)  
![image](https://user-images.githubusercontent.com/58950184/79060677-c6db9380-7cc2-11ea-8c09-80eb65ebccf8.png)

- 반복의 중첩
  - 이렇게 개발자 도구를 이용해 체계적으로 코드를 분석해 볼 수 있다
  ![image](https://user-images.githubusercontent.com/58950184/79060735-ac55ea00-7cc3-11ea-90f9-98acf715c324.png)
  - 안쪽 for문에서 순환하며 00에서 09까지 안쪽 for문에서 담당, 안쪽 for문 종료되면서 바깥쪽 for문 시작, 바깥쪽 for문이 다시 안쪽 for문 순환으로 넘기면서 10에서 19까지 출력...
  
#

## 9. 함수(function): 하나의 로직을 재실행 할 수 있도록 하는 것. 코드의 재사용성 증가.
![image](https://user-images.githubusercontent.com/58950184/79060865-ce9c3780-7cc4-11ea-970c-e5a57d7268a1.png)

- 출력: return '무언가' - 함수를 종료하고 '무언가'를 뱉아냄
  ![image](https://user-images.githubusercontent.com/58950184/79060934-a3661800-7cc5-11ea-8161-c7447c9df9cc.png)
- 입력: function(input) - 'input'이 변수가 됨. function을 호출할 때 괄호 안에 입력 넣어 input에 대입
![image](https://user-images.githubusercontent.com/58950184/79061029-bf1dee00-7cc6-11ea-9cd1-35db4607120d.png)
- 함수를 정의하는 다른 방법  
![image](https://user-images.githubusercontent.com/58950184/79061051-ebd20580-7cc6-11ea-9eeb-36ec05421874.png)
## 10. 배열
