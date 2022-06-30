# 🧼 Rush & code

## 🎥 프로젝트 사이트 기능 구현 영상

[Rush & code]()

## 👨‍👨‍👧‍👧 Members

정진우 [기술블로그](https://velog.io/@happyeveryone96), [깃허브](https://github.com/happyeveryone96)  
임상빈 [기술블로그](), [깃허브](https://github.com/wjdghks963)  
서수민 [기술블로그](https://velog.io/@sssm), [깃허브](https://github.com/ssm825)  
손소희 [기술블로그](https://sophie0527.tistory.com/), [깃허브](https://github.com/Sophie0527)

## 📢 Introduction

- 개발 인원 및 기간
  - 개발 기간 | 2022-06-20 ~ 2022-06-31
  - 개발 인원 | 총 4명
- 프로젝트 선정 이유
  - 2주라는 짧은 기간 안에 이루어지는 첫번째 프로젝트에 어울리는 기본에 충실한 웹 사이트인 LUSH를 선택하게 되었습니다. 지금까지 배웠던 기술들을 잘 녹여낼 수 있었던 프로젝트라 생각합니다.

## 📪 레포지토리 주소

- [Front-end-repo](https://github.com/wecode-bootcamp-korea/justcode-5-1st-rushandcode-front)
- [Back-end-repo](https://github.com/wecode-bootcamp-korea/justcode-5-1st-rushandcode-back)

## 🗒 Notion 프로젝트 소개

- [Rush & code 노션 페이지](https://www.notion.so/wecode/5-Rush-Code-e28f874f440d4ee8bad7e6d268b12772)

## ⚙ DB modeling

- [Rush & code db 자료 구조](https://dbdiagram.io/d/6299d08254ce263527530e12)

## 💻 Technlogies

- Front-end
  - HTML | STYLED-COMPONENT | JAVASCRIPT | REACT
- Back-end
  - PRISMA | MYSQL | NODE.JS | POSTMAN | EXPRESS

## 👀 담당자 별 구현 기능

### 🔸 Front-end 🔸

#### 정진우

- **`제품 상세`**
  - 제품 상세 정보 가져오기 기능 구현
  - 리뷰 추가, 수정, 삭제 기능 구현
  - 장바구니 추가 기능 구현
  - 내비게이션 바의 버튼 클릭 시 해당 위치로 스크롤 기능 구현
- **`장바구니`**
  - 장바구니 수정 기능 구현
  - 장바구니 삭제 기능 구현
  - 장바구니 전체 삭제 기능 구현

#### 임상빈

- **`메인 페이지`**
  - 메인페이지 첫번째 배너 무한 자동재생기능 및 인덱스버튼 클릭시 해당 슬라이더로 이동기능 구현
  - 가장 많이 판매된 제품순으로 12개를 백앤드에서 데이터를 받아 배너구현 해당 배너 이미지 클릭시 제품상세페이지로 이동
  - 세번째 캐러셀 배너 prev next 버튼 구현
  - 네번째 배너 이미지 Fixed 로 구현 및 배너 텍스트 스크롤 이벤트 추가하여 특정 구간에서 텍스트 애니메이션 효과 구현
  - 마지막 배너 keyframe 애니메이션으로 구현
- **`Footer`**
  - 푸터에 비디오 태그를 이용하여 비디오 재생

#### 서수민

- **`제품 리스트`**
  - 상품 클릭 시 Top Banner 이미지 / 텍스트 변경
  - 상품 리스트 추천순/인기순/낮은 가격순/높은 가격순 정렬 기능 구현
  - 상품 서브 카테고리 리스트 구현
  - 카테고리 및 제품 상세 페이지와 연동
- **`Navigation bar`**
  - 내비게이션 바에 mouse hover 시, 상품 카테고리 리스트와 my page(로그인, 회원가입) 툴팁 창 기능 구현
  - 상품 리스트와 연동

#### 손소희

- **`회원가입&로그인`**
  - 로그인/회원가입 페이지 레이아웃
  - Input 정보 오류 시 오류 별 메세지 알림 기능<br/>
    ( 최소 글자 입력조건, 영문대/소문자, 숫자, 특수문자 중 2가지 이상 조합 등)
  - 회원가입/로그인 버튼 클릭 시 조건에 맞다면 해당 화면으로 이동
- **`이벤트`**
  - 이벤트 페이지 레이아웃
  - 이벤트 클릭 시 해당 이벤트 페이지로 이동

---

### 🔸 Back-end 🔸

#### 정진우

- 상품리스트 API

#### 임상빈

- **`회원가입&로그인 API 및 에러핸들러 미들웨어`**
  - FE 에서 회원가입에 필요한 User 정보를 req.body 값으로 보내주면 해당 값에 대하여 필수조건을 Validation 한 후 password 정보는 bcrypt를 통하여 암호화 하여 user 정보를데이터 베이스에 저장 한 후 성공 및 실패에 대한 메시지를 전송하는 기능을 구현하였습니다.
  - FE에서 로그인 정보를 전달해주면 BE에서 해당유저 정보를 bcrypt를 사용하여 데이터베이스에 있는 정보와 비교하여 일치하는 경우 JWT Token을 이용하여 토큰 생성 후 Response 해주는 기능을 구현하였습니다.
  - BE 에러 핸들러 미들웨어 기능을 구현하여 어떤 레이어에 있던 에러작업을 미들웨어를 통하여 핸들할 수 있도록 구현하였습니다.

#### 서수민

- **`리뷰 API`**
  - 리뷰 작성/수정/삭제 API 구현

#### 손소희

- 제품 상세 API

## Contact US

- 정진우 [wlsdn0337@gmail.com](wlsdn0337@gmail.com)
- 임상빈 [dlatkdqla@gmail.com](dlatkdqla@gmail.com)
- 서수민 [ssm39825@gmail.com](ssm39825@gmail.com)
- 손소희 [ssh30510044@gmail.com](ssh30510044@gmail.com)
