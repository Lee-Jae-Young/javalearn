## DAY1 자바

```java
package day1;

public class TimeConversion {

	public static void main(String[] args) {
		int time = 10000; // 초단위시간
		System.out.print(time+ "  초는");
		//  시분초단위 변경 출력
		//  10000 초는 xx 시간 xx 분 xx 초입니다.
		// 10분간 실습
		// 10000초는 3600으로 나누면 약 2시간 하고 2800초 남음
		// 2800초는 60으로 나누면 46분하고 40초남음 
		int hour= time/3600; // 정수
		time = time % 3600;
		int minute = time / 60;
	    int second = time % 60;
	    System.out.println(hour + " 시간 " + minute + " 분 " + second + " 초입니다.");
	    // hour 변수 24시간 초과되면 "만 1일 경과했습니다" 출력
	    // 아니면 "1일 이내입니다" 출력
	    // 3분
	    String day = hour > 24?"만 1일 경과했습니다":"1일 이내입니다";
	    System.out.println(day);
	}

}
```

```java
package day1;

public class VariableTest {

	public static void main(String[] args) {
		// int-4바이트(32비트) 최대값 / 최소값
		// - 2^31 ~ 2^31-1
		/*System.out.println(Integer.MAX_VALUE);//자바라이브러리 제공변수
		System.out.println(Integer.MIN_VALUE);
		System.out.println(Byte.MAX_VALUE);//자바라이브러리 제공변수
		System.out.println(Byte.MIN_VALUE);*/
		
		boolean b1 = true;
		System.out.println("b1의 값은 " + b1);
		boolean b2 = 10 > 5 ;
		System.out.println("b2의 값은 " + b2);
		char c1= 'a';
		System.out.println("'" + c1 + "'");
		char c2 = '9';
		System.out.println(c2);
		boolean b3=true;
		// python b3 = True;
		
	}

}
```

