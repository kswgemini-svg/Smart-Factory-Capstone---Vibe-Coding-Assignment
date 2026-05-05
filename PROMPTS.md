# PROMPTS LOG

## 1. 과제 목표
- 타겟 논문: Enhancing object pose estimation for RGB images in cluttered scenes
- 목표: AI 코딩 툴을 활용하여 오픈소스 코드 구현/분석 수행

## 2. 사용 도구
- ChatGPT (Codex 계열 보조)
- Google Colab
- Kaggle API
- Python (pandas, matplotlib, opencv)

## 3. 실제 사용한 프롬프트 요약
1. "논문 데이터셋 다운로드 및 Colab 실행 절차를 단계별로 알려줘."
2. "Linemod/Occlusion 데이터 구조를 확인하고 샘플 이미지를 시각화하는 코드를 작성해줘."
3. "객체 ID(01~15)를 객체명으로 매핑해서 분포 그래프를 그리는 코드를 작성해줘."
4. "분석 결과를 보고서용 문장으로 정리해줘."

## 4. 실행 과정 로그 요약
- Kaggle 토큰 기반으로 데이터셋 다운로드 수행
- `/content/linemod_data` 압축 해제 완료
- RGB 이미지 기준 객체 분포 분석 수행
- 결과 파일 생성:
  - `object_distribution_rgb_only.csv`
  - `object_distribution_rgb_only.png`

## 5. 오류와 해결
- Python 셀에 bash 코드 혼합으로 문법 오류 발생 → 셀 분리로 해결
- Kaggle 인증 방식 혼동(json/token) → token 방식으로 해결
- 객체명이 unknown만 나오는 문제 → LINEMOD ID 매핑 규칙 적용으로 해결

## 6. 최종 산출물
- 실데이터 기반 객체 분포 CSV
- 실데이터 기반 객체 분포 그래프 PNG
- 분석 보고서 본문(매뉴얼 + 결과 해석)
