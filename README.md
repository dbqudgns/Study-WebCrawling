# 웹 크롤링 

- 정적 페이지 크롤링 강의 : YouTube-스타트 코딩
- 학습 기간 : 2025/05/22 ~ 2025/05/24

- 동적 페이지 크롤링 강의 : Youtube-나도 코딩
- 학습 기간 : 2025/06 ~ 
--- 

##  학습 내용 

### 정의
- 웹 사이트에 있는 정보를 자동으로 빠르게 수집하는 것 

### 활용 
- 데이터 분석 과정 중 데이터 수집
- 웹 사이트 자동화
- 인공지능 학습 데이터

### 웹 사이트 개발의 요소

<details> <summary><strong>HTML</strong></summary>
1. HTML : 웹 사이트의 구조를 표시하기 위한 언어 
    
- <태그이름>내용</태그이름>
    - <태그이름> : 시작 태그
    - </태그이름> : 종료 태그
      
- <태그이름 속성=”속성값”>내용</태그이름>
    - 속성 : 태그의 추가적인 정보
    - 속성은 여러 개 부여할 수 있고 없어도 된다.
    - 내용에는 텍스트나 태그가 들어갈 수 있거나 없어도 된다.

</details> <details> <summary><strong>CSS</strong></summary>
    
2. CSS : 디자인
- ex) h1 { color : red; }
    - 페이지안에 있는 모든 h1태그에 대해 글자 색깔을 빨강으로 바꿔라
  
![image](https://github.com/user-attachments/assets/5a7aa55c-4c01-4a9a-82cc-75d32f0d2964)
    
- 선택자 : 웹 페이지에서 원하는 태그를 선택하는 문법
    - 태그 선택자 : 태그 이름으로 선택하는 것
        - 태그 선택자는 다른 선택자와  결합해서 사용한다.
        
    - 클래스 선택자 : 클래스 속성 값으로 선택하는 것
        - 클래스 : 태그에 별명을 주는 것
        
   ![image](https://github.com/user-attachments/assets/50504fcc-49ac-4f8c-8c8d-2632d94c2c29)
        
    - 아이디 선택자 : 아이디 속성 값으로 선택하는 것
      
        - 아이디 : 태그에 별명을 주는 것
        
   ![image](https://github.com/user-attachments/assets/5ca30e3e-f709-4960-b9bb-e54e5b921131)
        
    - 자식 선택자 : 바로 아래 자식 태그를 선택하는 것
      
        - 내가 원하는 태그에 별명이 없을 때 사용
        
  ![image](https://github.com/user-attachments/assets/f6560058-1257-42eb-b023-da476a67a515)
</details>

### 정적 페이지 크롤링 ( Static-Crawling ) 

- 정적 페이지 : 데이터의 추가적인 변경이 일어나지 않는 페이지
    - 응답받은 HTML에 원하는 정보가 들어있음

- 데이터를 받아오는 라이브러리 : requests
- 데이터를 뽑아내는 라이브러리 : BeautifulSoup4

- 페이징 알고리즘
  1. 페이지를 바꾸면서 URL이 변경되는 부분을 찾는다.
     
  2. 페이지를 증가 시키면서 요청을 보낸다.

- 크롤링한 데이터 엑셀로 저장하는 라이브러리
  - pandas : 데이터 분석 라이브러리
    
  - openpyxl : 엑셀 자동화 라이브러리

---

## 환경 설정 
- 언어 : Python 3.13.3
- IDE : Visual Studio Code
- 편집 도구 : Jupter Notebook
