# Day6 과제
## Q1.
import java.util.Scanner;

public class Test1 {

	public static void main(String[] args) {
		/* 과제1. 자연수 n을 입력받고 1부터 홀수를 차례대로 더하면 합이
		 * n이상이면 그 때 더해진 홀수의 개수와 그 합을 출력하는
		 * 프로그램을 작성하시오.
		 */

		Scanner scanner = new Scanner(System.in);
		System.out.println("자연수를 입력하세요.");
		
		int n = scanner.nextInt();
		int total =0;
		
		for(int i=1; i<=n; i++) {
			if(i%2==0)
				continue;
			total += i;
		}
		System.out.println("1~n의 홀수의 합은 "+total);
	}

}

## Q2.
import java.util.Scanner;

public class Test2 {

	public static void main(String[] args) {
		/* 과제2. 자연수 n을 입력받아 "출력 예"와 같이 출력되는
		 * 프로그램을 작성
		 * !'*'과 '*'사이에 공백이 없고 줄사이에도 빈줄이 없다.!
		 */
		
		Scanner scanner = new Scanner(System.in);

		System.out.println("자연수를 입력하세요.");
		int n = scanner.nextInt();
		
		for(int i=n; i>=1; i--) {
			for(int j=0;j<n-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i*2-1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
		
		for(int i=2; i<=n; i++) {
			for(int j=0;j<n-i;j++) {
				System.out.print(" ");
			}
			for(int j=0; j<i*2-1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}

	}

}

## Q3.
import java.util.Arrays;
import java.util.Scanner;

public class Test3 {

	public static void main(String[] args) {
		/* 자연수 n을 입력받아 "출력 예"와 같이 n*n크기의 공백으로
		 * 구분하여 출력되는 프로그램을 작성하시오.
		 * 10 미만의 홀수만 출력하시오.
		 * !숫자는 공백으로 구분하되 줄사이에 빈줄은 없다.
		 */
		
		Scanner scanner = new Scanner(System.in);
		System.out.println("자연수를 입력하세요.");
		int n = scanner.nextInt();
		int num = 1 ;
		
		int[][] arr = new int[n][n];
		
		for(int i=0; i<arr.length; i++) { //행
			
			for(int j=0; j<arr[0].length; j++) {//열
				
				if(num%2==1) {
					arr[i][j] = num;
				}
				num += 2; 
				if(num >= 10)
					num =1;
				//arr[n][n] = n; //행*열
				System.out.print(arr[i][j]+" ");
			}
			System.out.println();

		} 
		
	}

}
