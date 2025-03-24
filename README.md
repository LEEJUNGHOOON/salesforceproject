# 🚀 SalesForce Project(Dream Order)

![imageremovebgpreview_12](https://github.com/user-attachments/assets/bfd5fd03-b644-4e30-b2fa-762c4857d98f)


> **한 줄 소개:** Dream Order의 영업 편리를 위한 세일즈포스를 이용한 솔루션 제공
> 프로젝트에 대한 간단한 설명을 작성하세요.

---

## 📌 **1️⃣ 프로젝트 개요**

### 🎯 **프로젝트 목표**
- ✅ **효율적인 Lead 관리**: 지도 기반 Lead 확보 및 자동화된 데이터 수집 기능 제공  
- ✅ **최적화된 설치 배정 시스템**: FSL를 레퍼런스로한 한국 시장에 적합한 지역 및 기사 근무시간을 고려한 최적 배정 알고리즘 구축  
- ✅ **데이터 기반 의사결정 지원**: Tableau 대시보드를 활용한 영업 전략 수립  

---

## 📌 **2️⃣ 팀원 소개**
### 👨‍💻 **팀원 및 역할**
| **사진** | **이름** | **역할** | **GitHub** |
|---------|--------|---------|------------|
| ![신동원](https://via.placeholder.com/100) | 신동원 | Admin (PM) | [GitHub](https://github.com/) |
| ![이경택](https://via.placeholder.com/100) | 이경택 | Admin | [GitHub](https://github.com/) |
| ![김은진](https://via.placeholder.com/100) | 김은진 | Admin | [GitHub](https://github.com/) |
| ![이정훈](https://via.placeholder.com/100) | 이정훈 | Developer (PL) | [GitHub](https://github.com/) |
| ![김우람](https://via.placeholder.com/100) | 김우람 | Developer | [GitHub](https://github.com/Ramkim1205) |

---

## 3️⃣ 프로젝트 프로세스


🖼 **프로세스 다이어그램:**
<img width="788" alt="프로세스 다이어그램" src="https://github.com/user-attachments/assets/c45e2ab1-f674-4add-ae92-de9802f72dd0" />

---

<img width="788" alt="image" src="https://github.com/user-attachments/assets/026953cd-e93e-408c-a83b-a503ee682630" />


---

## 4️⃣ ERD (Entity-Relationship Diagram)

📌 **ERD 설명:** 데이터베이스 구조 및 관계 설명

🖼 **ERD 이미지:**
<br>
![ERD](https://github.com/user-attachments/assets/fdd8c48f-bde2-4c3c-b859-8cd2c538a41f)


---

## 5️⃣ 요구사항 명세서

📌 **기능별 요구사항 정리**
<br>
![image](https://github.com/user-attachments/assets/2a99ac14-1e43-44bf-ab5b-ab2e9632452a)

---

## 6️⃣ 주요 기능


### 📌 Feature 1 – Outbound Lead Acquisition
- 테이블오더 영업 특성상 outbound영업 및 리드확보가 많은점을 고려하여,또 일일이 내가 확보한 리드의 정확한 위치를 입력하는데 불편하고 정확도가 떨어진다는 pain point가 존재.
- 컴포넌트에서 지도상에 리드의 위치를 누르고 회사명을 입력, 현재 타사 테이블 오더 이용중인지(차후 지역별 자사제품 점유율에 활용) 확인하고 save 버튼누르면 리드생성
-  1. 지도위치 클릭 -> 2. 해당 위치를 위도,경도 변환 api를 활용해 위도,경도 값 받음 -> 3. 주소변환 api를 통해 위도,경도를 정확한 주소값으로 변환-> 4. 리드 필드에 저장
- 📽 [시연 영상]
- 

https://github.com/user-attachments/assets/eda019c6-99da-42bf-a046-cb8654bf881e


- 

https://github.com/user-attachments/assets/312b7c08-9907-4445-9670-338fb2c5e98a



### 📌 Feature 2 – Web-To-Case Lead Acquisition & Address Data Addition

- 모바일 폼 팩터가 주를 이루는 요즘 시대에 더욱 간편하게 사용자로하여금 정보를 입력하여 리드확보가 더 많아 지게끔 프론트엔드 페이지 제작하여 배포함.
- Web-To-Lead 문서 : [https://github.com/web-to-lead](https://github.com/LEEJUNGHOOON/webtolead)
- 📽 [시연 영상]


https://github.com/user-attachments/assets/4178a3e2-b65a-4c55-8d2c-7d1ed257e149

- 또한 업무 프로세스상 모든 고객,혹은 잠재고객의 정확한 위치가 필요하여, 주소 정보가 없는 lead일 경우 영업사원으로 하여금 쉽게 해당 리드의 위치를 확보 할 수 있게 끔 도모하는 컴포넌트 개발함
- 1. 컴포넌트에 매장의 이름을 입력-> 매장의 이름을 주소변환 api를 거쳐 정확한 주소와 위,경도 값을 return -> 해당 lead 업데이트


https://github.com/user-attachments/assets/17aa34eb-a351-4eec-980d-41584532c216



### 📌 Feature 3 – CPQ System

- 영업 팀이 주문 견적을 신속하고 정확하게 생성할 수 있도록 해주는 Drag&Drop 형태의 CPQ시스템
- opportunity가 '솔루션 제안' 단계일때 CPQ 시스템이 visible 되면 해당 고객에 맞는 제품과 수량을 간편히 입력 후 저장하면 금액,견적서 자동생성
- 영업사원이 해당 opportunity에 연관된 products를 쉽게 확인할 수 있는 컴포넌트 개발
- 📽 [시연 영상]

https://github.com/user-attachments/assets/4064ddf0-9ce4-42dc-b780-4b2f00658d14


### 📌 Feature 4 – Installation Work Assignment System (Sales Operation)

## 📖 개요
본 시스템은 고객의 설치 요청을 효율적으로 기사들에게 배정하는 기능을 제공합니다.  
Salesforce를 기반으로 기사와 작업 요청을 매칭하며, 자동화된 필터링 및 추천 알고리즘을 활용하여 최적의 기사를 배정합니다.
 ## **4-1) 기사 관리 시스템**

### 1️⃣ **기사 레코드와 User를 1:1 매칭**
- 모든 기사는 **Salesforce User**와 1:1로 연결됩니다.
- 기사의 계정 정보를 활용하여 배정 프로세스를 진행합니다.

### 2️⃣ **기사 별 서울시 관할 구역 지정**
- 각 기사에게 특정 구역을 담당하도록 할당합니다.  
  예시: 
  - 강남구, 서초구, 송파구  
  - 영등포구, 동작구, 관악구  
  - 기타 (ETC)

### 3️⃣ **기사 근무 시간 설정**
- 기사 별로 근무 가능 시간을 설정합니다.
- 예시 근무 시간:
  - **주중 09:00~18:00**
  - **주말 10:00~15:00**
  - **주중 15:00~22:00**

---

## **4-2) 설치 작업 배정 프로세스**

### 1️⃣ **고객 희망 설치 날짜 입력 & 자동 설치 레코드 생성**
- `Opportunity`에서 고객이 희망 설치 날짜를 입력합니다.
- 거래가 완료되면 자동으로 `설치 레코드(Installation Record)`가 생성됩니다.  
  - 포함 정보: **위도, 경도, 서울시 구 정보, 설치 날짜**

### 2️⃣ **CXAPP - 설치 작업 리스트 표시**
- CXAPP 좌측 영역에 **배정해야 할 설치 작업 리스트**를 표시합니다.

### 3️⃣ **설치 레코드 선택 시 적합한 기사 필터링**
설치할 위치와 날짜 정보를 기반으로 적합한 기사를 필터링합니다.

#### 📌 **필터링 단계**
1️⃣ **설치 지역을 담당하는 기사 필터링**  
   - `Installation Record`의 **구 정보**와 일치하는 기사만 선택  
   - (예: "강남구"에 설치 시, 강남구를 담당하는 기사만 조회)  

2️⃣ **설치 날짜에 근무하는 기사 필터링**  
   - `Installation Date`가 기사의 근무 일정과 일치해야 함.  
   - (예: 1월 10일에 설치 요청 → 1월 10일이 근무일인 기사만 선택)  

3️⃣ **작업 시간 충돌 여부 체크**
   - 설치 작업 시작 시간 + 소요 시간을 계산하여 **시간이 겹치는 기사 제외**  
   - 예:
     - 설치 소요 시간: **2시간**
     - 설치 예정 시간: **오후 3시**
     - 기사의 근무 종료 시간: **오후 4시** → ❌ 배정 불가  

4️⃣ **기사 작업 할당율 계산 & 추천 기사 선정**
   - 가능한 기사들 중, 해당 날짜에 **작업 할당율이 가장 낮은 기사**를 추천  
   - 작업 할당율 공식:
     ```
     (이미 배정된 작업 수) / (하루 최대 작업 가능 수)
     ```
   - 할당율이 낮을수록 가용 시간이 많은 기사 → 우선 추천

### 4️⃣ **기사 배정 및 최종 작업 할당**
- 기사와 설치 레코드를 선택 후 **배정 버튼 클릭**  
- 해당 기사에게 설치 작업이 배정됨  

---
- 📽 [시연 영상]
  

https://github.com/user-attachments/assets/8c373df9-8fb7-49b9-b4d2-634259b20281



### 📌 **기능 5 - 기사 전용 모바일 화면(Sales Operation)**
## 📖 개요
이 기능은 **기사(Salesforce User)** 가 Salesforce Mobile에서 **자신에게 배정된 작업을 효율적으로 수행**할 수 있도록 지원합니다.  
작업 일정, 지도 라우팅, 제품 리스트 확인, 네비게이션 기능을 포함하여 **현장 업무 최적화**를 목표로 합니다.

---

## 🛠 **기능 상세**

### 1️⃣ **자동 날짜 선택 & 현재 위치 수신**
- Salesforce Mobile 접속 시, 자동으로 **오늘 날짜**가 선택됨.
- 기사 현재 위치를 GPS를 통해 시스템에서 자동으로 수신.

### 2️⃣ **할당된 작업 리스트 & 지도 표시**
- 오늘 날짜에 **기사에게 배정된 작업들을 시간별 리스트**로 정렬하여 보여줌.
- **지도에 전체적인 작업 위치 데이터 시각화**
  - 📍 내 현재 위치
  - 🔵 다음 작업 위치

### 3️⃣ **작업 상세보기**
- 리스트에서 특정 작업을 선택하면 **작업 상세 화면**으로 이동.
- **설치해야 할 제품 리스트 확인**  
  - 고객이 요청한 제품 목록을 표시  
  - 설치할 제품의 모델명, 수량 등 세부 정보 제공  

### 4️⃣ **네비게이션 기능 (카카오 길 찾기 연동)**
- "길 찾기" 버튼을 누르면 **카카오 길 찾기 API**를 통해 네비게이션 가능.  
- 🚗 **출발지:** 기사 현재 위치  
- 🏠 **목적지:** 설치 작업 위치  

---

## 📽 **동영상 시연**
📌 **기능 시연 영상**


https://github.com/user-attachments/assets/d33cb13b-0df8-43a3-836a-f0936e532e34



---

## 🔄 **작업 완료 후 동작**
1️⃣ **작업이 완료되면, 리스트에서 해당 작업 삭제**  
2️⃣ **다음 작업 위치로 자동 라우팅**  
   - 현재 위치를 "이전 작업 완료 위치"로 설정  
   - 새로운 작업 위치와 내 위치를 기반으로 경로 다시 계산  

---


https://github.com/user-attachments/assets/b63ec42b-648d-459a-98e9-bb90f3da7e1c



### 📌 Feature 6 – Data Visualization & Dashboard

## 📖 개요  
이 기능은 **Salesforce 데이터를 활용한 시각적 분석**을 제공하며,  
**지도 API 및 SOQL 쿼리**를 활용하여 **서울시 권역별 영업 데이터를 시각화**하는 것이 목표입니다.  

---

## 🛠 **1️⃣ 서울시 구별 지도 Layer 적용**  
- 📌 **Leaflet 지도 API**와 **공공데이터(GeoJSON)**를 활용하여 서울시 **자치구별 Layer**를 적용  
- 🔗 사용 데이터: [Korea District GeoJSON](https://github.com/cubensys/Korea_District)  
- 🎯 **서울시 권역별로 색을 다르게 표현하여 구분**  

🖼 **서울시 권역별 지도 Layer 적용 화면**  

<img width="453" alt="스크린샷 2025-03-10 오후 1 50 09" src="https://github.com/user-attachments/assets/c21302ad-b210-49ef-b728-2ca97ae8fe61" />

---

## 🛠 **2️⃣ 타사 사용 매장 & 설치 완료 매장 시각화**  
### **💾 데이터 수집**  
- 기능 1️⃣ **타사 테이블오더 사용 매장 (`Lead` 오브젝트)**  
- 기능 4️⃣, 5️⃣ **설치가 완료된 매장 (`Work` 오브젝트)**  
- **SOQL 쿼리**를 통해 데이터를 조회하여 지도에 마커를 표시  

### **📍 지도에 다른 색상 마커로 시각화**  
- 🔵 **타사 테이블오더 사용 매장** → `파란색 마커`  
- 🔴 **설치 완료 매장** → `빨간색 마커`  

🖼 **매장 데이터 시각화 예시**  
<img width="452" alt="스크린샷 2025-03-10 오후 1 50 30" src="https://github.com/user-attachments/assets/5c4a9639-d4d1-401a-86eb-3a241a97b5d1" />


✅ **기대 효과**  
- 권역별 **설치 점유율** 및 **핫한 상권**을 한눈에 파악 가능  
- 영업사원이 **어떤 지역을 우선 공략할지 전략 수립 가능**  

---

## 🛠 **3️⃣ 리드(Lead)별 우선순위 시각화**  
- `Lead` 오브젝트에서 **중요도(priority)** 를 설정하여 **지도에서 다른 마커로 표현**  
- **중요도 높은 리드** → `초록색 마커`  
- **중요도 중간 리드** → `빨간색 마커`  
- **중요도 낮은 리드** → `노란색 마커`  

✅ **기대 효과**  
- 특정 권역에 **중요한 리드가 밀집되어 있는지 시각적으로 파악 가능**  
- 해당 데이터를 바탕으로 **권역별 영업 인력 증원 여부 결정 가능**  

🖼 **권역별 리드 중요도 시각화 예시**  

| 리드 우선순위 필드 | 리드 중요도 분석 |
|-----------------|-----------------|
| <img width="913" alt="리드 우선순위 필드" src="https://github.com/user-attachments/assets/17b17d12-9916-4136-891b-7fd4ff6aa558" /> | <img width="449" alt="리드 중요도 분석" src="https://github.com/user-attachments/assets/fab2a65f-90a8-40e9-8c7d-13509ab6e9f4" /> |


---

## 🎯 **기대 효과**  
✅ 권역별 **설치 점유율 및 영업 기회 분석 가능**  
✅ **핫한 상권 및 공략 지역 선정 가능**  
✅ **영업사원의 배치 최적화 & 전략적 영업 가능**  

---

> 🚀 **이 기능은 Leaflet 지도 API와 Salesforce 데이터를 연동하여, 영업 활동을 효과적으로 시각화하고 전략적으로 활용할 수 있도록 설계되었습니다.**

### 📌 Feature 7 – Tableau Dashboard

## 📖 개요  
이 기능은 **Tableau를 활용한 시각적 데이터 분석 대시보드**를 제공합니다.  
**서울시 권역별 설치 데이터**를 매핑하고, **총 설치 수 & 점유율 분석**을 통해 CEO가  
**빠르고 직관적인 의사결정**을 할 수 있도록 설계되었습니다.  

---

## 🛠 **1️⃣ 권역별 설치 데이터 매핑**  
- **Tableau 지도(Map) 시각화 기능을 활용하여 설치된 매장을 권역별로 시각화**  
- 서울시 전체 지도에서 각 자치구별로 **설치된 매장 수를 색상으로 구분**  
- 특정 구역을 클릭하면 **해당 구역의 점유율**을 확인 가능  

🖼 **권역별 설치 데이터 매핑 예시**  

<img width="920" alt="스크린샷 2025-03-10 오후 2 45 13" src="https://github.com/user-attachments/assets/1bfc7f7f-5c35-42e6-a3fe-34240e7986cf" />

---


## 🛠 **2️⃣ 권역별 점유율 분석 (도넛 차트 활용)**  
- **도넛 차트(Donut Chart)를 활용한 권역별 점유율 분석**  
- 권역별로 **설치된 제품 비율을 한눈에 확인 가능**  
- **각 권역을 클릭하면 해당 구역의 세부 데이터로 Drill-Down 가능**  

🖼 **권역별 점유율 도넛 차트 예시**  

| 용산구 | 송파구 |
|-----------------|-----------------|
| <img width="930" alt="스크린샷 2025-03-10 오후 2 45 51" src="https://github.com/user-attachments/assets/73b5bbde-4e62-4802-8e1c-686bdb652fdf" /> | <img width="929" alt="스크린샷 2025-03-10 오후 2 47 42" src="https://github.com/user-attachments/assets/d00230d4-d9c4-41e5-aa7b-75ce2bc0a371" />|
---

## 🎯 **기대 효과**  
✅ **CEO가 제품 설치 현황을 직관적으로 파악 가능**  
✅ **구역별 점유율 & 시장 트렌드 분석 가능**  
✅ **필터링 기능을 통한 맞춤형 데이터 조회 가능**  
✅ **데이터 기반으로 최적의 의사결정 지원**  

---
태블로 퍼블릭에서 보기 : https://public.tableau.com/app/profile/junghoon.lee3688/viz/Team5Tableau/2

> 🚀 **이 대시보드는 Tableau의 강력한 시각화 기능을 활용하여, 설치 데이터의 흐름을 명확하게 파악하고,  
> 비즈니스 전략을 최적화할 수 있도록 설계되었습니다.**

---

### 📌 Feature 8 – CTI Integration(Amazon Connect & Salesforce)

## 📖 개요  
이 기능은 **상담원**이 Service Console에서 빠른 문제해결이 필요한 고객층인 **자영업자들의 전화 문의를 효율적으로 처리**할 수 있게 지원하며,  
화면 전환없이 고객을 **파악**하고 문의를 **기록**하는 것을 목표로 합니다.

---

## 🛠 **기능 상세**

### 1️⃣ **전화번호 기반 고객 정보 실시간 조회**
- **Amazon Connect**로 수신된 전화번호를 **AWS Lambda**를 활용
- **Salesforce**의 Contact 데이터와 비교해 **실시간 조회**

### 2️⃣ **Case 자동 생성 및 **
- 상담원이 전화 수락 시. **고객 정보 기반의 Case 자동 생성** 
- 해당 Case에서 **통화 내용 기록** 및 Knowledge를 이용한 **빠른 상담 가능**

---

## 📽 **동영상 시연**

https://github.com/user-attachments/assets/e65d6e9f-b216-4046-b263-4a8e17e7dd8b


---

✅ **기대 효과**  
- **상담원의 업무 효율성 향상**
- **고객 응대 품질 개선** 


### 🚀 ETC (기타 기능)

본 섹션에서는 **추가적인 UI/UX 개선 기능**을 소개합니다.  
이 기능들은 **사용자 경험(UX) 최적화 및 직관적인 인터페이스 제공**을 목적으로 설계되었습니다.

---

## 🛠 **1️⃣ Dock (네비게이션 컴포넌트)**  

📌 **개요**  
- Mac 환경의 **하단 Dock 바**를 모티브로 하여,  
  **Home / Record 페이지 간 쉽고 직관적인 이동**을 지원하는 네비게이션 컴포넌트 제작  

📌 **특징**  
✅ **아이콘 기반 네비게이션**  
✅ **애니메이션 효과 적용 (Hover 및 Active 상태 반응)**  
✅ **모든 페이지에서 일관된 사용자 경험 제공**  

🖼 **Dock UI 예시**  



https://github.com/user-attachments/assets/685daa1e-0952-4d42-8ff2-b45543b9d8e1



---

## 🛠 **2️⃣ Experience Cloud 페이지 (고객 랜딩 페이지 UX/UI 디자인)**  

📌 **개요**  
- **Salesforce Experience Cloud** 기반의 **고객 랜딩 페이지 UX/UI 최적화**  
- 고객이 **Product 카탈로그를 쉽게 탐색**할 수 있도록 **슬라이드 UI 적용**  
- 상세 페이지에서 **SOQL 쿼리를 활용하여 제품 정보 조회**  

📌 **기능 세부 사항**  

### 🔹 **1. Product 카탈로그 (슬라이드 UI)**
- 제품을 **슬라이드 형식으로 UI 디자인**
- 고객이 **좌/우로 스크롤하며 제품 탐색 가능**  
- 각 제품 카드를 클릭하면 상세 페이지로 이동  

### 🔹 **2. Product 상세 페이지 (SOQL 데이터 조회)**
- **SOQL 쿼리**를 통해 **선택된 제품 ID**를 기반으로 상세 정보를 조회  
- **표시되는 정보:**  
  ✅ 제품 설명  
  ✅ 가격  
  ✅ 화면 크기 (인치)  
  ✅ 추가 옵션  


📌 **UX/UI 최적화 요소**  
✅ **고객 중심의 직관적인 UI 설계**  

---

## 🎯 **기대 효과**
✅ **페이지 이동이 쉬운 Dock UI → 사용자 경험(UX) 개선**  
✅ **Experience Cloud에서 고객이 원하는 제품을 빠르게 찾을 수 있도록 UX 최적화**  
✅ **SOQL 연동을 통해 정확한 제품 상세 정보 제공**  
✅ **고객이 쉽게 탐색할 수 있는 Product Slide UI 도입**  




https://github.com/user-attachments/assets/2a74c090-2a40-4bf1-a6d4-029f88e340e4




---

> 🚀 **이 기능들은 Salesforce 플랫폼의 UX/UI를 개선하여,  
> 사용자가 더욱 직관적이고 편리하게 시스템을 사용할 수 있도록 설계되었습니다.**






## 7️⃣ API & SOQL

📌 **API 및 SOQL 쿼리는 [Wiki Page](https://github.com/LEEJUNGHOOON/salesforceproject/wiki)에 정리했습니다.**  
🔗 **[📖 API 문서 바로가기](https://github.com/LEEJUNGHOOON/salesforceproject/wiki/API)**  
🔗 **[📖 APEX & SOQL 문서 바로가기](https://github.com/LEEJUNGHOOON/salesforceproject/wiki/APEX-&-SOQL)**  

---

## 📌 **8️⃣ 기술 스택**
📌 **프로젝트에서 사용된 주요 기술 스택**

### **💻 Backend**
- ![Apex](https://img.shields.io/badge/Apex-0055CC?style=flat&logo=salesforce&logoColor=white)
- ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
- ![SFDX](https://img.shields.io/badge/SFDX-00A1E0?style=flat&logo=salesforce&logoColor=white)
- ![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-F90?logo=aws-lambda&logoColor=white)

### **🎨 Frontend**
- ![LWC](https://img.shields.io/badge/LWC-0070D2?style=flat&logo=salesforce&logoColor=white)

### **🗄 Database**
- ![SOQL](https://img.shields.io/badge/SOQL-00A1E0?style=flat&logo=salesforce&logoColor=white)

### **☁️ 서버**
- ![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat&logo=netlify&logoColor=white)

### **🛠 협업 툴**
- ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
- ![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat&logo=jira&logoColor=white)
- ![Miro](https://img.shields.io/badge/Miro-050038?style=flat&logo=miro&logoColor=yellow)
- ![Notion](https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white)

---

## 📌 **9️⃣ 문의**
📧 이메일: [wjdgns9799@gmail.com](mailto:wjdgns9799@gmail.com)  
🐙 GitHub: [LEEJUNGHOOON](https://github.com/LEEJUNGHOOON)  

---

## 📌 **🔟 레퍼런스**
본 프로젝트는 아래의 문서를 참고하여 개발되었습니다.

- 📌 **Salesforce 공식 Help 문서**  
  🔗 [Salesforce Help Center](https://help.salesforce.com/)  

- 📌 **LWC 컴포넌트**  
  🔗 [Sudeer Kamat's GitHub](https://github.com/SudeerKamat)  

- 📌 **Trailhead Salesforce Quick Start**  
  🔗 [Quick Start: eBikes Sample App](https://trailhead.salesforce.com/ko/content/learn/projects/quick-start-ebikes-sample-app/get-to-know-app-ebikes)  

- 📌 **Aamoos 블로그 (Tistory)**  
  🔗 [leaflet 관련 자료](https://aamoos.tistory.com/428)  

---

> 🚀 **이 프로젝트는 오픈소스로 개발되었습니다. 많은 참여 부탁드립니다!**  
> 🙌 좋아요(⭐)와 Fork를 눌러주시면 큰 힘이 됩니다!
