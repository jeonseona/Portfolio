# **PORTFOLIO**

## **📘 목차**

<b>

- 📑 [개요](#-포트폴리오-개요)
- 🔧 [기술 및 도구](#-기술-및-도구)
- 📀 [링크](#-링크)

 </b>

## **📑 포트폴리오 개요**

<img src="https://drive.google.com/uc?id=1mDZwF6E4fWpRNRf0Y4Q6ogsSVzbhC5IV" alt="마이 페이지">

> **프로젝트:** 캠핑 추천 사이트
>
> **기획 및 제작:** 전선아 배재천 정영훈 오세현 권민채
>
> **분류:** 팀 프로젝트
>
> **제작 기간:** 2024.06.03 ~ 2024.06.28
>
> **주요 기능:** 캠핑장 추천, 마이페이지, 관리자, 로그인, 고객센터, 공지/이벤트, 리뷰, QR, 채팅, 캘린더
>
> **사용 기술:** Spring Tool Suite 4(4.21.1) Spring Boot, HTML&CSS, Javascript, Java, Python, Flask, Oracle XE
>
> **문의:** jeonsa0314@naver.com

<br />

## **🔧 기술 및 도구**

![Spring Tool Suite](https://img.shields.io/badge/Spring%20Tool%20Suite-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white)


<br />

## **📀 링크**

**링크:** https://github.com/KampingMate/KampingMate/tree/main

<br />

## **💁🏻‍♀️ 기능 구현**

### **1. 네이버 뉴스("캠핑")**

<img src="https://drive.google.com/uc?id=1cxqW6tXil33lkJ3Sbwskkp2Zf9g37FY1" alt="뉴스">

- 뉴스 검색 API 기능 구현
- 최신순으로 10개씩만 추출 (이전 & 다음 버튼으로 이동 가능)
- 주어진 검색어 "캠핑" 을 인코딩하여 Naver 뉴스 API에 요청하고 결과를 JSON으로 포맷팅하여 반환.

### **2. Footer(QR)**

<img width="100%" alt="QR" src="https://drive.google.com/uc?id=13hylxCAHj1YPzStj2dqFe_UEd20IJJdj">

- 캠핑 관련 웹사이트의 푸터를 구성 (세계적인 아웃도어는 Outdooractive 플랫폼의 API를 사용)
- 구글 폼을 제작하여 qr로 변환 후 만족도 조사 생성 (제출된 설문지도 구글 폼에 저장)

### **3. 반응형 웹**

![MyPage-main](https://drive.google.com/uc?id=185YhSqkWS97msHf3bOKAmDYzJKwvcBeG)
![MyPage-info](https://drive.google.com/uc?id=1CPDJ6lZzE4r0eBa-Y5c_UCrnW622n3su)
![MyPage-bookMark](https://drive.google.com/uc?id=1Yw_YSdmbPM0Vv9suwGy4JWUymtzWmtI1)
![MyPage-reco](https://drive.google.com/uc?id=1sz_kp3_FdLN552RLJ43vWXwJft6fYa-d)
![MyPage-recoDetail](https://drive.google.com/uc?id=1Y9jg0jnvh10hazE3RuIsnDLp57PptSlW)
![MyPage-review](https://drive.google.com/uc?id=1T4sUzBWk92v6_u9fqo6Ui5HJhf8vRNCp)
![MyPage-reviewDetail](https://drive.google.com/uc?id=1tBB04_csFD2Pf-bdZyR_iqpxCCYeiKKv)

- 5개의 endpoint를 두고 반응형을 구현함

```javascript
// media.js
const deviceSizes = {
  desktop: '1440px',
  laptop: '1280px',
  tablet: '1024px',
  mobile: '768px',
  phone: '480px',
};

const media = {
  desktop: `screen and (max-width: ${deviceSizes.desktop})`,
  laptop: `screen and (max-width: ${deviceSizes.laptop})`,
  tablet: `screen and (max-width: ${deviceSizes.tablet})`,
  mobile: `screen and (max-width: ${deviceSizes.mobile})`,
  phone: `screen and (max-width: ${deviceSizes.phone})`,
};

export { deviceSizes, media };
```

<img width="100%" alt="반응형 네비게이션" src="https://user-images.githubusercontent.com/51189962/136144313-2a67d258-3ec1-4517-80fc-3f67b957dff5.gif" />

- 네비게이션 메뉴의 경우 mobile(768px)을 기준으로 그 이상일 경우 상단바, 이하일 경우 햄버거메뉴로 변경

  

