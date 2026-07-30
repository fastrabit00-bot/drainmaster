# DrainMaster SEO Blueprint v1.0

## 1. 프로젝트 목표

드레인명장 홈페이지는 단순한 업체 소개 페이지가 아니라, 지역 검색과 서비스 검색을 동시에 확보하는 SEO 중심 사이트로 구축합니다.

핵심 목표는 다음과 같습니다.

- 서울, 경기, 인천 지역 검색 노출 확대
- 하수구막힘, 배수구막힘, 고압세척, 배관내시경 등 서비스 검색 노출 확대
- 지역 페이지와 서비스 페이지를 서로 연결하는 Topic Cluster 구축
- 동일한 품질로 지역 페이지를 빠르게 확장할 수 있는 템플릿 체계 구축
- 이미지, 구조화데이터, 내부링크, 메타데이터를 공통 기준으로 관리
- GitHub에서 파일 버전과 배포 상태를 안정적으로 관리

---

## 2. 사이트 구조

```text
drainmaster/
├── index.html
├── robots.txt
├── sitemap.xml
│
├── assets/
│   ├── css/
│   │   ├── common.css
│   │   ├── home.css
│   │   ├── region.css
│   │   └── service.css
│   │
│   ├── js/
│   │   └── common.js
│   │
│   └── images/
│       ├── hero/
│       ├── services/
│       ├── process/
│       ├── cta/
│       ├── icons/
│       └── locations/
│
├── services/
│   ├── index.html
│   ├── high-pressure-cleaning/
│   │   └── index.html
│   ├── drain-camera/
│   │   └── index.html
│   ├── restaurant-drain/
│   │   └── index.html
│   ├── building-pipeline/
│   │   └── index.html
│   ├── rooftop-drain/
│   │   └── index.html
│   └── home-blockage/
│       └── index.html
│
├── seoul/
│   ├── index.html
│   ├── gwanakgu/
│   │   └── index.html
│   ├── gangnamgu/
│   │   └── index.html
│   └── ...
│
├── gyeonggi/
│   ├── index.html
│   ├── suwon/
│   │   └── index.html
│   ├── yongin/
│   │   └── index.html
│   └── ...
│
└── incheon/
    ├── index.html
    ├── bupyeonggu/
    │   └── index.html
    ├── namdonggu/
    │   └── index.html
    └── ...
```

---

## 3. URL 규칙

### 3.1 기본 규칙

- 영문 소문자 사용
- 단어 구분은 하이픈 사용
- 모든 폴더 안에 `index.html` 사용
- URL 끝에 `.html`이 노출되지 않도록 폴더 구조 사용
- 지역명은 로마자 표기를 하나로 통일
- URL을 만든 뒤에는 되도록 변경하지 않음

### 3.2 권장 URL 예시

```text
/
 /services/
 /services/high-pressure-cleaning/
 /services/drain-camera/
 /services/restaurant-drain/

 /seoul/
 /seoul/gwanakgu/
 /seoul/gangnamgu/

 /gyeonggi/
 /gyeonggi/suwon/
 /gyeonggi/yongin/

 /incheon/
 /incheon/bupyeonggu/
```

### 3.3 금지 규칙

```text
/seoul-gwanakgu.html
/page1.html
/service01.html
/서울/관악구/
```

---

## 4. 페이지 유형

### 4.1 메인페이지

목적:
- 브랜드 신뢰 형성
- 핵심 서비스 안내
- 주요 지역 허브 연결
- 전화 또는 문의 전환

필수 섹션:

1. Hero
2. 증상 선택
3. 서비스 카드
4. 드레인명장 특징
5. 작업 과정
6. 서비스 지역
7. FAQ
8. CTA

### 4.2 서비스 허브페이지

목적:
- 전체 서비스 분류
- 서비스별 상세 페이지 연결
- 지역 페이지로 연결

필수 섹션:

1. 서비스 소개
2. 서비스 카드
3. 증상별 선택
4. 작업 방식 안내
5. 주요 지역 링크
6. FAQ
7. CTA

### 4.3 서비스 상세페이지

예시:
- 고압세척
- 배관내시경
- 식당 하수구
- 건물 배관
- 옥상 우수관
- 가정집 막힘

필수 섹션:

1. 서비스 중심 Hero
2. 서비스가 필요한 증상
3. 원인 설명
4. 작업 방법
5. 작업 과정
6. 적용 공간
7. 관련 지역
8. 관련 서비스
9. FAQ
10. CTA

