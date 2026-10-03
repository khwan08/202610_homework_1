# OncoTarget AI — 췌장암 KRAS G12R 정밀 신약 발굴 플랫폼

> **Google DeepMind Science Skills & Google Stitch 아키텍처 기반의 1인 딥테크(TechBio) 가상 바이오텍 인텔리전스 플랫폼**

---

## 📌 과제 제출용 핵심 문서 및 바로가기 링크

본 프로젝트는 단순 코드나 텍스트가 아닌, **실제 동작하는 3D 인터랙티브 웹 플랫폼**, **창업 마스터 슬라이드 시스템**, **A4 제출용 최종 보고서**로 구성되어 있습니다.

| 번호 | 문서 및 사이트 링크 | 내용 및 용도 |
| :---: | :--- | :--- |
| **1** | [**과제 최종 보고서 (Markdown)**](file:///c:/Users/Khwan/Desktop/학교과제/과제_최종보고서_OncoTarget_AI.md) | 학술적 배경, 생화학 메커니즘, 5대 공격 무기, 1인 딥테크 비즈니스 모델이 총망라된 공식 제출용 보고서 |
| **2** | [**과제 제출용 보고서 (인쇄/PDF 뷰어)**](file:///c:/Users/Khwan/Desktop/학교과제/과제_제출용_보고서.html) | A4 레이아웃 및 상단 [PDF로 저장/인쇄] 버튼이 탑재된 브라우저 전용 제출용 문서 |
| **3** | [**OncoTarget AI 메인 플랫폼**](file:///c:/Users/Khwan/Desktop/학교과제/index.html) | Google Stitch 디자인 시스템이 적용된 실시간 3D 분자 포켓 회전, 다중오믹스 합성치사 지도, 도즈-반응 시뮬레이터 |
| **4** | [**창업 학습 슬라이드 (13 Slides)**](file:///c:/Users/Khwan/Desktop/학교과제/slides.html) | 키보드 방향키(`←`, `→`) 네비게이션을 지원하는 6개 모듈 인터랙티브 프레젠테이션 |

---

## 🔬 핵심 연구 요약 (Executive Summary)

* **타깃 질환**: 췌관선암종 (PDAC, 5년 생존율 < 10%)
* **표적 3중 변이**:
  1. **KRAS G12R**: 암세포 증식의 구동 엔진 (Arg12의 양전하 구아니디늄 잔기 돌출로 기존 G12C 폐암약 무력화)
  2. **EP300 Loss**: 히스톤 아세틸화 조절 마비로 암세포가 쌍둥이 단백질인 **CBP(CREBBP)에 100% 생존을 의존**
  3. **SMAD4 Deletion**: 종양 억제 경로 차단 및 **DNA 상동재조합복구(HRR) 결함** 유발
* **5대 공격 무기**:
  1. `α,β-케토아마이드` Arg12 비가역 공유결합 (PDB: 8CX5, 1.85Å, IC50 = 14.2 nM)
  2. `Daraxonrasib` CypA 삼중 복합체 분자 접착제 (PDB: 9BGC, Kd = 0.8 nM)
  3. `CRBN E3 리가아제` 기반 PROTAC 표적 단백질 완전 분해 (ChEMBL5483196)
  4. `거대음세포작용(Macropinocytosis)` 대사 중독을 역이용한 나노 트로이목마
  5. `CBP 분해(dCBP-1)` + `PARP 억제(Olaparib)` 3중 합성치사 동시 타격 (**시너지 지수 CI = 0.24**)
* **1인 딥테크(TechBio) 사업화 로드맵**:
  * **엔진 1**: B2B 타깃 실사 리포트(Dossier) 판매 (건당 $3,000~$5,000, 즉각적인 현금흐름)
  * **엔진 2**: 독점 물질특허(IP) 출원 $\to$ 글로벌 CRO(WuXi) 세포 검증 $\to$ 빅파마 조기 기술이전 (계약규모 5,000억 원+, 유니콘 등극)

---

## 💻 실행 및 확인 방법

1. 브라우저(크롬, 엣지 등)에서 [`index.html`](file:///c:/Users/Khwan/Desktop/학교과제/index.html)을 더블클릭하여 인터랙티브 대시보드를 확인합니다.
2. 발표 및 커리큘럼 복습 시 [`slides.html`](file:///c:/Users/Khwan/Desktop/학교과제/slides.html)을 실행합니다.
3. 과제 제출 시 [`과제_제출용_보고서.html`](file:///c:/Users/Khwan/Desktop/학교과제/과제_제출용_보고서.html) 우측 상단의 **[PDF로 저장 / 인쇄]** 버튼을 눌러 PDF 파일로 저장 후 제출합니다.
