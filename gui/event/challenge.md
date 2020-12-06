

## GUI 실습문제
### 1. JLabel 컴포넌트는 Mouse 이벤트를 받을 수 있다. JLabel 컴포넌트에 마우스를 올리면<br> "Love Java"가, 내리면 "사랑해"가 출력되도록 스윙 응용프로그램을 작성하라.
<img src="event/1.png" width="320"/>  
<img src="event/2.png" width="320"/>  
  
### 2. 컨텐트팬의 배경색은 초록색으로 하고 마우스를 드래깅하는<br>동안만 노란색으로 유지하는 스윙 응용프로그램을 작성하라.
<img src="event/3.png" width="320"/>  
<img src="event/4.png" width="320"/>

### 3. JLabel을 활용하여 "Love Java"를 출력하고 왼쪽 화살표 키 <Left> 키를 입력할 때마다 "avaJ evoL"와 "Love Java"를 번갈아 출력하는 스윙 프로그램을 작성하라. StringBuffer 클래스의 reverse() 메소드를 이용하여 구현하는 것과 JLabel에 포커스를 설정하는 것을 잊지 말아야 한다.
<img src="event/5.png" width="320"/>  
<img src="event/6.png" width="320"/>  

### 4. JLabel을 활용하여 "Love Java"를 출력하고 왼쪽 화살표 키 <Left> 키를 입력할 때마다 "ove JavaL", "ve JavaLo", "e JavaLov" 등과 같이 계속 한 문자씩 왼쪽으로 이동하는 스윙 프로그램을 작성하라. 문자열의 이동은 String 클래스의 substring()메소드를 이용하여 구현하라. String text = "Love Java"인 경우, text.substring(0, 1)은 "L"을 리턴하고, text.substring(1)은 "ove Java"를 리턴한다. JLabel에 포커스 설정하는 것을 잊지 말아야 한다.

<img src="event/7.png" width="320"/>  
<img src="event/8.png" width="320"/>    

### 5. JLbel 컴포넌트는 Key 이벤트를 받을 수 있다. JLabel 컴포넌트를 이용하여 "Love Java"를 출력하고 +키를 치면 폰트 크기를 5픽셀씩 키우고, -키를 치면 폰트 크기를 5픽셀씩 줄이는 스윙 응용프로그램을 작성하라. 5픽셀 이하로 작아지지 않도록 하라.

- 힌트
  - JLabel 컴포넌트에 폰트를 설정하는 방법은 다음과 같다.
```
JLabel la = new JLabel("Love Java")
la.setFont(new Font("Arial", Font.PLAIN, 10)); Arial 폰트로 10픽셀 크기
Font f = la.getFont();
int size = f.getSize();
la.setFont(new Font("Arial", Font.PLAIN, size+5)); //15픽셀 
```
<img src="event/9.png" width="320"/>  
<img src="event/10.png" width="320"/> 

### 6. 클릭 연습용 스윙 응용프로그램을 작성하라. JLabel을 이용하여 문자열이 "C"인 레이블을 하나 만들고 초기 위치를 (100, 100)으로 하라. 문자열을 클릭할 때마다 레이블은 프레임 내의 랜덤한 위치로 움직인다.
- 힌트
  - 배치관리자를 삭제하면 레이블이 임의의 위치로 움직일 수 있다.
  
<img src="event/11.png" width="320"/>  
<img src="event/12.png" width="320"/> 
  