### 4.4 광역 지역 허브페이지

예시:
- 서울
- 경기
- 인천

필수 섹션:

1. 지역 중심 Hero
2. 지역 서비스 소개
3. 하위 지역 목록
4. 주요 서비스
5. 자주 발생하는 증상
6. 작업 과정
7. FAQ
8. CTA

### 4.5 세부 지역페이지

예시:
- 관악구
- 강남구
- 수원
- 용인

필수 섹션:

1. 지역명 포함 Hero
2. 지역에서 자주 발생하는 증상
3. 주요 서비스
4. 주거·상가·건물 유형
5. 작업 과정
6. 인접 지역
7. 관련 서비스
8. FAQ
9. CTA

---

## 5. 메인페이지 V2 구조

```text
HEADER
↓
HERO
↓
증상 선택
↓
주요 서비스
↓
왜 드레인명장인가
↓
작업 과정
↓
서비스 지역
↓
FAQ
↓
CTA
↓
FOOTER
```

### 5.1 Hero

권장 H1:

```text
하수구막힘부터 배관 고압세척까지 드레인명장
```

보조문구 예시:

```text
싱크대, 욕실, 식당, 상가, 건물 배관의 막힘 원인을 점검하고 현장에 맞는 방법으로 작업합니다.
```

필수 버튼:

- 전화 상담
- 증상 선택
- 서비스 지역 보기

### 5.2 증상 선택

권장 카드:

- 싱크대막힘
- 욕실배수구막힘
- 변기막힘
- 세탁실막힘
- 식당하수구막힘
- 건물배관막힘

### 5.3 서비스 카드

현재 공용 이미지와 연결:

| 서비스 | 이미지 |
|---|---|
| 고압세척 | `assets/images/services/high-pressure-cleaning.webp` |
| 배관내시경 | `assets/images/services/drain-camera.webp` |
| 식당 기름 슬러지 | `assets/images/services/restaurant-grease.webp` |
| 건물 배관 | `assets/images/services/building-pipeline.webp` |
| 옥상 우수관 | `assets/images/services/rooftop-drain.webp` |
| 가정집 막힘 | `assets/images/services/home-blockage.webp` |

---

## 6. 제목 태그 규칙

### 6.1 H1

- 페이지당 1개
- 페이지의 가장 중요한 검색어 포함
- 지역페이지는 지역명 포함
- 서비스페이지는 서비스명 포함

예시:

```text
관악구 하수구막힘 배관 청소와 고압세척
```

### 6.2 H2

페이지의 핵심 주제를 구분합니다.

예시:

```text
관악구에서 자주 발생하는 하수구막힘 증상
관악구 하수구 작업 서비스
배관 상태에 따른 작업 과정
인접 지역 출장 안내
자주 묻는 질문
```

### 6.3 H3

H2 아래 세부 항목에 사용합니다.

예시:

```text
싱크대 물빠짐 저하
식당 바닥배수구 역류
건물 메인 배관 막힘
```

### 6.4 금지 사항

- 디자인을 위해 의미 없이 H 태그 사용
- H1 여러 개 사용
- H2 다음에 바로 H4 사용
- 모든 제목에 지역명 반복
- 제목을 키워드 나열식으로 작성

---

## 7. 메타데이터 규칙

### 7.1 Title

권장 길이:
- 약 25~40자 내외

구성:

```text
핵심키워드 + 서비스/증상 + 브랜드명
```

예시:

```text
관악구 하수구막힘 고압세척·배관내시경 | 드레인명장
```

### 7.2 Meta Description

구성:

```text
지역 + 증상 + 서비스 + 작업 방식 + 상담 유도
```

예시:

```text
관악구 싱크대, 욕실, 식당, 상가 하수구막힘을 점검합니다. 배관내시경과 고압세척 등 현장 상태에 맞는 작업 방법을 안내합니다.
```

### 7.3 Canonical

모든 페이지에 자기 자신을 가리키는 canonical을 사용합니다.

```html
<link rel="canonical" href="https://도메인/seoul/gwanakgu/">
```

### 7.4 Open Graph

필수 항목:

```html
<meta property="og:type" content="website">
<meta property="og:title" content="">
<meta property="og:description" content="">
<meta property="og:url" content="">
<meta property="og:image" content="">
<meta property="og:site_name" content="드레인명장">
```

---

## 8. 키워드 구조

### 8.1 핵심 키워드

