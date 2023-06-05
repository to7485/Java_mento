# 실습 환경 구축하기

## 내 PC에 실습을 위한 폴더 만들기
내 PC -> D드라이브 진입 -> JAVA1900_이니셜 -> 안에 util,work 폴더만들기

![image](https://user-images.githubusercontent.com/54658614/211975967-b510f6c6-1f98-4372-b52c-65c6ed39bb6e.png)

## 자바의 특징
- 자바는 다음과 같은 특징을 가지고 있습니다.

### 객체 지향 언어
- 객체 지향 언어는 하나의 기능을 객체로 만들고, 이러한 객체들을 결합해서 하나의 프로그램을 완성하는 기법을 말합니다.
- 자바는 대표적인 객체 지향 언어로 상속, 캡슐화, 다형성이 잘 나타납니다.

### 단순성
- C/C++을 기반으로 개발되었지만, C/C++에서 제공하는 문법인 포인터 등 혼란을 일으키는 불필요한 기능들을 제거했습니다.

### 이식성
- 자바는 바이트 코드를 생성하고 가상머신(JVM : Java Virtual Machine)을 이용해 자바 프로그램이 여러 운영체제에서 동일한 실행 결과가 나오도록 설계했습니다. 따라서 운영체제의 종류와 상관없이 어느 환경에서나 실행할 수 있습니다.

※바이트 코드 : 0과1로 이루어진 코드( 사실 자바로 작성해도 컴퓨터가 바로 알아들을수는 없다. 바이트 코드로 변환을 해야한다.)<br>
※운영체제(Operating System) : 사용자가 컴퓨터를 사용하기 위해서 필요한 소프트웨어(윈도우,Mac, Linux등등..)<br>
※자바 가상 머신(JVM, Java Virtual Machine): 자바 바이트 코드를 실행시키기 위한 가상의 기계

### 멀티스레드
- 멀티 스레드는 CPU를 최대한 활용하기 위해 프로그램이 2가지 이상을 동시에 실행할 수 있는 기능을 말합니다.
    - 동시성 : 멀티 작업을 위해 하나의 코어에서 멀티 스레드가 번갈아가며 실행
    - 병렬성 : 멀티 작업을 위해 멀티 코어에서 개별 스레드를 동시에 실행

### 메모리 자동 정리
- 자바는 자동으로 가비지 컬렉터(GC : Garbage Collector)가 사용하지 않는 메모리를 주기적으로 수거하고 관리합니다.

### 풍부한 오픈소스 라이브러리
- 자바는 무료로 제공하는 라이브러리가 이미 많이 개발되어 있어 프로그램 개발 기간을 단축할 수 있으며, 안전성 높은 프로그램을 개발할 수 있다.

## JDK 설치하기
- [JDK다운로드](https://www.oracle.com/java/technologies/downloads)

### 오라클 홈페이지로 접속하여 JDK 파일을 다운받아야 한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/67290536-31a8-49ff-a493-af0c92c8f2cf)

### 오른쪽 위 다운로드 버튼을 누른다.

![image](https://github.com/to7485/Java_mento/assets/54658614/5407af4c-0131-45d8-b8f4-16ebbd3aaa88)

### JAVA 11버전을 다운받을 것이다.
- 스크롤을 내리고 운영체제에 맞는 파일을 다운로드 하자.

![image](https://github.com/to7485/Java_mento/assets/54658614/adccc982-3b75-4bf6-be4c-ab7489d5ef01)

### 파일을 열고 Next를 눌러서 설치를 진행한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/1eb2d008-cd99-42ac-8802-9e56c686e490)

### 설치할 경로를 지정하고 Next를 누른다.
- 나는 웬만하면 기본경로에 설치한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/48f3531f-ff63-4557-b471-d710f8ecb6be)

### 설치가 완료되면 Close버튼을 눌러 종료한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/ba13ec2f-5903-4ffa-97df-6612cf6ab5d1)


## 시스템 환경변수 설정하기
- 경로를 따로 변경하지 않았다면 'C:\Program Files\Java\jdk-11.0.16.1\bin'에 컴파일러인 javac.exe와 자바 프로그램을 실행해주는 java.exe가 있다.
- 이 실행파일들은 자바 프로그램을 개발할때 항상 사용하게 되므로 어느 폴더에서나 실행할 수 있도록 환경 변수를 설정해야 한다.

[내PC] - [속성]을 선택하고 [시스템]-[고급 시스템 설정]을 클릭합니다. 이어서[시스템 속성]창에서 [환경변수]를 클릭합니다.<br>

![image](https://github.com/to7485/Java_mento/assets/54658614/82e4f897-ddae-4860-827a-d9fb1ee46f15)

[시스템 변수]에서 [새로 만들기]를 클릭합니다. 변수 이름에는 'JAVA_HOME' 변수값에는 자바가 설치된 경로(C:\Program Files\Java\jdk-11.0.16.1)를 지정해줍니다.<br>

![image](https://github.com/to7485/Java_mento/assets/54658614/cc7a10b5-7354-4f48-9c22-c2dfa4bd9fd8)

![image](https://github.com/to7485/Java_mento/assets/54658614/3ed520c8-a09d-4ca9-a1c0-a61464942957)

[시스템 변수]에서 [Path]환경 변수를 선택하고 [편집]을 클릭합니다. 이어서 나타나는 대화상자에서 [새로만들기]를 클릭한 후 '%JAVA_HOME%\\bin'을 입력하고 [확인]버튼을 클릭한다.
- JAVA 16버전부터는 이 과정을 진행하지 않아도 자동으로 설정됩니다.

![image](https://github.com/to7485/Java_mento/assets/54658614/15451cfd-898b-449e-82e4-8e7856126c69)

![image](https://github.com/to7485/Java_mento/assets/54658614/0d74a857-0d7a-4db5-b8a3-db4787e1a39f)

환경변수가 올바르게 설정되었는지 확인하기 위해 [검색]창에 'cmd'를 입력하여 명령 프롬포트 화면을 실행한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/653610a9-5893-489c-93d2-e18390638768)

명령 프롬포트에서 'java -version'을 입력하고 엔터를 누른다. 정상적으로 JDK가 설치되었다면 다음과 같이 자바 버전이 출력된다.

![image](https://github.com/to7485/Java_mento/assets/54658614/75f7603f-2dde-41a8-9148-328faabc18bc)

# 이클립스 설치하기

## 통합 개발환경
통합 개발 환경(統合開發環境, Integrated Development Environment, IDE)은 코딩, 디버그, 컴파일, 배포 등 프로그램 개발에 관련된 모든 작업을 하나의 프로그램 안에서 처리하는 환경을 제공하는 소프트웨어이다.

### 대중적인 IDE
- 이클립스(Eclipse) : 웹, Java, C, C++
- Visual Studio : C, C++, C#, Python
- Intellij : Java, C/C++
등등 많은 IDE가 있다.

- [Eclipse다운로드](https://www.eclipse.org/)

이클립스 웹사이트에 접속한 후 오른쪽 상단에 [Download]버튼을 클릭합니다.

![image](https://github.com/to7485/Java_mento/assets/54658614/8c5c7de8-fef8-4fa1-9532-8b60ca36f1ba)

다운로드 버튼 밑에 [Download Packages]를 누릅니다.(설치파일로 다운받지 않을것이다)

![image](https://github.com/to7485/Java_mento/assets/54658614/7b97dabf-f430-4ba0-942b-64b2732ea20b)

Eclipse IDE for Enterprise Java and Web Developers 버전을 운영체제에 맞게 다운로드 한다.

![image](https://github.com/to7485/Java_mento/assets/54658614/ef554a0b-5486-4a44-8b82-ef968a97b2db)

![image](https://github.com/to7485/Java_mento/assets/54658614/ed726382-1455-4a56-b6d6-4c5b3e7265c8)

다운로드 받은 압축파일을 util 폴더로 옯기고 압축을 풀어서 사용하면 된다.
(압축을 해제할때는 반디집이 제일 좋다)

![image](https://github.com/to7485/Java_mento/assets/54658614/18d8b7c9-d4a3-4468-bbbc-842e1bf18b47)
