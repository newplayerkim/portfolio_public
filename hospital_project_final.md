
# Project with UML
## Hospital Reservation
due : 2025/07/17~18  
member : omission  
part : use case diagram, class diagram, activity diagram  
theme : hospital reservation  

---

## 사용 기술 스택 (Technology Stack)

### 🔹 현재 사용 기술
- **UML 도구**: draw.io  
  → Use Case, Activity, Class Diagram 작성

- **Markdown**  
  → 문서화 및 보고서 작성

- **데이터베이스(DB)**: MySQL, MongoDB  
  → 예약 정보, 사용자 정보 저장

- **버전 관리**: Git, GitHub  
  → 파일 관리 및 온라인 공개용

### 🔹 기술 스택 
- **프론트엔드**: HTML / CSS  
  → 병원 예약 시스템의 사용자 인터페이스(UI) 구현 시 사용 가능

- **백엔드**: Java / Python / Node.js 등 
  → 실제 예약 기능을 구현할 경우의 서버 언어 예시

- **데이터베이스**: MySQL / SQLite   
  → 예약 정보, 사용자 정보 등을 저장할 수 있는 관계형 DB

---

## 나의 파트

이번 병원 예약 시스템 UML 프로젝트에서 프론트엔드 역할을 맡아 사용자 인터페이스(UI)와 화면 흐름을 설계하며, 프론트엔드 개발의 본질을 이해하는 계기가 되었습니다.

특히 Use Case Diagram과 Activity Diagram을 바탕으로 사용자 경험(UX)과 논리적 흐름이 밀접하게 연결된다는 점을 체감했고, 예약 과정에서의 버튼 위치, 입력 방식 등 다양한 UI 요소의 중요성을 깨달았습니다.

향후 HTML, CSS, JavaScript 등 기초 기술부터 React 같은 프레임워크까지 차근차근 익히며 역량을 키우고 싶습니다.

---

## 1. Use Case Diagram

![Use Case Diagram](usecasediagramimage)

설명:  
Use Case Diagram은 환자(Patient), 의사(Doctor)와 시스템 간의 상호작용을 기반으로 병원 예약 프로그램을 설계한 것입니다.

주요 액터:  

### 1. **환자 (Patient)**

- **Login (로그인)**  
  - 시스템 사용을 위해 인증 과정이 필요하며, 로그인 후 예약 기능에 접근할 수 있습니다.

- **예약 (Make Reservation)**  
  - 의사의 진료 가능 시간표를 조회하고, 본인의 일정을 고려해 진료 예약을 생성합니다.

- **예약된 일정 확인 (Check Reservation)**  
  - 기존에 예약된 진료 일정을 조회해 확인할 수 있습니다. 향후 진료 준비나 시간 조율에 사용됩니다.

- **예약 변경 (Modify Reservation)**  
  - 이미 생성된 예약의 일시 또는 의사를 변경하는 기능입니다. 일정 충돌이나 개인 사정이 생겼을 때 활용됩니다.

- **예약 취소 (Cancel Reservation)**  
  - 더 이상 진료가 필요 없거나 일정이 불가능할 경우, 예약을 시스템에서 제거합니다.

### 2. **의사 (Doctor)**

- **Login (로그인)**  
  - 시스템 사용을 위해 인증 과정이 필요하며, 로그인 후 예약 기능에 접근할 수 있습니다.

- **일정 수립 (Set Schedule)**  
  - 의사는 자신이 가능한 진료 시간대를 시스템에 등록합니다. 이 정보는 환자들이 예약할 수 있는 기준 시간표가 됩니다.

---

## 2. Activity Diagram

![Activity Diagram](activitydiagramimage)

설명:  
액티비티 다이어그램은 실제 프로세스 흐름을 나타내며, 예약 조건 및 의사 일정 업데이트 조건에 따라 실행됩니다.

---

## 3. Class Diagram

![Class Diagram](classdiagramimage)

설명:  
클래스 다이어그램은 병원 예약 시스템의 주요 클래스 구조를 보여줍니다.

주요 클래스:
- `User` → `Doctor`, `Patient` 상속  
- `Reservation`, `Schedule`, `MedicalRecord` 클래스는 예약 및 진료 기록 정보 관리  
- `Hospital` 클래스는 예약 및 진료 데이터 총괄

---

## 4. Conclusion

이 프로젝트는 병원 예약 시스템의 구조를 UML 기반으로 시각화한 것입니다.  
- 사용자 흐름 (Use Case)  
- 작업 흐름 (Activity)  
- 데이터 구조 (Class)  

### 추후 확장 가능 항목:
- 관리자 기능  
- 예약 알림 기능  
- 진료 대기 시간 예측  

---

## 5. 느낀점

### ✅ 좋은 점
- 개발하는 과정을 직·간접적으로 체험해볼 수 있는 좋은 계기였다.
- 추가 메서드(의사와 관리자 구분, 우선순위 환자 예약 등)를 구현하고 싶었으나 자원(시간, 노력) 부족으로 구현하지 못했지만, 이런 조율 과정이 중요하다는 것을 깨달았다.
- UML 도구 사용법을 습득했다.
- 컴퓨터공학부 특성상 졸업작품을 위한 사전 연습이 되어 도움이 되었다고 생각한다.

### ❌ 아쉬운 점
- 1학년이라 실사용 가능한 개발 스택이 거의 없어 실제 프로젝트에서는 활용이 어렵다는 점이 속상했고, 이를 보완해나갈 것이다.
- 사실 개발자가 꿈은 아니고 다른 분야에 관심이 더 있지만, 앞으로 수업을 들으며 차근차근 진로를 결정해나갈 계획이다.
- 목요일 저녁만 사용할 수 있어서 순서도 작성도 미흡했다고 느꼈다. 시간이 더 주어진다면 보완 가능하다고 생각한다.
