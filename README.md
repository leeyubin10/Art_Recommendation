# ArtEmis: 미술 작품 관계 분석 및 추천 시스템

## 📌 프로젝트 개요
이 프로젝트는 **ArtEmis** 데이터를 활용하여 미술 작품 간의 관계를 분석하고, 감정적 또는 주제적으로 유사한 작품들을 추천하는 시스템을 구축하는 것을 목표로 합니다. 미술 작품과 작가 간의 관계를 그래프 마이닝 기법을 통해 탐구하며, 사용자에게 감정적 반응이나 스타일에 맞는 작품을 추천합니다.

---

## 📊 데이터 설명

### ArtEmis 데이터셋
**ArtEmis** 데이터셋은 454,684개의 감정적 주석을 포함하며, 다음과 같은 열을 포함하고 있습니다:
- **art_style**: 작품의 스타일 (예: 추상화, 인상파 등)
- **painting**: 작품 이름 또는 ID
- **emotion**: 감정 반응 (9개의 감정 중 하나)
- **utterance**: 감정을 선택한 이유에 대한 설명
- **repetition**: 작품에 대해 의견을 제시한 주석자의 수 (평균 5.68명)

### OLA 데이터셋 (객관적 언어)
**OLA** 데이터셋은 감정적 언급을 배제하고, 작품에 대한 객관적 설명을 포함합니다. 주요 열은:
- **art_style**: 작품 스타일
- **painting**: 작품 ID
- **utterance**: 객관적인 작품 설명

---

## 🔎 분석 방법
1. **데이터 전처리**: 데이터 정리 및 결측치 처리, 작품 ID 표준화
2. **그래프 구축**: 작품을 노드로, 공유된 특성(감정, 스타일 등)을 기반으로 엣지 생성
3. **그래프 시각화**: 
   - **grampml**: 그래프 데이터를 처리하고, 시각화할 수 있는 도구로 그래프 분석 수행
   - **Gephi**: 관계망을 시각화하여 작품 간의 상호 연관성 및 패턴을 탐구

---

## 🛠️ 설치 방법

1. 레포지토리 클론:
   ```bash
   git clone https://github.com/leeyubin10/artemis-artwork-recommendation.git
   cd artemis-artwork-recommendation
