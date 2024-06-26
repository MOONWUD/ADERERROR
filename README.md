# ADERERROR_PROJECT: Javajo

         
## 1. 프로젝트 개요  
### 계획 수립 및 설계 ###    
- 사전 조사 : 다양한 이벤트 적용을 효과적으로 적용할 수 있는브랜드 조사. 브랜드 AderError(아더에러)로 선정    
- 선정 이유 : 과업을 통한 퍼블리싱 실력 향상 및 GSAP등과 같은 플러그인 학습    
- 요구사항 분석 : 이벤트 효과 구현 희망    
- 제약사항 분석 : 사용해보지 않은 SCSS과 GSAP, SVG 활용   


            
### Page ###   
- index(main) : 브랜드의 정체성을 담은 제품, 시그니처 라인, 컨셉 포도 등 전체적으로 소개    
- Brand : 핵심 전달 메세지 및 추구하는 이미지를 보여주는 페이지    
- Product List : 한 눈에 보이는 상품 리스트 페이지    
- Product Page : 상품 사진과 스펙, 가격을 알 수 있는 상세페이지    
- Collabo : 콜라보 프로젝트 소개 및 콜라보 상품을 한 눈에 볼 수 있는 페이지    


           
### 목표 ###    
****팀원들과 자바스크립트 공부를 통한 실력 향상 기대 및 적극 활용****   
****아더에러의 심플한 기존 홈페이지에 다양한 이벤트를 넣어 화려하게 구현****    


           
### 팀 구성 및 역할 분담 ###    
- 문지영 : 팀 리더, 기술리더 1, ProductPage    
- 정진영 : 깃허브 관리자, 기술리더 2, ProductList    
- 하은혜 : 디자이너 1, Brand    
- 김예진 : 디자이너 2, Collabo    


         
## 2. 요구사항 분석 
### 기능적 요구사항 ###   
- gsap SCrollTigger를 활용한 스크롤 애니메이션   
- 다양한 플러그인을 사용해 사이트 구현    
- 스크립트를 활용해 다양한 상품 옵션 제시    
- css 애니메이션을 이용한 제품 이미지 슬라이드    


          
### 디자인 요구사항 ###    
- 깔끔하고 가독성 좋은 디자인으로 쇼핑몰 제품을 한 눈에 들어오게 함    
- 이미지를 적극 활용해 브랜드 컨셉을 보여줌    


             
## 3. 작업 순서   
- ****프로젝트 시작****  역할분담, 브랜드 선정 및 페이지 구성 방향 결정
- ****디자인컨센 회의****  index page 디자인 회의 및 피그마에 각자 Sub page 디자인          
- ****Sub Page 디자인****  ProductPage 및 ProductList 페이지 디자인 완료       
- ****Index Page 디자인**** 진행방향 및 퍼블리싱 가이드라인회의, index페이지 디자인완료, 시멘틱마크업 진행       
- ****Sub Page HTML, CSS 작업**** Header/Footer 퍼블리싱, Sub 페이지 퍼블리싱, Github Organization 개설      
- ****SUb Page JS 작업****  Sub 페이지 퍼블리싱, Mouse Emoji 및 Favicon 구현
- ****Index Page HTML, CSS 작업**** Index page 퍼블리싱 및 Sub, index Page 반응형 구현
- ****Index Page JS 작업**** Index 페이지 GSAP, SVG를 활용한 이벤트 효과 구현
- ****최종 정리 및 완료보고서 작성****


          
## 4. 스타일 가이드 라인    
![styleGuide](https://github.com/MOONWUD/ADERERROR/assets/160007468/aa915a6a-2a1a-4d5e-b999-c4a20ae28438)


       
## 5. 퍼블리싱 가이드 라인    
****[퍼블리싱 가이드라인 보러가기](https://drive.google.com/file/d/12SmzhmHL9iDBwW5Nza0HVd9f5j042hKl/view?usp=sharing)****


             
## 6. 디렉토리 구조    
![DirectoryStructure](https://github.com/MOONWUD/ADERERROR/assets/160007468/77cae505-5bb4-4595-897b-5d4748e50008)


        
## 7. 발생 이슈 및 해결 방법    
            📌 main video 영역에 반응형 구현시 비율로 인한 어려움을 겪음     
               ✔️ youtube 영상 자체에 width 값을 크게 주어 영역을 넘는 부분에 overflow hidden을 사용  
                   
            📌 가로스크롤 영역부분 반응형시 사진이 넘치는 현상이 발생      
               ✔️ 모바일에 경우 가로 스크롤을 보는 경우가 드물어 세로로 된 형태로 사진을 돋보이게 만듦 
                   
            📌 GSAP ScrollTrigger를 이용했을때 속도와 타이밍 문제가 발생      
               ✔️ duration과 scrub 값을 조절하고 start와 end 값을 지정해 해결, pc 버전에서만 gsap를 적용   
                   
            📌 product-slideShow를 setInterval로 구현 시 점점 빨라지는 현상 발생     
               ✔️ css의 animation을 이용하여 transform: translateX() 값 조정을 통해 구현 완료
                   
            📌 색상선택시 사진이 변경되는 JS 구현시 어려움을 겪음   
               ✔️ backgroundimage를 이용해 addClass와 removeClass를 사용하여 구현 완료      
                  
            📌 배경 쉐입 변경 이벤트 구현시, 요소 넘침 + 변경되는 쉐입의 높이 불일치    
               ✔️ 스크롤 이벤트시 height 값의 변동 폭을 최대한으로 줄이고, div를 감싸는 wrapper의 width값을 100%으로 고정    
                           
            📌 중앙정렬 했음에도 센터가 맞지 않아 보이는 png 이미지   
               ✔️ padding-right 값을 %로 지정하고, 다양한 화면 사이즈에서 봤을 때도 중앙에 있어 보이도록 크기 값을 조절
                     


                 
## 8. 프로젝트 완료 리뷰    
    👍 Good ~      
      - 퍼플리싱 가이드라인을 정하고 프로젝트를 진행한 것은 큰 도움이 되었다. 
        혼자 작업할 때도 클래스명이나, 주석 표시를 때에 따라 다르게 적어 여러 문서를 돌아다니며 찾아야 했다. 
        하지만 이번 작업은 미리 정한 규칙으로 빠르고 쉽게 원하는 구간을 찾거나 수정할 수 있었다. 
        그럼에도 불구하고 많이 부족한 점이 있었으나, 시도한 것만으로 멋진 결과물을 얻었다고 생각한다. 
        한 번의 시도로 부족한 부분, 더욱 더 상의해야 할 부분은 파악할 수 있었다. 
        
      - 각자 맡은 부분이 있었으나, 문제가 생기면 본인 파트가 아니더라도 상의하고 해결했다. 
        팀프로젝트지만 각자 맡은 파트만 진행해 합쳐놓고 보면 오합지졸인 경우가 있으나,
        우리팀은 매일 한 두번 이상은 상의를 통해 의견을 나누고 또 합쳤다. 
          
    👎 bad ~
      - 미디어쿼리를 충분히 고려하지 않은 css작업이 문제였다. 
        반응형을 목표로 하였으나, 완벽하지 못한 반쪽짜리 반응형으로 완성시켰다. 
        pc 먼저 작업에 들어가서 모바일로 변환시 구현되지 않는 기능이 많아 전부 뺄 수 밖에 없었다. 
        pc 먼저 작업하더라도 모바일로 변환될 것을 고려하여 작업했다면 좋지 않았을까하는 마음이 
        크게 아쉽게 남는다. 
        
      - css 변수를 미리 작업하지 않고 진행해서 추후에 변수로 대체하려고 했을 때,
        모두 다른 단위 값을 쓰고 있어 합치는 과정이 쉽지 않았다. 
        px부터 rem까지 다양한 단위가 사용되었다. 클래스명이나 주석처리 방식 등
        다양한 퍼플리싱 가이드 라인으로 규격화 했다고 생각했지만 빈틈이 존재했다.  
        애를 먹었지만 뒤늦게라도 다시 상의를 통해 공통된 단위를 정했다. 
           
    👐 Takeaway ~
      -  git organization을 통해서 협업하는 것을 배울 수 있었다. 
         혼자 작업할 때는 충돌업이 순조롭게 작업하다가, 팀원들과 함께 작업하면서 반복되는 충돌 속에서
         무엇을 살리고 무엇을 남겨야하는지 상의하는 것을 배웠다. 
         또한, 서로가 작업한 것이 충돌하지 않기 위해 PUSH와 PULL을 실시간으로 공유하였다. 
         소통의 중요성을 또 한 번 깨닫는 시간이었다. 
         
      - 평소에 관심이 없던 브랜드에 대해서 리브랜딩을 하려고 하니, 
        흥미가 떨어지는 부분이 있었다. 
        하지만 프로젝트를 진행하면서 내가 이런 디자인도 할 수 있다는 것을 배웠다. 
        관심이 없다고해서 시도조차 안하던 과거의 나는 이제 없다. 
        할 수 있다고 믿는다 !


***
            
### 240524_금
**발표 및 보고서 제출**

### 240523_목
**다같이**
- 발표준비~~~! 

**하은혜**
- index 로딩페이지 완성

**문지영**
- productPage2 추가

### 240522_수
**정진영**
- productlist page 여백 수정
- index 매거진 세션 부분 효과 작업
- 피그마 PC 버전 디자인 수정

**하은혜**
- 피그마에 PC/MO 최종 디자인으로 수정 완료
- index 로딩 페이지 추가

**문지영**
- productPage 모바일 슬라이드 이미지 모션 수정 완료
- 코드리뷰 작성
- index 3d viedo section 추가

**김예진**
- 피그마에 pc, 모바일 최종 디자인 수정
- collabo, index 유효성검사 오류 수정
- collabo page 여백 수정
- collabo, index css 변수 적용

### 240521_화
**정진영**
- index page 모바일 버전 작업
- 가로 스크롤 부분 모바일 버전 디자인 수정 및 구현

**하은혜**
- brand 모바일/태블릿 완성
- index page PC.ver 수정 완료

**문지영**
- productPage 모바일 구현
- header + footer 수정

**김예진**
- index zoom-in 스크립트 수정
- index zoom-in, product list 모바일/태블릿 완성
- collabo pc 수정

### 240520_월
**정진영**
- index pc 메인 효과 및 가로 스크롤 사진 크기 등 수정
- index page 상단 모바일 버전 작업 시작

**하은혜**
- index에 배경스크롤 이벤트 추가 후 push
- brand 모바일 완성 + 수정완료

**문지영**
- index-magazine 재구성
- 3D slide로 구성 및 완성
- productPage 수정(전체적인 레이아웃)

**김예진**
- collabo page 모바일, 태블릿 사이즈 수정
- index zoom-in 스크립트 수정
- index product list 모바일 버전 구현

### 240517_금
**정진영**
- productlist page 모바일 버전 완료
- nav 영역 주소 추가

**하은혜**
- brand 페이지 완성 및 업로드
- 배경 곡선 -> 직선 이벤트 구현 완료

**문지영**
- global Js 수정하기(Js가 아니라 css로 구현 완료)
- slide list에 click even 완료
- productPage 모바일 완성

**김예진**
- collabo page 태블릿버전 구현
- collabo page js 구현
- index page js 수정

### 240516_목
**정진영**
- index page 60% 작업 완료 html 및 css js 구현(이벤트 추가)
- productlist page 모바일 버전 수정

**하은혜**
- 메인 이미지 레이아웃 수정 및 교체
- 글자 페이드인 이벤트 구현 완료

**문지영**
- product-slideShow Js 구현(수정 필요)
- haeder, footer mobile 구현 완료
- index page magazine section 구현 완료

**김예진**
- collabo page mobile html, css 구현
- collabo page js 구현
- index page zoom section 구현 1차 완료

### 240515_수
**정진영**
- productlist page js 구현 및 page 완성
- index page 50% html 및 css js 구현
- gsap scrollTrigger 기능 학습 및 활용

**하은혜**
- brand페이지 1차 완성(80%), assets > images > brand 폴더에 이미지 추가 후 업로드   
     
**문지영**
- mouse emoji 구현
- productPage html 완성
- productPage scss 완성

**김예진**
- collabo page pc html, css 1차 완성
- collabo page pc js 구현
- favicon 추가
 
### 240514_화 
퍼블리싱 가이드(section전 주석문 표기 및 표기법)정함, 서브페이지 퍼블리싱, 
Github Organization 개설 ^^    
     
**문지영**       
- slideImg 편집, 수정   
- header, footer scss 구현
- productpage html 설계

**정진영**
- productlist page html 및 css 구현

**김예진**
- collabo page pc htrml 및 css 구현
- collabo page 모바일 디자인 수정

### 240513_월
- 앞으로의 진행방향 회의 및 퍼블리싱 가이드(클래스명 및 파일명)
- 포지션 정함(기술리더 - gsap 및 scss 학습)
- 디자인 완성 및 마크업 작업

### 240510_금
디자인 수정
- 브랜드 페이지, 회사소개 페이지 완료
- 메인 페이지

### 240509_목
디자인 수정
- 상세페이지, 상품 리스트 페이지 완료

### 240508_수
메인 페이지 구성 및 구성 페이지 디자인 시작

### 240507_화
프로젝트 회의
- 팀 리더 및 깃허브 관리자 선정
- 벤치마킹 홈페이지 선정 및 브랜드
- 프로젝트 페이지 구성 결정