- 하수구막힘
- 배수구막힘
- 배관막힘
- 하수도막힘
- 배관청소
- 고압세척
- 배관내시경
- 하수구역류

### 8.2 증상 키워드

- 물이 안 내려감
- 물빠짐이 느림
- 악취 발생
- 바닥배수구 역류
- 꿀렁거리는 소리
- 오수 역류
- 반복되는 막힘
- 기름 슬러지

### 8.3 공간 키워드

- 가정집
- 아파트
- 빌라
- 단독주택
- 식당
- 카페
- 고깃집
- 중국집
- 미용실
- 상가
- 사무실
- 공장
- 건물
- 옥상
- 지하주차장

### 8.4 지역 키워드

```text
지역명 + 하수구막힘
지역명 + 배수구막힘
지역명 + 고압세척
지역명 + 배관내시경
지역명 + 하수구역류
```

### 8.5 페이지별 키워드 집중 원칙

한 페이지는 하나의 중심 주제에 집중합니다.

예시:

```text
관악구 페이지:
관악구 하수구막힘 중심

고압세척 페이지:
배관 고압세척 중심
```

한 페이지에 모든 지역과 모든 서비스를 무리하게 넣지 않습니다.

---

## 9. 콘텐츠 작성 규칙

### 9.1 지역페이지 차별화 요소

각 지역페이지에는 다음 요소 중 최소 3개 이상을 다르게 구성합니다.

- 주요 주거 형태
- 상가 밀집 지역
- 식당 및 상업시설 환경
- 오래된 건물 배관 특성
- 공동 배관과 세대 배관 차이
- 옥상 우수관 및 외부 배수 환경
- 인접 지역
- 지역별 FAQ
- 서비스 우선순위
- 도입부 문장

### 9.2 중복 방지

금지:

- 지역명만 바꾼 동일 문장
- FAQ 전체 복사
- 메타 설명 복사
- 같은 내부링크 배열 반복
- 같은 ALT 문구 반복

권장:

- 문단 순서 일부 변경
- 지역별 주요 증상 변경
- 지역별 건물 유형 반영
- 관련 서비스 링크 변경
- 인접 지역 링크 변경

### 9.3 권장 분량

초기 기준:

- 메인페이지: 1,500~2,500자
- 서비스 허브: 1,200~2,000자
- 서비스 상세: 1,800~3,000자
- 광역 지역 허브: 1,500~2,500자
- 세부 지역페이지: 1,800~3,000자

분량보다 검색 의도 충족과 중복 방지가 우선입니다.

---

## 10. 내부링크 규칙

### 10.1 메인페이지 링크

메인페이지는 다음으로 연결합니다.

- 서비스 허브
- 핵심 서비스 상세페이지
- 서울 허브
- 경기 허브
- 인천 허브
- 대표 세부 지역페이지

### 10.2 지역 허브 링크

서울 허브는 다음으로 연결합니다.

- 서울 하위 지역
- 주요 서비스
- 메인페이지
- 경기 및 인천 허브

### 10.3 세부 지역페이지 링크

관악구 페이지 예시:

- 상위: 서울 허브
- 인접 지역: 동작구, 금천구, 구로구
- 관련 서비스: 고압세척, 배관내시경, 식당 하수구
- 메인페이지
- 문의 CTA

### 10.4 서비스페이지 링크

고압세척 페이지 예시:

- 서울
- 경기
- 인천
- 관악구
- 강남구
- 수원
- 용인
- 배관내시경
- 건물 배관
- 식당 하수구

### 10.5 앵커텍스트 규칙

권장:

```text
관악구 하수구막힘 서비스
배관 고압세척 작업 안내
식당 하수구 기름 슬러지 제거
서울 지역 출장 안내
```

금지:

```text
여기 클릭
자세히 보기
바로가기
```

필요할 때만 보조적으로 사용합니다.

---

## 11. Breadcrumb 규칙

예시:

```text
홈 > 서울 > 관악구 하수구막힘
```

HTML 예시:

```html
<nav aria-label="breadcrumb">
  <ol>
    <li><a href="/">홈</a></li>
    <li><a href="/seoul/">서울</a></li>
    <li aria-current="page">관악구 하수구막힘</li>
  </ol>
</nav>
```

BreadcrumbList 구조화데이터도 함께 적용합니다.

---

## 12. 이미지 규칙

### 12.1 공통 규격

