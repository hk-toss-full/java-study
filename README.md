# java-study

# 특징 
---
1. 멀티 쓰레드
2. jvm
3. oop 객체지향


---


jdk ->  jre -> jvm


# version

17, 11, 8


```
public class Main {
    public static void main(String[] args) {
//        console.log
        System.out.println("hello");
        // 변수 const let
        // 변수 선언
//        타입 변수명  =  값;
//        숫자 타입
//        
    }
}
```
# 기본 자료형 (타입)

## 정수

byte (1 byte)(-2^7 ~ 2^7 -1) -> short  (2 byte)(-2^15 ~ 2^15 -1) -> int (4 byte)(-2^32 ~ 2^31 -1) -> long  (8 byte)(-2^64 ~ 2^63 -1)

## 실수

float(4byte) -> double(8byte)




## 형변환
명시적 형변환
(byte) 1 + 4.5f

암시적 형변환 
낮은 것이 높은 것이 되는 것
byte 2 -> short(2^15) 2

```
byte b = (byte) (f + d); //  (byte) 2 .200000023841858
int i = b;
```

## 문자
char (0 ~ 2^7)

## 논리
boolean (0 ~ 1)

조건 <= (이하) < (미만) > (초과) >=(이상) ==(같다) != (다르다)

# 반복 

## for 
```
선언 조건 증감
for(int i = 0; i < 5; i++){
    System.out.println(i);
}

for(int i = 0; i < 5; i++){
    for (int j = 0; j <= i ;j++){
        System.out.print("*");
    }
    System.out.println();
}
```

## while
```
조건 맞으면 안에 실행
조건만 들어가니 선언 밖에서
증감은 안에서
while(조건){
    
}
```
## do - while
실행하고 조건
```
do {

}while(조건)
```
# 조건

## if 
```
if(조건){
맞으면 실행
}else if(조건){
위 조건 아니고 조건이 맞으면 실행
}else{
위 조건들이 다 아니면 실행
}

```
## switch
```
switch(변수){
    case 값:
        변수가 값이랑 같으면 실행
        return; return 이 없으면 아래도 그냥 실행함
    case 값:
        변수가 값이랑 같으면 실행
        return; return 이 없으면 아래도 그냥 실행함
    default:
        return; 항상 끝 else와 같음
}

자바 17 부턴 -> 화살표로 return 생략
switch(변수){
    case 값->
        변수가 값이랑 같으면 실행
        // return; return 이 없으면 아래도 그냥 실행함
    default ->
        // return; 항상 끝 else와 같음
}
```
# 참조형 
대문자로 시작함
## class 형

## array 형
```
//      array 여러가지 데이터를 넣을 때
//      특징 선언과 동시에 길이가 정해져 있음 (불변)
//       array 선언 방법
//        1. 타입[] 변수명 = {값, 값, 값};
//        2. 타입[] 변수명 = new 타입[길이];
```
## interface 형


# 객체지향 

## 특징
1. 객체(Object): 객체는 속성(데이터)과 메소드(행동)를 갖는 것

2. 클래스(Class): 클래스는 객체를 생성하기 위한 템플릿 

3. 상속(Inheritance): 상속은 한 클래스의 속성과 메소드를 다른 클래스가 받아들이는 것

4. 캡슐화(Encapsulation): 캡슐화는 객체의 속성(data fields)과 메소드를 하나로 묶고, 실제 구현 내용 일부를 외부에 감추어 은닉하는 것

5. 다형성(Polymorphism): 다형성은 하나의 메소드나 클래스가 있으면 그것들을 다양한 방법으로 동작시키는 기능 (Override, Overloading)


## 설계 원칙

S - Single Responsibility Principle (SRP) = 단일 책임 원칙  : 클래스(객체)는 단 하나의 책임만 가져야 한다.

O - Open/Closed Principle (OCP) = 개방-폐쇄 원칙 : 확장에 열려있어야 하며, 수정에는 닫혀있어야 한다.

L - Liskov Substitution Principle (LSP) = 리스코프 치환 원칙 : 서브 타입은 언제나 기반(부모) 타입으로 교체가능 해야 한다.

I - Interface Segregation Principle (ISP) = 인터페이스 분리 원칙 : 인터페이스를 각각 사용에 맞게 끔 잘게 분리

D - Dependency Inversion Principle (DIP) = 의존 역전 원칙 : 대상의 상위 요소(추상 클래스 or 인터페이스)로 참조

# 접근 제어자
1. public: 이 접근 제어자가 붙은 클래스, 메서드, 필드는 어떤 클래스에서도 접근이 가능

2. protected: 이 접근 제어자가 붙은 필드와 메서드는 동일 패키지 내의 클래스 또는 해당 클래스를 상속받은 다른 패키지의 클래스에서 접근이 가능

3. default(선언 없음): 이 접근 제어자가 붙은 클래스, 필드, 메서드는 동일 패키지 내의 클래스에서만 접근이 가능 

4. private: 이 접근 제어자가 붙은 필드와 메서드는 해당 클래스 내에서만 접근이 가능









```
