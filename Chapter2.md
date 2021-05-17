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

 
 
