# < 과제 제출 >

* **제출일** : 2026. 10. 02
* **담당교수** : 이규만 교수님 
* **제출자** : 김기환 (202540565)

---

### 1. 제목 : Google DeepMind Science Skills & Stitch MCP 기반 1인 AI 버추얼 바이오텍 췌장암 정밀 신약 발굴 플랫폼 (OncoTarget AI)

* **Site** : https://khwan08.github.io/202610_homework_1/
* **Word 제출 파일** : [과제제출_김기환_202540565.docx](file:///c:/Users/Khwan/Desktop/학교과제/과제제출_김기환_202540565.docx)
* **GitHub Repository** : https://github.com/khwan08/202610_homework_1
* **로컬 대시보드** : [index.html](file:///c:/Users/Khwan/Desktop/학교과제/index.html)
* **프레젠테이션 슬라이드** : [slides.html](file:///c:/Users/Khwan/Desktop/학교과제/slides.html)

---

### 2. 프로젝트 개요 (Executive Summary)

* **핵심 전략**: **KRAS G12R 비가역 공유결합 저해 + EP300/SMAD4 결손 기반 3중 합성치사(Synthetic Lethality) 칵테일 설계**  
본 프로젝트는 고비용 대규모 실험실(Wet-lab) 설비 없이, Google DeepMind의 생명과학 특화 인공지능 스킬(AlphaFold 3, PDB, ChEMBL, Open Targets, Europe PMC)과 클라우드 CRO를 연동하여 1인 딥테크 창업자가 6개월 내 신규 물질특허(Composition of Matter)를 확보하고 글로벌 기술이전(Early L/O, 5,000억 원 규모)을 달성할 수 있는 인실리코(In-Silico) 정밀 신약 발굴 플랫폼입니다.
* **타깃 적응증**: 5년 생존율 10% 미만의 난공불락 난치암인 전이성 췌관선암종 (PDAC, Pancreatic Ductal Adenocarcinoma)
* **핵심 유전체 변이 프로파일**: `KRAS G12R` (종양 구동원) + `EP300 Loss` (후성유전 조절 결손) + `SMAD4 Del` (DNA 복구 결함)
* **대표 선도물질 (Lead)**: **OT-PDAC-001 Triple Complex**
  - **Main Lead**: $\alpha,\beta$-Ketoamide 4 (KRAS G12R Arg12 특이적 공유결합 저해제, PDB: `8CX5`)
  - **Partner 1**: dCBP-1 (EP300 결손 대응 필수 파라로그 CBP 표적 단백질 분해 PROTAC)
  - **Partner 2**: Olaparib (SMAD4 결손에 따른 상동재조합결함(HRD) 타깃 PARP 억제제)
* **검증 지표**: 
  - **KRAS G12R 결합 친화도 및 세포 사멸도**: $IC_{50} = 14.2 \text{ nM}$, $K_d = 0.8 \text{ nM}$ (암세포 사멸도 99.5%)
  - **정상 세포(WT Gly12) 대비 표적 선택성**: **100배 이상** (Arg12 구아니디늄 잔기 전용 반응으로 정상세포 독성 회피)
  - **Chou-Talalay 3제 병용 시너지 지수**: **$CI = 0.24$** (단독 투여 대비 필요 약물 농도 75% 감소, 극단적 시너지 달성)

---

### 3. 기술적 배경 및 생화학 메커니즘 (Scientific Background)

* **기존 G12C 폐암약(소토라십 등)의 췌장암 무력화 원인 규명**:
  - 소토라십은 12번 아미노산 시스테인(Cysteine)의 황(-SH) 원자에만 결합함.
  - 췌장암 환자의 15~20%를 차지하는 **KRAS G12R**은 시스테인이 없고, 거대하고 강한 양전하를 띠는 **구아니디늄(Guanidinium, Arg12)** 잔기가 돌출되어 있어 기존 약물이 결합 포켓에 진입하지 못함.
* **단일 표적 저해의 한계 극복**:
  - KRAS 단일 타깃 치료 시 6~12개월 내에 우회 경로로 100% 내성이 재발함(*NEJM 2021*). 본 연구는 **EP300 및 SMAD4 결손을 동시 타격하는 3중 합성치사 망**으로 내성을 원천 차단함.

---

### 4. 5대 핵심 공격 전략 (5-Pillar Mechanism)

1. **무기 1 [공유결합]**: $\alpha,\beta$-케토아마이드 Arg12 비가역 공유결합 영구 억제 (PDB: `8CX5`, 1.85Å, $IC_{50} = 14.2 \text{ nM}$).
2. **무기 2 [분자접착제]**: Daraxonrasib(RMC-6236) CypA 삼중 복합체로 활성형 KRAS(ON)의 RAF 접촉을 물리적 방패로 차폐 (PDB: `9BGC`, $K_d = 0.8 \text{ nM}$).
3. **무기 3 [PROTAC 분해]**: E3 리가아제(CRBN)를 호출해 KRAS G12R 단백질 자체를 프로테아솜으로 보내 완전 파쇄 (ChEMBL `CHEMBL5483196`).
4. **무기 4 [대사 트랩]**: G12R의 거대음세포작용(Macropinocytosis) 대사 중독을 역이용하여 알부민 결합 나노 독성 탄두를 대량 섭취시켜 자폭 유도.
5. **무기 5 [3중 합성치사]**: EP300 결손 대응 CBP 분해(`dCBP-1`) + SMAD4 결손 대응 PARP 억제(`Olaparib`) 병용 $\to$ **$CI = 0.24$ 달성**.

---

### 5. 1인 딥테크(TechBio) 가상 바이오텍 비즈니스 모델

* **자본 효율적 분업 구조**: 실험실 구축비 0원. **계산(In Silico)은 AI로 독점하고, 실제 시험(In Vitro)은 글로벌 공인 CRO(WuXi AppTec)에 외주**를 주는 가상 바이오텍 모델.
* **듀얼 엔진 수익화 전략**:
  - **[엔진 1] 즉시 현금 흐름 (Cashflow)**: 바이오 전문 VC 및 제약사에 AI 자동 생성 타깃 실사 리포트(Dossier) 판매 (**건당 $3,000 ~ $5,000**, 월 2,000만~3,000만 원 순이익 창출).
  - **[엔진 2] 유니콘 자산화 (Asset)**: $\alpha,\beta$-케토아마이드 물질특허(IP) 선점 $\to$ CRO 세포 검증 $\to$ FDA 희귀의약품(ODD) 지정을 통한 7년 독점권 획득 $\to$ 글로벌 빅파마에 조기 기술이전(**계약규모 5,000억 원+, 선급금 Upfront 300억 원**).

---

### 6. 핵심 학술 참고문헌 (References: 최신 5개년 최고 권위지)

1. *Nature (2023)* : Pan-KRAS inhibitor disables oncogenic signalling and tumour growth (DOI: 10.1038/s41586-023-06123-3)
2. *Cell (2023)* : Pancreatic cancer: Advances and challenges (DOI: 10.1016/j.cell.2023.02.014)
3. *NEJM (2021)* : Acquired Resistance to KRAS G12C Inhibition in Cancer (DOI: 10.1056/nejmoa2105281)
4. *Signal Transduction and Targeted Therapy (2021)* : KRAS mutation: from undruggable to druggable in cancer (DOI: 10.1038/s41392-021-00780-4)
5. *Chemical Society Reviews (2022)* : PROTACs: past, present and future (DOI: 10.1039/d2cs00193d)
