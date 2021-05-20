# 수업
## 소수 구하기
import java.util.Scanner;

public class Ex05 {

	public static void main(String[] args) {
		//숫자 n값을 입력받아 1부터 n까지 소수를 구하는 프로그램을 작성
		//1에서 n까지 소수 출력
		Scanner sc = new Scanner(System.in);
		
		System.out.println("숫자를 입력하세요.");
		int num = sc.nextInt();
		
		for(int i = 2; i<=num; i++) {
			if ((i!=2)&&(i%2==0)) {
			}
			else if((i!=3)&&(i%3==0)) {
				
			}
			else if((i!=5)&&(i%5==0)) {
				
			}
			else if((i!=7)&&(i%7==0)) {
				
			}
			else {
				System.out.println(i+"");
			}
		}

	}

}
