# 프로젝트 2 - AI 문의 요약 자동화

## 1. 자동화 대상 업무

반복적으로 접수되는 고객 문의를 확인하고 요약하여 관리하는 업무

---

## 2. 선정 도구

Make

### 선정 이유

* Google Sheets 연동이 용이함
* Google Gemini AI 연동 가능
* 조건 분기 기능 제공
* 시각적 워크플로우 구성 가능

---

## 3. 워크플로우 설계

Google Form 제출

↓

Google Sheets 신규 행 감지

↓

Google Gemini AI 문의 분석

↓

Google Sheets 저장

↓

긴급 문의 여부 확인

↓

Gmail 알림

---

## 4. Trigger

Google Sheets - Watch New Rows

Google Form 응답이 저장되면 자동 실행

---

## 5. Action

### Action 1

Google Gemini AI

문의 내용 요약 및 분류

### Action 2

Google Sheets

분석 결과 저장

### Action 3

Gmail

긴급 문의 알림 발송

---

## 6. Filter

문의 유형이 "긴급"인 경우에만 Gmail 발송

---

## 7. 실행 결과

문의가 접수되면 Gemini AI가 자동으로 내용을 분석하였다.

분석 결과는 별도의 시트에 저장되었으며 긴급 문의는 Gmail 알림이 자동 발송되었다.

---

## 8. AI 활용 효과

기존에는 문의 내용을 직접 확인하고 정리해야 했으나 Gemini AI를 활용하여 자동 요약이 가능하였다.

이를 통해 반복 업무를 줄이고 업무 처리 속도를 향상시킬 수 있었다.
