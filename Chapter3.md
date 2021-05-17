### 문제1
package ch03;

public class Test1 {

	public static void main(String[] args) {
	
		System.out.println("문제1");
		
		int aa = Integer.parseInt(args[0]);
		int bb = Integer.parseInt(args[1]);
		int cc = Integer.parseInt(args[2]);
		
		int total = aa+bb+cc;
		
		System.out.println("sum : "+total);
		
		int avgg = total / 3;
		
		System.out.println("avg : "+avgg);
		
	}

}
![image](https://user-images.githubusercontent.com/84062291/118463862-3419ed80-b73b-11eb-9e45-e651e7e4eb1e.png)


### 문제2
package ch03;

public class Test2 {

	public static void main(String[] args) {
				
		System.out.println("문제2");
		
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		
		a = 100 + a;
		b = b % 10;
		System.out.println(a);
		System.out.println(b);

	}

}
![image](https://user-images.githubusercontent.com/84062291/118463967-4d229e80-b73b-11eb-9f8d-d6a955239ac3.png)


### 문제3
package ch03;

public class Test3 {

	public static void main(String[] args) {
		
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		
		int ab = a/b;
		int ba = a%b;
		
		System.out.println(a + "/" + b + "=" +ab+"..."+ba);

	}

}
![image](https://user-images.githubusercontent.com/84062291/118464046-63305f00-b73b-11eb-8fd4-3523c568a1a5.png)


## 책 P88
package ch03;

public class OperationEx1 {

	public static void main(String[] args) {
		int myAge = 23;
		int teacherAge = 38;
		
		boolean value = (myAge > 25);
		System.out.println(value);
		
		System.out.println(myAge <= 25);
		System.out.println(myAge == teacherAge);
		
		char ch;
		ch = (myAge > teacherAge)? 'T' : 'F';
		
		System.out.println(ch);

	}

}
![image](https://user-images.githubusercontent.com/84062291/118464164-81965a80-b73b-11eb-88d2-8f8be7181fcc.png)
