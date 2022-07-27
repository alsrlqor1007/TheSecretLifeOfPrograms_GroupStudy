# RISC와 CISC 명령어 집합


> ### CISC(Complex Instruction Set Computer)

`Intel`칩으로 대표되는 CISC
1. 복잡한 명령어 집합을 가지고 있다.
2. 명령어의 개수 증가에 따라 프로세서 내부 구조가 매우 복잡해지고, 고속으로 작동되는 프로세서를 만들기 힘듦. (RISC를 탄생시킨 결정적 계기)
3. 주로 메인프레임이나 펜티엄 시리즈와 같은 CISC CPU도 내부적으로 복잡한 명령어들을 단순한 명렁어로 나누어 명령어 파이프라인에서 처리하기 때문에 실제 내부 작동 원리는 RISC와 같음.
   ex) 복잡한 명령어: 메모리 1의 내용 X 메모리 2의 내용 -> 메모리 3에 삽입

<br>

> ### RISC(Reduced Instruction Set Computer)

`ARM` 칩으로 대표되는 RISC
1. CISC에서 실제 쓰이는 명령어가 몇 개 되지 않는다는 사실을 바탕으로, 적은 수의 명령어만으로 명령어 집합을 가지고 있는 CPU 구조.
2. 파이프라이닝 기술을 도입할 수 있어 빠른 동작 속도와 하드웨어 단순화 및 효율화, 가격 경쟁력 우위 등의 장점들을 가짐.
3. RISC는 대부분 현대 프로세서 디자인에 채택되어 있고, 임베디드 프로세서에도 사용됨.

<br>

> ### CISC / RISC 특징
### 1. CISC의 특징
- 명령어의 포맷이나 길이에 관한 규칙이 없음(가변적임)
- Micro-Rom 방식의 명령어 디코딩

   :Micro-Rom(= Microcode-Rom, 기계어를 쉽게 추가할 수 있도록 이용하는 방식)
- 하나 이상의 클럭 주기로 하나의 명령어 실행

### 2. RISC의 특징
- 고정 길이 명령어
- 랜덤 로직 방식의 명령어 디코딩
   
   : 빠른 프로세스 수행은 가능하지만 복잡한 프로세스들에는 비효율적
- 단일 클럭 프로세싱
   : 파이프라인 프로세싱이라고도 하며 클럭 주기당 하나의 명령어 실행

<br>

> ### CISC VS RISC

|  |CISC|RISC|
|:-:|:---:|:-----:|
|구조|복잡|단순|
|구성|복잡, 많은 명령어	|간단, 최소 명령어|
|명령어 길이|	가변적	|고정된 길이|
|레지스터|	적음	|많음|
|처리속도|	느림	|빠름|
|전력소모|	많음	|적음|
|용도	|개인용 컴퓨터 ex) PC 상의 Intel 프로세서	|서버, 워크스테이션|

**※ RISC에서 레지스터가 많은 이유: 많은 수의 Register로 메모리 접근을 줄이는 구조이기 때문에**

<img width="717" alt="image" src="https://user-images.githubusercontent.com/91880235/171986070-333b9f9f-4018-461d-bed5-d3d8c9c28cf3.png">

<br>

> ### ETC

### 1. `아키텍쳐 변천사`

- `x86`(범용 CPU, IA-32, 32비트)
  
- `x64`(범용 CPU, IA-64, 64비트)

- `x86-64`(32비트 호환되는 64비트, AMD64(원조), INTEL64(카피), 현재 대부분의 CPU에 해당)


   -> 기존의 x64(IA-64)는 거의 실패한 구조로, 요즘은 x86-64를 x86라고 통칭하여 부름

- `ARM`(저전력 고효율, 스마트기기와 같은 소형기기에 주로 사용)

- `RISC-V`(차세대 CPU, 개발 중)

<br>

### 2. `RISC-V(RISC Five)`
- 2010년부터 UC버클리에서 개발 중인 RISC 기반 개방형(오픈소스) 명령어 집합(ISA)
- CPU코어를 개발자가 원하는 방향대로 구현할 수 있음.

   다양한 운영체제와 IDE를 지원하고, 임베디드 시스템 설계에 범용으로 사용될 수 있음
- 리눅스 지원(리눅스 5.6 릴리즈 버전에서 RISC V 추가)

<img width="400" alt="image" src="https://user-images.githubusercontent.com/91880235/171985138-1f82aab3-a335-4b03-9d06-3c1871f77e95.png">

<br>

### 3. `EPIC(Explicity Parallel Instruction Computing)`

- 여러 명령어를 병렬로 실행 가능한 CPU 구조.
  
- Intel에 의해 개발되었고 RISC + VLIW 조합으로 구성됨.
  
- 분기 예측이 가능하여 파이프라인 해저드 방지.

- 인텔의 `아이테니엄`이 대표적인 EPIC CPU 구조였으나 2021년 단종. IA64 실패의 결과.

*※ VLIW(Very Long Instruction Word)*

   *: 여러가지 독립적인 연산 여러개가 하나의 명령어에 들어가 있는 구조.*
 
   *※ 파이프라인 해저드*

   *: 분기 명령어와 같은 이벤트들이 필요없는 주기들을 생성하여 파이프라인이 중단되는 상태.*

<br>

### 4. `Windows 비트 확인 법`
- `내 컴퓨터 정보`에서 확인
  
<img width="328" alt="image" src="https://user-images.githubusercontent.com/91880235/171985751-8434a711-abd2-4754-bc8c-9213730fa629.png">

### * Mac OS 비트 확인 법
- 터미널에 `uname-a` 입력
<img width="483" alt="image" src="https://user-images.githubusercontent.com/91880235/171985851-bd22e484-8e2c-4b53-bd09-fab20ac83a62.png">

<br>

> ### 참고
<hr> 

- [RISC 나무위키](https://namu.wiki/w/RISC)
- [CISC 나무위키](https://namu.wiki/w/CISC)  
- [[운영체제] 4. CISC와 RISC](https://cooling.tistory.com/19)
- [RISC-V 나무위키](https://namu.wiki/w/RISC-V)
- [x86과 x64의 뜻과 차이 - CPU, OS, S/W](https://blog.naver.com/mumasa/221049608979)
- [RISC-V에 대한 나만의 생각](https://butter-shower.tistory.com/207)
- [RISC-V 구조가 왜 좋은가?](https://www.kernel.bz/boardPost/118681/4)
