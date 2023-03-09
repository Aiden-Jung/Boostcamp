# [Day 1] Python - 파이썬 AI 개발환경 준비하기

## 1. Basic computer class for newbies

### 1-1. 컴퓨터 OS
  
* #### 운영 체제

  * 우리의 프로그램이 동작할 수 있는 구동 환경

  * 프로그램은 운영 체제에 의존적 → 운영 체제에 맞춰서 개발

![운영 체제](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e1/Operating_system_placement.svg/165px-Operating_system_placement.svg.png)[1]

### 1-2. 파일 시스템
  
  * 파일

    * 컴퓨터 등의 기기에서 의미 있는 정보를 담는 논리적인 단위
    * 모든 프로그램은 파일로 구성되어 있고, 파일을 사용한다.

  * 파일 시스템

    * 운영 체제에서 파일을 저장하는 **트리구조** 저장 체계

  * 파일 vs 디렉토리

    * 파일
      * 컴퓨터에서 정보를 저장하는 논리적인 단위
      * 파일은 파일명과 확장자로 식별됨

    * 디렉토리
      * 폴더 또는 디렉토리로 불림
      * 파일과 다른 디렉토리를 포함할 수 있음

* #### 절대 경로와 상대 경로
  * 절대 경로
    * 루트 디렉토리부터 파일위치까지의 경로

  * 상대 경로
    * 현재 있는 디렉토리부터 타깃 파일까지의 경로

### 1-3. 터미널

* #### GUI vs CLI
  * GUI (Graphic User Interface)
    * 그래픽을 이용하여 컴퓨터에 명령을 입력하는 인터페이스 체계

  * CLI (Command Line Interface)
    * 텍스트를 이용하여 컴퓨터에 명령을 입력하는 인터페이스 체계

## 2. Python Overview

### 2-1. Python의 시작

* Python
  * 1991년 귀도 반 로섬이 발표
  * 1989년 크리스마스에 할 일이 없어 파이썬 개발
  * 처음 C언어로 구현되었음
  * 몬티 파이썬이라는 코메디 그룹의 이름에서 유래
    * Python(피톤)은 그리스 신화속의 괴물 뱀
* 사용 이유
  * 쉽고 간단하며 다양하며 이해하기 쉬운 문법

### 2-2. Python의 특징

* 플랫폼
  * 윈도우,리눅스,안드로이드,맥OS,iOS등 프로그램이 실행되는 운영 체제를 플랫폼이라고 함
* 독립적인
  * OS에 상관없이 한번 프로그램을 작성하면 사용가능
* 인터프리터
  * 소스코드를 바로 실행할 수 있게 지원하는 프로그램 실행 방법
* 객체 지향적 언어
  * 실행 순서가 아닌 단위 모듈(객체)중심으로 프로그램을 작성
  * 하나의 객체는 어떤 목적을 달성하기 위한 행동(method)와 속성(attribute)을 가지고 있음
* 동적 타이핑 언어
  * 프로그램이 실행하는 시점에 프로그램이 사용해야할 데이터에 대한 타입을 결정함

### 2-3. 참고

* 컴파일러 vs 인터프리터
  * 컴파일러
    * 소스코드를 기계어로 먼저 번역하여 해당 플랫폼에 최적화되어 프로그램을 실행
    * 장점: 실행속도가 빠름
    * 단점: 한번의 많은 기억장소 필요
    * 주요 언어: C, 자바, C++, C#
  * 인터프리터
    * 별도의 번역과정 없이 소스코드를 실행시점에 해석하여 컴퓨터가 처리할 수 있도록 함
    * 장점: 간단히 작성,메모리가 적게 필요
    * 단점: 실행속도가 느림
    * 주요 언어: 파이썬, 스칼라

* 프로그램의 동작 과정
  * 사람이 알 수 있는 고급언어를 기계만 알 수 있는 저급언어로 변환
  * Source Code → Compiler → Assembler → CPU
  * Source Code → Interpreter → CPU

## 3. Coding Environment

### 3-1. 개발 환경 설정
* 개발 환경 개요
  * 프로그램을 작성하고,실행 시키는 환경
  * 일반적으로 <코딩 환경>이라고 부름
  * 개발환경을 결정
    1. 운영 체제
       * Windows, Linux, Mac OS
    2. Python Interpreter
       * 기존 라이브러리 사용 여부에 따라 버전을 선택
    3. 코드 편집기
       * 설치된 어플리케이션 (ex. VS code)
       * 웹 기반 인터랙티브 편집기 (ex. Jupyter)

## 4. Jupyter & Colab

### 4-1. Jupyter
* Jupyter 개요
  * Julia+Python+R
  * IPython(http://ipython.org) 커널을 기반으로 한 대화형 파이썬 셸
  * 일반적인 터미널 셸 + 웹 기반 데이터 분석 Notebook제공
  * 미디어, 텍스트, 코드, 수식 등을 하나의 문서로 표현 가능
  * 사실상의 데이터 분석 Interactive Shell의 표준
* Jupyter 설치 및 실행
  * Jupyter 설치
    ```    
    conda install jupyter
    ```
  * Jupyter 실행
    ```
    jupyter notebook
    ```
* Jupyter 주요 단축키
  * cell 안 편집 상태
    * 툴팁 표시하기: Shift + Tab
    * 들여쓰기 사용하기: ctrl + ] or ctrl + [
    * 셀 나누기: ctrl + shift + -
  * cell 밖 상태
    * 아래 셀이랑 합치기 :shift + M
    * 셀 오려두기: x
    * 셀 copy: c
    * 셀 붙여넣기: v or shift + v
    * 셀 지우기: d, d
    * 셀 지우기 취소: z
    * Markdown변환: m, m
    * Code로 변환: y, y

### 4-2. Colab
* Colab 개요
  * 구글이 개발 클라우드 기반의 jupyter notebook
  * 구글 드라이브 + GCP + jupyter 등이 합쳐져서 사용자가 손쉽게 접근
  * 초반 여러가지 모듈 설치의 장점을 가짐
  * 구글 드라이브의 파일을 업로드하여 사용가능한 장점 가짐
  * VS Code 등과 연결해서 사용가능
  * V100이상의 GPU를 무료로 쓸 수 있다는 장점을 가짐
* Colab vs Jupyter 주요 단축키 비교

![주요 단축키 비교](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F5703564%2Fc5ccef67da06b3b2aad5795cd722849a%2F2.png?generation=1602690479582417&alt=media)[2]

<!-- 출처 -->
[1]: https://en.wikipedia.org/wiki/Operating_system

[2]: https://www.kaggle.com/getting-started/191091