- 파일 형식: WebP
- 기본 비율: 16:9
- 텍스트 삽입 금지
- 전화번호 삽입 금지
- 로고 삽입 금지
- 과도한 합성 이미지 금지
- 같은 색감 유지
- 실제 현장 사진처럼 자연스럽게 표현

### 12.2 권장 크기

- Hero: 1600×900 또는 1920×1080
- 서비스 카드: 1200×675
- 섹션 이미지: 1200×675
- 썸네일: 필요 시 800×800 별도 제작

### 12.3 파일명 규칙

권장:

```text
high-pressure-cleaning.webp
drain-camera-inspection.webp
restaurant-drain-grease.webp
building-main-pipeline.webp
rooftop-rainwater-drain.webp
home-kitchen-blockage.webp
```

금지:

```text
image1.webp
photo-final.webp
새폴더이미지.webp
```

### 12.4 ALT 규칙

ALT는 이미지가 무엇인지 설명해야 합니다.

예시:

```html
<img
  src="/assets/images/services/high-pressure-cleaning.webp"
  alt="배관 내부를 세척하는 고압세척 작업"
  width="1200"
  height="675"
  loading="lazy">
```

지역페이지 예시:

```text
관악구 식당 하수구 배관 고압세척 작업
관악구 건물 배관내시경 점검
```

모든 이미지에 지역명을 억지로 넣지는 않습니다.

### 12.5 로딩 규칙

- 첫 화면 Hero 이미지는 lazy loading 사용 금지
- 나머지 이미지는 `loading="lazy"` 사용
- width와 height 명시
- 가능하면 `decoding="async"` 사용
- Hero 이미지는 preload 검토

---

## 13. 구조화데이터 규칙

### 13.1 메인페이지

권장:

- Organization
- WebSite
- WebPage
- FAQPage

### 13.2 지역 허브

권장:

- WebPage
- BreadcrumbList
- ItemList
- FAQPage

### 13.3 세부 지역페이지

권장:

- WebPage
- BreadcrumbList
- Service
- FAQPage

### 13.4 서비스페이지

권장:

- Service
- WebPage
- BreadcrumbList
- FAQPage

### 13.5 주의사항

- 실제 페이지에 표시되는 내용만 구조화데이터에 입력
- 존재하지 않는 후기, 평점, 가격 입력 금지
- 실제 사업장 주소가 없다면 임의 주소 입력 금지
- FAQ 스키마의 질문과 답변은 본문에도 동일하게 표시
- 모든 페이지에 같은 LocalBusiness 정보를 무리하게 반복하지 않음

---

## 14. FAQ 규칙

### 14.1 질문 수

페이지당 권장:

- 3~6개

### 14.2 질문 유형

- 증상 판단
- 작업 방법
- 고압세척 필요 여부
- 배관내시경 필요 여부
- 반복 막힘 원인
- 출장 가능 지역
- 작업 전 준비사항

### 14.3 관악구 FAQ 예시

```text
Q. 관악구 식당 하수구가 반복해서 막히는 이유는 무엇인가요?
A. 주방에서 배출되는 기름과 음식물 찌꺼기가 배관 벽면에 쌓이면 물길만 일시적으로 뚫어도 막힘이 반복될 수 있습니다. 배관 상태를 점검한 뒤 청소 범위를 판단해야 합니다.

Q. 물이 천천히 내려가면 바로 고압세척이 필요한가요?
A. 모든 막힘에 고압세척이 필요한 것은 아닙니다. 막힌 위치, 배관 길이, 오염물의 종류를 확인한 뒤 적절한 작업 방법을 선택합니다.

Q. 배관내시경은 언제 사용하나요?
A. 막힘 위치가 불분명하거나 반복적으로 문제가 생기는 경우, 배관 내부 상태와 이물질 위치를 확인하기 위해 사용할 수 있습니다.
```

### 14.4 중복 방지

지역별 FAQ 질문 또는 답변을 최소 30% 이상 다르게 구성합니다.

---

## 15. CTA 규칙

### 15.1 기본 CTA

- 전화 상담
- 증상 문의
- 출장 지역 확인

### 15.2 문구 예시

```text
배수 속도가 느리거나 역류가 반복된다면 배관 상태를 먼저 확인해 보세요.
```

버튼:

```text
전화로 상담하기
증상 문의하기
서비스 지역 보기
```

### 15.3 모바일 CTA

- 화면 하단 고정 전화 버튼 사용 가능
- 본문을 지나치게 가리지 않도록 높이 제한
- 전화번호는 `tel:` 링크 적용

