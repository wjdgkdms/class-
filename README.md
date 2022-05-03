# classvariable
package s21319_java02;
//클래스 정의
 class Circle{
	 static int radius =10;	//class 자료형 필드 반지름
     //int radius =5;	//	//	instance 반환형 메소드
	 String color = "Black";	//	instance 자료형 필드 색상
	 double calcArea() {	//반환형 메소드
		 return 3.14 * radius * radius;	//해당 값 리턴
	 }
 }
public class S21319_99_ValueClass {

	public static void main(String[] args) {
		Circle a;	//참조 변수 선언
		a = new Circle();	//객체 생성
		//a.radius = 100;
		//a.radius = "Red";
		double area = a.calcArea();	//객체 메소드 접근
		System.out.println("a필드색상 : "+a.color+" 원의 면적 ="+area+" radius:"+a.radius);
		
		Circle b;	//참조 변수 선언
		b = new Circle();	//객체 생성
		b.radius = 20;	//객체 필드 접근
		b.color = "white";	//객체 필드 접근
		area = b.calcArea();	//객체 메소드 접근
		System.out.println("b필드색상 : "+b.color+" 원의 면적 ="+area+" radius:"+b.radius);
		
		Circle c;	//참조 변수 선언
		c = new Circle();	//객체 생성
		area = c.calcArea();	//객체 메소드 접근
		System.out.println("c필드색상 : "+c.color+" 원의 면적 ="+area+" radius:"+c.radius);
		
		//static 전역, 클래스변수 자바를 기동할때 생김 전체가 사용!
	}

}
![image](https://user-images.githubusercontent.com/102034804/166407940-4bff1a63-520a-4025-b68f-8211e8a77a46.png)

실행화면입니다.
