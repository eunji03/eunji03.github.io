# 과제1

## p123 연습문제
### Q1.
import java.util.Scanner;

public class Test1 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);

		int num1 = 10;
		int num2 = 2;
		char operator;
		
		System.out.println("사칙연산 기호를 입력하세요.");
		operator = sc.nextLine().charAt(0);
		
		switch(operator) {
		case '+' :
			break;
		case '-' :
			break;
		case '*' :
			break;
		case '/' :
			break;	
		}
    
		if(operator == '+') {
			 System.out.println(num1+num2);
		}
		else if(operator == '-') {
			 System.out.println(num1-num2);
		}	
		else if(operator == '*') {
			 System.out.println(num1*num2);	
		}	
		else if(operator == '/') {
			 System.out.println(num1/num2);
		}
		else {
			System.out.println("다시 입력하세요.");
		}
	}
  
  ### Q2.
	public static void main(String[] args) {
  
		for(int i = 1; i <= 9; i++) {
			if (i%2==1)
				continue;
			System.out.println("구구단"+i+"단");
			
			for(int j = 1; j<=9; j++) {
				System.out.println(i+" * "+j+" = "+ i* j);
			}
		}
	}
  
  ### Q3.
  public static void main(String[] args) {
		
		for(int i = 1; i <= 9; i++) {
			System.out.println("구구단"+i+"단");
			
			for(int j = 1; j<=i; j++) {
				System.out.println(i+" * "+j+" = "+ i* j);
			}
		}
	}
  
  ### Q4.
  public static void main(String[] args) {
		
		for(int i=1; i<=4; i++) {
			for(int j=0;j<4-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i*2-1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
  
  ### Q5.
  public static void main(String[] args) {
		
		for(int i=1; i<=4; i++) {
			for(int j=0;j<4-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i*2-1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
		
		for(int i=3; i>=0; i--) {
			for(int j=0;j<4-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i*2-1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
  
  ## P100 나혼자코딩!
import java.util.Scanner;

public class Test100 {

	public static void main(String[] args) {
		
		int score;
		
		Scanner sc = new Scanner(System.in);

		System.out.println("점수를 입력하세요.");
		score = sc.nextInt();
		
		if(score>=90) {
			char greade = 'A';
			System.out.println(greade);
		}
		else if(score>=80) {
			char greade = 'B';
			System.out.println(greade);
			}
		else if(score>=70) {
			char greade = 'C';
			System.out.println(greade);
			}
		else if(score>=60) {
			char greade = 'D';
			System.out.println(greade);
			}
		else {
			char greade = 'F';
			System.out.println(greade);
			}
	}
}

## P106 나혼자코딩!
import java.util.Scanner;

public class Test106 {

	public static void main(String[] args) {
		
		int floor;

		Scanner sc = new Scanner(System.in);
		System.out.println("몇 층에 가시겠습니까?");
		floor = sc.nextInt();
		
		switch(floor) {
		case 1 :
			System.out.println(floor+"층 약국입니다.");
			break;
		case 2 :
			System.out.println(floor+"층 정형외과입니다.");
			break;
		case 3 :
			System.out.println(floor+"층 피부과입니다.");
			break;
		case 4 :
			System.out.println(floor+"층 치과입니다.");
			break;
		case 5 :
			System.out.println(floor+"층 헬스클럽입니다.");
			break;
		}
    
	}
}

## 과제2 사칙연산 계산기
import java.util.Scanner;

public class Test6 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
	      
		int num1;
		int num2;
		char operator;
		
		System.out.print("피연산자 : ");
		num1 = sc.nextInt();
		
	  System.out.print("연산자 : ");
	  operator = sc.next().charAt(0);
	    
	  System.out.print("피연산자 : ");
	  num2 = sc.nextInt();
	    
		if(operator == '+') {
			System.out.print("결과값 : ");
			 System.out.println(num1+num2);
		}
		else if(operator == '-') {
			System.out.print("결과값 : ");
			 System.out.println(num1-num2);	
		}	
		else if(operator == '*') {
			System.out.print("결과값 : ");
			 System.out.println(num1*num2);
		}	
		else if(operator == '/') {
			System.out.print("결과값 : ");
			 System.out.println(num1/num2);	
		}
		else {
			System.out.println("다시 입력하세요.");
		}
		
	}
}

## 과제3
### if-else
import java.util.Scanner;

public class Test7 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		
		int num1; // 몸무게
		int num2 = 100;
		int num3; //키
		
		while(true) {
			System.out.print("몸무게 : ");
			num1 = sc.nextInt();
			
			System.out.print("키 : ");
			num3 = sc.nextInt();
			
			int total = num1+num2-num3;
			
			if(total>0) {
				System.out.println("비만");
			}
			else
			System.out.println("비만이 아닙니다.");
			System.out.println("종료하시겠습니까?(q)");
			char exit = sc.next().charAt(0);
      
			if(exit == 'q')
			{
				System.out.println("종료되었습니다.");
				break;
			}
		}
	}
}

### 삼항연산자
import java.util.Scanner;

public class Test7 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		
		int num1; // 몸무게
		int num2 = 100;
		int num3; //키
		
		while(true) {
			System.out.print("몸무게 : ");
			num1 = sc.nextInt();
			
			System.out.print("키 : ");
			num3 = sc.nextInt();
			
			int total = num1+num2-num3;
			
			String m = (total > 0)? "비만" : "no비만";
			
			System.out.println(m);
      
			System.out.println("종료하시겠습니까?(q)");
			char exit = sc.next().charAt(0);
			if(exit == 'q')
			{
				System.out.println("종료되었습니다.");
				break;
			}
		}
	}
}
