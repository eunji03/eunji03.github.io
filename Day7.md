# Day 7 과제 대실패....
## Q1
import java.util.Scanner;

public class Test1 {

	public static void main(String[] args) {
		// 자연수 n(3<=n<=10)을 입력받아 영문자를 출력하는 프로그램을 작성
		
		Scanner scanner = new Scanner(System.in);
		
		System.out.println("자연수를 입력하세요.");
		int n = scanner.nextInt();	//자연수를 입력
		
		//int num = 3<=n && n<=10;
		
		char[] eng = new char[52];	//알파벳 배열-크기52(대문자 26개, 소문자 26개)
	
		
		for(int i=0; i<eng.length; i++) { //알파벳 배열 초기화
			if(i<26) {
				eng[i] = (char)(i+65);	//대문자 저장 - 대문자는 아스키코드 65부터 26개(65)
			}
			else {	
				eng[i] = (char)(i+71);	//소문자는 아스키코드 97부터 26개(71)
			}
		}
		int alphabet = 0;
		
		for(int i=n; i>=0; i--) {
			
			for(int j=0; j<i; j++) {
				
				System.out.print(eng[alphabet]);
				alphabet++;
			}
			System.out.println();
		}
		
	}

}

## Q2.
import java.util.Scanner;

public class Test2 {

	public static void main(String[] args) {
		/* 100개의 정수를 저장할 수 있는 배열을 선언하고 정수를 차례로 입력받다가
		 * 0이 입력되면 0을 제외하고 그 때까지 입력된 정수를 가장 나중에
		 * 입력된 정수부터 차례대로 출력하는 프로그램을 작성하시오.
		 */
		Scanner scanner = new Scanner(System.in);
		
		int[] arr = new int[100];	//정수100개를 저장할 수 있는 배열선언
		
		System.out.print("정수를 입력하세요 : ");
		
		/*for(int i = 0; i < arr.length; i++) {
			arr[i] = scanner.nextInt();
			
			if (arr[i] == 0) {
				System.out.println("0을 제외하고 입력하세요.");
				break;
			}
		}
		for(int j = arr.length-1; j >= 0; j-- ) {
			
			if(arr[j] != 0 ) {
				System.out.print(arr[j]+" ");
			}
			
		}*/
		
		for(int i = 0; i < arr.length; i++) {
			arr[i] = scanner.nextInt();
			
		}
		for(int j = arr.length-1; j >= 0; j-- ) {
			
			if(arr[j] != 0 ) {
				System.out.println(arr[j]+" ");
			}
			
		}
		
	}
}

## Q3.
import java.util.Scanner;

public class Test3 {

	public static void main(String[] args) {
		/* 자연수 n을 입력받아 "출력 예" 와 같이 공백으로 구분하여
		 * 출력하는 프로그램을 작성하시오.
		 * ! 숫자를 공백으로 구분하되 줄사이에 빈줄은 없다.
		 */
		
		Scanner scanner = new Scanner(System.in);
		System.out.println("자연수를 입력하세요.");
		int n = scanner.nextInt();
	
		int num = 1;
		
		for(int i=1; i<=n; i++) {
			for(int j=0;j<3-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i; j++) {
				System.out.print(num++);
				
			}
			System.out.println();
		}
		
	}

}

## Q4.
import java.util.Scanner;

public class Test4 {

	public static void main(String[] args) {
		/* 100미만의 양의 정수들이 주어진다.
		 * 입력받다가 0이 입력되면 마지막에 입력된 0을 제외하고
		 * 그 때까지 입력된 정수의 십의 숫자가 각각 몇 개인지
		 * 작은 수부터 출력하는 프로그램을 작성(0개인 숫자는 출력하지 않는다.)
		 */
		Scanner scanner = new Scanner(System.in);
		
		System.out.print("100미만의 양의 정수를 입력 : ");
		int num = scanner.nextInt();      // 입력
		int[] count = new int[num];  // 양수의 사용 횟수 카운트
		  
		// 카운트 시작
		for (int i = 0 ; i < num; i++)   {
			
		   for (int j = 0 ; j < num; j++)  {
			   if (i%2 == 0)   {
				   count[j]++;       
				   break;
			   }
		   }
		   
		  }
		  
		  // 사용된 횟수 출력
		  System.out.println("100미만의 양의 정수가 사용된 횟수를 출력합니다.");
		  
		  for (int i = 0 ; i < num ; i++)  {
		   System.out.println(num + " : " + count[i]);
		   num++;
		  }
		
	}

}

## Q5.
import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class Test6 {

	public static void main(String[] args) {
		// 10개의 정수를 입력받아 배열에 저장한 후 내림차순으로 정렬하여 출력하시오.
		Scanner scanner = new Scanner(System.in);
		
		int[] arr = new int[10];	//정수100개를 저장할 수 있는 배열선언
		
		System.out.print("정수를 입력하세요 : ");
		
		for(int i = 0; i < arr.length; i++) {	//입력
			arr[i] = scanner.nextInt();
			
		}
		for(int j = arr.length-1; j >= 0; j-- ) {	//출력
			
			if(arr[j] != 0 ) {
				Arrays.sort(arr);	//내림차순
				System.out.print(arr[j]+" ");
			}
			
		}

	}

}
