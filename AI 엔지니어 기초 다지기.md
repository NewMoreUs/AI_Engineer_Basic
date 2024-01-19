# 정형 데이터

## 정형 데이터 정의
정형 데이터
- 액셀 파일 형식이나 관계형 데이터베이스의 테이블에 담을 수 있는 데이터로 행(row)과 열(column)으로 표현 가능한 데이터. 하나의 행은 데이터 인스턴스를 나타내고, 각 열은 데이터의 피처를 나타냄

비정형 데이터
- 이미지, 비디오, 음성, 자연어 등의 정제되지 않은 데이터
- 정형 데이터와 달리 틀이 없고, 테이블 형식으로 표시할 수 없음
- 하나의 데이터 인스턴스로 표현하기 위해 흑백의 경우 2차원, 컬러의 경우 3차원이 필요함

## 정형 데이터의 중요성
- 범용적인 데이터: 사람, 기업, 현상, 사회의 많은 부분들이 정형데이터로 기록됨
- 기업에서 기본적으로 사용되는 데이터, 분야를 막론하고 많은 데이터가 정형데이터로 존재

정형 데이터의 분석 능력이란?
- 데이터에 대한 상상력과 통찰력
- 다양한 경험을 통해 데이터에 국한 되지 않고 범용적으로 쓰일 수 있는 능력

# 평가지표 이해
분류 (Classification)
- 예측해야 할 대상의 개수가 정해져 있는 문제
- 예) 이미지에서 개, 고양이 분류, 신용 카드 거래가 사기 거래인지 정상 거래인지 분류 등

회귀 (Regression)
- 예측해야 할 대상이 연속적인 숫자인 문제
- 예) 일기 예보에서 내일의 기온 예측, 주어진 데이터에서 집값 예측

평가지표 (Evaluation Metric)
- 분류, 회귀 머신러닝 문제의 성능을 평가할 지표


분류 문제에 대한 평가 지표 - Confusion Matrix

| Confusion Matrix | 예측 |  |
| ---- | ---- | ---- |
|  | Negative | Positive |
| 실제 | TN (True Negative) | FP (False Positive) |
|  | FN (False Negative) | TP (True Positive) |
- TP: model-P, 정답-P
- TN: model-N, 정답-N
- FP: model-N, 정답-P
- FN: model-P, 정답-N

Accuracy
1. Accuracy: (TP + TN) / (TP + TN + FP + FN)
2. precision: TP / (TP + FP)
3. Recall: TP / (TP + FN)

ROC (Receiver operating characteristic)
- 수신자 조작 특성
- True Positive Ratio: $TP/TP+FN$
- False Positive Ratio: $FP/FP+TN$

AUC (Area Under Curve)
- ROC 곡선의 면적을 표시한 것으로 0과 1 사이의 값을 가짐
- 1에 가까울수록 모델이 잘 예측하는 것을 뜻함













