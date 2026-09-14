# 인사 정보 그리드 - React + MESCIUS Wijmo

**React + MESCIUS Wijmo**로 구현한 인사 정보 관리용 데이터 그리드입니다. 사원 정보를 Grid로 조회하고 검색·필터링하며, 컬럼 표시 설정, 인사등급 필터, 신규 행 추가 및 Excel/PDF/인쇄 기능을 제공합니다.

## 주요 기능

- 사원 정보 데이터 Grid 표시
- Grid 검색 및 필터링
- 인사평가 등급별 필터
- 상위 3개 컬럼 고정
- 컬럼 표시/숨김 설정
- 사원 정보 신규 행 추가
- Excel / PDF 내보내기
- Grid 데이터 인쇄
- 인사평가 등급별 셀 스타일 표시
- 한국어 Wijmo Culture 적용

## 사용 기술

- React 18.3
- JavaScript
- MESCIUS Wijmo 5.20241.19
- Bootstrap CSS 3.3.7
- react-use-event-hook

## 사용된 Wijmo 컴포넌트

| 컴포넌트 | 사용 목적 |
|---|---|
| FlexGrid | 사원 정보 데이터 표시 |
| FlexGridColumn | 사원 정보 컬럼 구성 |
| FlexGridFilter | 컬럼별 데이터 필터링 |
| FlexGridSearch | Grid 검색 기능 |
| Selector | 행 선택 기능 |
| CollectionView | 데이터 관리 및 신규 행 처리 |
| ComboBox | 인사등급 필터 및 입력 항목 |
| InputDate | 생년월일·입사일자 입력 |
| InputNumber | 근속년도 입력 |
| Popup | 신규 사원 정보 입력창 |
| ListBox | 컬럼 표시/숨김 선택 |
| FlexGridXlsxConverter | Excel 내보내기 |
| FlexGridPdfConverter | PDF 내보내기 |
| PrintDocument | Grid 인쇄 |

## 화면 구성

- **검색 영역**: 사원 정보 검색
- **인사등급 필터**: 전체 / A / B / C 등급별 데이터 필터링
- **내보내기**: Excel, PDF, Print 선택
- **사원 정보 추가**: 이름, 사원번호, 생년월일, 연락처, 부서, 직위, 근무지, 근속년도, 승급자격, 인사평가 입력
- **Grid**: 사원번호, 이름, 생년월일, 부서, 직위, 연락처, 이메일, 근무지, 근속년도, 입사일자, 승급자격, 인사평가 표시
- **컬럼 설정**: Grid 좌측 상단 설정 아이콘을 통해 컬럼 표시 여부 변경
- **인사평가 표시**: A/B/C 등급에 따라 셀 스타일 구분

## 프로젝트 구조

```text
.
├── package.json
├── public/
│   └── index.html
└── src/
    ├── index.js
    ├── data.js
    ├── style.css
    ├── search.svg
    ├── AddNewPopup.js
    ├── ColumnPicker.js
    ├── ExportComboBox.js
    └── StatusComboBox.js
```

- `index.js`: 메인 Grid 및 전체 화면 구성
- `data.js`: 사원 정보 샘플 데이터
- `AddNewPopup.js`: 신규 사원 정보 입력 Popup
- `ColumnPicker.js`: Grid 컬럼 표시/숨김 설정
- `ExportComboBox.js`: Excel, PDF, Print 기능
- `StatusComboBox.js`: 인사평가 등급 필터
- `style.css`: Grid 및 Popup UI 스타일

## 설치 및 실행

```bash
npm install
npm start
```

브라우저에서 `http://localhost:3000`으로 접속합니다.

## 빌드

```bash
npm run build
```

## 데이터

`src/data.js`에 정의된 사원 정보 샘플 데이터를 `CollectionView`에 연결하여 사용합니다.

주요 데이터:
- 사원번호 및 사원명
- 생년월일 및 입사일자
- 부서 및 직위
- 전화번호 및 이메일
- 근무지
- 근속년도
- 승급자격 충족 여부
- 인사평가 등급

별도의 DB나 외부 API 연동 없이 프로젝트에 포함된 데이터를 기반으로 동작합니다.

## 활용 사례

- 인사 정보 관리 시스템
- 사원 데이터 관리 및 조회
- HR Dashboard 및 Data Grid
- 인사평가 데이터 분석
- 대규모 사내 데이터 테이블
- React 기반 Enterprise UI
- Wijmo FlexGrid 활용 사례

## 태그

`wijmo`, `mescius-wijmo`, `react`, `javascript`, `flexgrid`, `flexgridfilter`, `flexgridsearch`, `collectionview`, `flexgrid-xlsx`, `flexgrid-pdf`, `printdocument`, `hr-dashboard`, `hr-management`, `employee-management`, `employee-data-grid`, `data-grid`, `enterprise-ui-components`, `react-dashboard`, `business-application`
