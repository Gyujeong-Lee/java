# JAVA

> Write once, Run anywhere 
>
> 자바가 깔려 있는 어느 곳에서든 실행 가능하다. - > 플랫폼 독립적이다.

## 목차

- Chapter 1 
- Chapter 2
- Chapter 3
- ...



## 설치

- JDK 12
- Intellij



## Chapter 1

### 자바 프로그램과 실행 원리의 이해

- 구조

![image-20220607165031994](JAVA.assets/image-20220607165031994.png)

- 런처와 가상머신

  - 런처 - Java.exe 

    - OS와 가상머신을 연결시킴
    - 자바 가상머신 실행 

  - 가상머신 - JVM

    - OS에 따라 달라진다. But 코드 자체를 변화시킬 필요는 없다.
    - C의 경우 운영체제에 따라 코드의 수정이 필수적이다.

    

- 자바 컴파일러와 바이트 코드

  - 자바 컴파일러

    ![image-20220607165704530](JAVA.assets/image-20220607165704530.png)

    - 소스파일 -> 클래스파일
    - 소스파일 내용을 가상머신이 이해할 수 있도록 변환

  - 자바 런처

    - 자바 프로그램과 자바 가상머신을 처음 구동하는 소프트웨어
    - 클래스 파일을 대상으로 구동을 시작한다.

  

### 자바 프로그램 입문

- 프로그램의 골격과 구성
  - Class  : *FirstJavaProgram*
    - method : *main*
  - **중괄호**를 이용해 클래스와 메소드의 영역을 구분
  - **세미콜론**을 통해 문장의 끝을 표시
    - 단, 명령적 성격을 가진 코드에만 표시 (class, method 정의는 표시 x)

```java
class FirstJavaProgram {
    public static void main(String[] args) {
        System.out.println("Welcome to Java");
        System.out.println("First Java Program");
    }
}
```

- 프로그램 실행 시 main 메소드 안 문장들을 순차적으로 실행
- **println**의 경우 자동 개행



- 들여쓰기와 주석
  - 블록 단위 주석 : `/**/`
  - 행 단위 주석 : `//`
  - 들여쓰기 : space 4칸



## Chapter 2

### 변수의 이해와 활용

- 변수 
  - 메모리 공간의 활용을 위한 도구
  - 메모리 공간의 할당과 접근을 위해 필요한 도구
  - 변수의 선언 -> 메모리 공간의 할당

- 변수의 선언

  - 메모리 공간의 할당
  - 변수의 용도(type), 변수의 이름

  ```java
  int num1;
  num1 = 10;
  int num2 = 20;
  int num3 = num1 + num2;
  int num4, num5;
  ```

- 자료형의 종류와 구분

  - 기본 자료형

    각 자료형 별 할당 메모리 크기가 다름

  ![image-20220607172412001](JAVA.assets/image-20220607172412001.png) 
  - float, double의 경우 오차가 발생할 수 있음 (실수 표현 과정)

- 변수 선언 시 제약 사항 
  - 자바는 대소문자를 구분한다.
  - 변수의 이름은 숫자로 시작할 수 없다.
  - $와 _를 제외한 특수문자는 사용할 수 없다.
  - 키워드는 변수의 이름으로 사용할 수 없다.





