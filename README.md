# django-wordcounter

## 개요 
1. 소개
2. 사진
3. 기능
4. 한계 및 과제
* * *
   
## 소개

멋쟁이사자처럼 django 입문 강의에서 사용된 첫번째 프로젝트이다.   
기초 레벨 수준의 프로젝트로, View에서 파이썬으로 가공한 데이터를 Template으로   
데이터를 옮기는 과정을 연습하기 위해 만든 프로젝트이다.   

긴 본문을 입력하면, 총 단어의 수가 몇 개 있는지,   
그리고 각 단어는 본문 내에서 몇 번 등장하는지를 알려준다

꾸미는 과정은 Bootstrap으로 꾸몄다.


* * *
   
## 사진 
![wordcounter1](/wordcounter/wordcounter1.png "wordcounter1")     
![wordcounter2](/wordcounter/wordcounter2.png "wordcounter2")   
![wordcounter3](/wordcounter/wordcounter3.png "wordcounter3")   
![wordcounter4](/wordcounter/wordcounter4.png "wordcounter4")   
* * *
   
## 기능
1. 총 단어 세기
2. 각 단어 수 세기  
3. fontawsome에서 끌어온 아이콘에 github, sns 저장소 링크 남기기
4. about 페이지
5. 공백 포함, 미포함별 총 단어 수 세기 선택 버튼  (과제)
* * * 
   
## 한계 및 과제
1. 한계 :  본문 입력을 GET방식으로 하는건 사실 옳지 못하다. POST방식으로 보내줘야 하는데, 아직 수업때 다루지 않았으므로 (나중에 다룰 예정이므로) 아직은 GET방식으로 하기로 한다. 
2. 과제 : 공백포함-미포함별 단어 세기를 구현해보기. 우리가 구현한 것은 공백을 포함하지 않은 총 단어 수이다. 공백을 포함한 총 단어수는 간단히 "공백제외 단어 수 + 공백 수"라고 볼 수 있는데,
공백 수는 단순히 "공백제외 단어 수 -1 개"이다. 따라서 공백 포함 총 단어 수는 (공백제외 단어 수 X 2 - 1) 개 이다.
