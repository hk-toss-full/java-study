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

## class 형

## array 형

## interface 형




;
```






```