---

## 16. 기술 SEO 규칙

### 16.1 필수 파일

- `robots.txt`
- `sitemap.xml`
- `favicon`
- `404.html`

### 16.2 robots.txt 기본 예시

```text
User-agent: *
Allow: /

Sitemap: https://도메인/sitemap.xml
```

### 16.3 Sitemap

다음 페이지를 포함합니다.

- 메인
- 서비스 허브
- 서비스 상세
- 광역 지역 허브
- 세부 지역페이지

초안, 백업, 테스트 페이지는 제외합니다.

### 16.4 404 페이지

필수 링크:

- 메인페이지
- 서비스 페이지
- 서울
- 경기
- 인천
- 전화 상담

### 16.5 성능

- 공통 CSS 분리
- 불필요한 외부 라이브러리 최소화
- WebP 이미지 사용
- 사용하지 않는 JavaScript 제거
- 폰트 요청 최소화
- 이미지 width/height 지정
- 렌더링 차단 요소 최소화

---

## 17. 공통 컴포넌트

모든 페이지에서 재사용할 공통 요소:

```text
Header
Mobile Navigation
Breadcrumb
Hero
Symptom Cards
Service Cards
Why Us
Process
Region Links
FAQ
CTA
Footer
Mobile Call Button
```

### 17.1 Header

포함:

- 로고 또는 브랜드명
- 서비스
- 지역
- 작업 과정
- FAQ
- 전화 CTA

### 17.2 Footer

포함:

- 브랜드명
- 대표 서비스
- 주요 지역
- 전화번호
- 이용 관련 기본 정보
- 개인정보처리방침 링크
- 사이트맵 링크

---

## 18. 지역페이지 마스터 템플릿

### 18.1 기본 구조

```text
Breadcrumb

Hero
- H1
- 지역 중심 설명
- 전화 CTA

지역에서 자주 발생하는 증상
- 주거 공간
- 식당·상가
- 건물·공용 배관

주요 서비스
- 고압세척
- 배관내시경
- 식당 하수구
- 건물 배관

작업 과정
- 상담
- 현장 점검
- 작업 방법 선택
- 작업 및 확인

지역 특성 콘텐츠

인접 지역
- 상위 지역
- 인접 3~5개 지역

관련 서비스

FAQ

CTA
```

### 18.2 지역별 변수

템플릿에서 바꿔야 하는 항목:

```text
{{REGION_NAME}}
{{REGION_PARENT}}
{{TITLE}}
{{DESCRIPTION}}
{{H1}}
{{INTRO}}
{{LOCAL_FEATURE_1}}
{{LOCAL_FEATURE_2}}
{{LOCAL_FEATURE_3}}
{{NEARBY_REGION_1}}
{{NEARBY_REGION_2}}
{{NEARBY_REGION_3}}
{{FAQ_1}}
{{FAQ_2}}
{{FAQ_3}}
{{CANONICAL_URL}}
```

---

## 19. 서비스페이지 마스터 템플릿

### 19.1 기본 구조

```text
Breadcrumb

Hero
- 서비스명
- 증상과 필요성
- CTA

서비스가 필요한 증상

주요 원인

작업 방법

적용 공간

작업 과정

관련 서비스

주요 서비스 지역

FAQ

CTA
```

### 19.2 서비스별 변수

```text
{{SERVICE_NAME}}
{{SERVICE_SLUG}}
{{SERVICE_TITLE}}
{{SERVICE_DESCRIPTION}}
{{SERVICE_H1}}
{{SERVICE_IMAGE}}
{{SYMPTOM_1}}
{{SYMPTOM_2}}
{{SYMPTOM_3}}
{{METHOD_1}}
{{METHOD_2}}
{{RELATED_SERVICE_1}}
{{RELATED_SERVICE_2}}
{{FAQ_1}}
{{FAQ_2}}
{{FAQ_3}}
```

---

## 20. 서울 확장 규칙

### 20.1 서울 허브

서울 허브는 서울 전체를 설명하고 25개 구 페이지로 연결합니다.

### 20.2 서울 구 페이지

우선 제작 순서 예시:

1. 관악구
2. 강남구
3. 송파구
4. 강동구
5. 영등포구
6. 구로구
7. 금천구
8. 동작구
9. 성동구
10. 광진구

이후 나머지 지역으로 확장합니다.

### 20.3 인접 지역 연결

예시:

