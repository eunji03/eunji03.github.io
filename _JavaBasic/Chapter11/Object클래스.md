# Object 클래스

## java.lang 패키지
- 외부 패키지에 선언한 클래스를 사용할 때는 import문으로 클래스가 어느 패키지에 속해있는지 선언해야한다.
- java.lang패키지는 컴파일할 때 import java.lang.*; 문장이 자동으로 추가된다.

## 모든 클래스의 최상위 클래스 Object
- Object클래스는 모든 자바 클래스의 최상위 클래스이다. 모든 클래스는 Object클래스로부터 상속을 받는다.
- 우리가 Object클래스를 상속받는 코드를 작성하지 않아도 컴파일 과정에서 extend Object가 자동으로 쓰인다.
- 우리가 직접 만드는 클래스뿐 아니라 기존 JDK에서 제공하는 클래스도 모두 Object클래스에서 상속을 받습니다.
- 모든 클래스가 Object클래스를 상속받았으므로 Object의 메서드를 사용할 수 있고, 재정의할 수도있고, Object형으로 변환할 수도 있다.


### Object 메소드 설명
protected Object clone() : 해당 객체의 복제본을 생성하여 반환함.

boolean equals(Object obj) : 해당 객체와 전달받은 객체가 같은지 여부를 반환함.

protected void finalize() : 해당 객체를 더는 아무도 참조하지 않아 가비지 컬렉터가 객체의 리소스를 정리하기 위해 호출함.

Class<T> getClass()	: 해당 객체의 클래스 타입을 반환함.
  
int hashCode() : 해당 객체의 해시 코드값을 반환함.

void notify() : 해당 객체의 대기(wait)하고 있는 하나의 스레드를 다시 실행할 때 호출함.

void notifyAll() : 해당 객체의 대기(wait)하고 있는 모든 스레드를 다시 실행할 때 호출함.

String toString()	: 해당 객체의 정보를 문자열로 반환함.

void wait() : 해당 객체의 다른 스레드가 notify()나 notifyAll() 메소드를 실행할 때까지 현재 스레드를 일시적으로 대기(wait)시킬 때 호출함.

void wait(long timeout) : 해당 객체의 다른 스레드가 notify()나 notifyAll() 메소드를 실행하거나 
  전달받은 시간이 지날 때까지 현재 스레드를 일시적으로 대기(wait)시킬 때 호출함.
  
void wait(long timeout, int nanos) : 해당 객체의 다른 스레드가 notify()나 notifyAll() 메소드를 실행하거나 
  전달받은 시간이 지나거나 다른 스레드가 현재 스레드를 인터럽트(interrupt) 할 때까지 현재 스레드를 일시적으로 대기(wait)시킬 때 호출함.


- Object의 모든 메서드를 재정의할 수 있는 것은 아니다. final예약어로 선언한 메서드는 자바 스레드에서 사용하거나 
클래스를 로딩하는 등 자바 가상 머신과 관련된 메서드이기 때문에 재정의할 수 없다.

## toString() 메서드
- 객체 정보를 문자열(String)로 바꿔준다.
- Object클래스를 상속받는 모든 클래스는 toString()을 재정의할 수 있다.

### 
