## 이진분류란
- 입력 데이터를 두 개의 가능한 클래스 중 하나로 분류하는 작업

### 1. 기본 개념
출력이 두 가지 클래스 중 하나입니다 (예: 양성/음성, 스팸/정상, 1/0).
주로 확률로 표현되며, 임계값(보통 0.5)을 기준으로 클래스를 결정합니다.

### 2. 네트워크 구조
- 입력층: 특징 수에 따른 노드
- 은닉층: 하나 이상의 층, 각 층에 여러 노드
- 출력층: 단일 노드 (0~1 사이의 값 출력)

### 3. 활성화 함수
- 은닉층: ReLU, tanh 등
- 출력층: Sigmoid (0~1 사이의 확률값 출력)

### 4. 손실 함수
- 주로 Binary Cross-Entropy 사용
- Loss = -[y log(p) + (1-y) log(1-p)]
(y: 실제 레이블, p: 예측 확률)

### 5. 최적화 알고리즘
- Adam, RMSprop, SGD 등

### 6. 평가 지표
- 정확도(Accuracy), 정밀도(Precision), 재현율(Recall)
- F1 점수, ROC 곡선, AUC 등

### 7. 과적합 방지 기법:
- 드롭아웃(Dropout)
- L1/L2 정규화
- 데이터 증강(Data Augmentation)

### 8. 불균형 데이터 처리:
- 클래스 가중치 조정
- 오버샘플링/언더샘플링
- SMOTE 등의 기법 사용

### 9. 응용 분야:
- 스팸 메일 탐지
- 의료 진단 (질병 유무)
- 금융 사기 탐지
- 감성 분석 (긍정/부정)

이진 분류는 많은 실제 문제에 적용될 수 있는 기본적이면서도 중요한 작업입니다. 딥러닝을 통해 복잡한 특징을 자동으로 학습할 수 있어, 전통적인 방법보다 더 높은 성능을 낼 수 있습니다.

#### [▶︎ 실습](https://github.com/hwd0ng/ML_KNN/blob/main/KNN_%E1%84%8B%E1%85%A1%E1%86%AF%E1%84%80%E1%85%A9%E1%84%85%E1%85%B5%E1%84%8C%E1%85%B3%E1%86%B7%20%E1%84%87%E1%85%AE%E1%86%AB%E1%84%89%E1%85%A5%E1%86%A8.ipynb)
