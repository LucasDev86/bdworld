

## GUI 실습문제
### 1. JLabel 컴포넌트는 Mouse 이벤트를 받을 수 있다. JLabel 컴포넌트에 마우스를 올리면<br> "Love Java"가, 내리면 "사랑해"가 출력되도록 스윙 응용프로그램을 작성하라.
<img src="event/1.png" width="320"/>  
<img src="event/2.png" width="320"/>  
  
### 2. 컨텐트팬의 배경색은 초록색으로 하고 마우스를 드래깅하는<br>동안만 노란색으로 유지하는 스윙 응용프로그램을 작성하라.
<img src="event/3.png" width="320"/>  
<img src="event/4.png" width="320"/>

### 3. JLabel을 활용하여 "Love Java"를 출력하고 왼쪽 화살표 키 <Left> 키를 입력할 때마다 <br>"avaJ evoL"와 "Love Java"를 번갈아 출력하는 스윙 프로그램을 작성하라.<br>StringBuffer 클래스의 reverse() 메소드를 이용하여 구현하는 것과<br>JLabel에 포커스를 설정하는 것을 잊지 말아야 한다.
<img src="event/5.png" width="320"/>  
<img src="event/6.png" width="320"/>  

### 4. JLabel을 활용하여 "Love Java"를 출력하고 왼쪽 화살표 키 <Left> 키를 입력할 때마다 <br>"ove JavaL", "ve JavaLo", "e JavaLov" 등과 같이 계속 한 문자씩 왼쪽으로 이동하는<br>스윙 프로그램을 작성하라. 문자열의 이동은 String 클래스의 substring()메소드를 이용하여 구현하라.<br>String text = "Love Java"인 경우, text.substring(0, 1)은 "L"을 리턴하고,<br> text.substring(1)은 "ove Java"를 리턴한다.<br>JLabel에 포커스 설정하는 것을 잊지 말아야 한다.

<img src="event/7.png" width="320"/>  
<img src="event/8.png" width="320"/>    

### 5. JLbel 컴포넌트는 Key 이벤트를 받을 수 있다. JLabel 컴포넌트를 이용하여 <br>"Love Java"를 출력하고 +키를 치면 폰트 크기를 5픽셀씩 키우고, -키를 치면 폰트 크기를 5픽셀씩 줄이는 스윙 응용프로그램을 작성하라.<br>5픽셀 이하로 작아지지 않도록 하라.

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

### 6. 20개의 10 * 10 크기의 JLabel 컴포넌트가 프레임 내에 (50,50)<br>위치에서 (250,250) 영역에서 랜덤한 위치에 출력되도록 스윙프로그램을 작성하라.<br>프레임의 크기는 300*300으로 하라. 

- 힌트
  - JLabel 컴포넌트의 위치를 랜덤하게 설정하기 위해 (x,y) 좌표는 다음과 같이 구한다.
  


<img src="06.png" width="320"/>    
  

- 힌트
  - 컴포넌트의 배경색을 노란색으로 설정하려면 comp.setBackground(Color.YELLOW);로 하면된다.