```text
관악구
→ 동작구
→ 금천구
→ 구로구
→ 서초구
```

인접 지역은 실제 지리 관계에 맞춰 연결합니다.

---

## 21. 경기 확장 규칙

경기는 시·군 단위로 운영합니다.

예시:

```text
/gyeonggi/suwon/
/gyeonggi/yongin/
/gyeonggi/seongnam/
/gyeonggi/bucheon/
/gyeonggi/goyang/
```

필요한 경우 구 단위 하위 페이지를 추가합니다.

예시:

```text
/gyeonggi/suwon/paldalgu/
/gyeonggi/suwon/yeongtonggu/
```

초기에는 시 단위 페이지를 먼저 완성한 후 검색 수요와 콘텐츠 확보 상황에 따라 구 단위를 확장합니다.

---

## 22. 인천 확장 규칙

예시:

```text
/incheon/bupyeonggu/
/incheon/namdonggu/
/incheon/gyeyanggu/
/incheon/seogu/
/incheon/yeonsugu/
```

인천 허브에서 전체 구·군으로 연결하고, 각 구 페이지에서는 인접 구와 주요 서비스를 연결합니다.

---

## 23. Git 버전관리 규칙

### 23.1 브랜치

초기에는 복잡한 브랜치 운영보다 GitHub Desktop에서 안정적으로 관리합니다.

권장:

- `main`: 현재 공개 또는 배포 가능한 상태
- 기능 개발이 커질 경우 별도 브랜치 사용

### 23.2 커밋 메시지

예시:

```text
Add homepage V2 structure
Add Seoul hub page
Add Gwanakgu SEO template
Add service image library
Update internal links
Fix mobile CTA layout
```

### 23.3 파일 백업

루트 폴더에 아래와 같은 백업 파일을 계속 쌓지 않습니다.

```text
index-old.html
index-final.html
index-final2.html
index-really-final.html
```

백업은 Git 기록을 사용합니다.

테스트 파일은 별도 폴더에서 관리합니다.

```text
/dev/
/drafts/
```

배포 전에는 sitemap에서 제외합니다.

---

## 24. 제작 순서

### Phase 1. 기반 구축

- [x] 기본 저장소 구조
- [x] 이미지 폴더 구조
- [x] Hero 이미지
- [x] 서비스 이미지 6장
- [x] 메인페이지 V1
- [x] SEO Blueprint v1.0
- [ ] 공통 CSS
- [ ] 공통 Header/Footer
- [ ] 메인페이지 V2

### Phase 2. 서비스축

- [ ] 서비스 허브
- [ ] 고압세척
- [ ] 배관내시경
- [ ] 식당 하수구
- [ ] 건물 배관
- [ ] 옥상 우수관
- [ ] 가정집 막힘

### Phase 3. 지역축

- [ ] 서울 허브
- [ ] 관악구 마스터
- [ ] 서울 주요 구
- [ ] 서울 25개 구

### Phase 4. 수도권 확장

- [ ] 경기 허브
- [ ] 경기 주요 시
- [ ] 인천 허브
- [ ] 인천 구·군

### Phase 5. 최종 SEO 점검

- [ ] Title 중복 확인
- [ ] Description 중복 확인
- [ ] H1 중복 확인
- [ ] Broken Link 확인
- [ ] ALT 확인
- [ ] Canonical 확인
- [ ] Schema 확인
- [ ] Sitemap 확인
- [ ] robots.txt 확인
- [ ] 모바일 화면 확인
- [ ] 페이지 속도 확인

---

## 25. 다음 구현 작업

다음 작업은 아래 순서로 진행합니다.

1. 메인페이지 V2 완성
2. 공통 CSS 정리
3. Header와 Footer 공통 구조 확정
4. 서울 허브 제작
5. 관악구 마스터페이지 제작
6. 서비스 허브 제작
7. 고압세척 서비스 상세페이지 제작
8. 내부링크 연결
9. sitemap.xml 생성
10. 전체 SEO 점검

---

## 26. 프로젝트 기준 문장

> 드레인명장 사이트의 모든 페이지는 하나의 검색 의도에 집중하며, 지역과 서비스를 자연스럽게 연결하고, 실제 사용자에게 도움이 되는 정보를 제공하는 것을 우선으로 합니다.

---

문서 버전: **DrainMaster SEO Blueprint v1.0**  
작성 기준: 메인페이지, 서비스 페이지, 서울·경기·인천 지역 확장
