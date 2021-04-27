# 1강
Intro. 딥러닝 시작하기

## Ch 01.
### Step1. 딥러닝이란?

1. DL은 인공지능이라는 거대한 학문의 일부
2. DL은 ML의 여러 기법 중 하나

### Step2. 딥러닝의 원리

1. ML의 정의
   - 주어진 데이터나 과거 용례를 통하여 문제에 대한 해결 성능을 최대화하는 것
2. Role of Statistics:
   - Inference from samples
3. Role of Computer Science:
   - 최적화 문제 해결
   - 추론을 위한 모델을 구성하고 평가
- 다시말하면, 사람이 쓴 글씨를 computation을 통해 디지털화된 글씨를 얻는 것
- 즉, 추상적인 정보를 확실한 정보로 변환
  
-머신러닝의 원리
![1-1](./img/1-1.gif)
-딥러닝의 원리
![1-2](./img/1-2.gif)

### Step3. 딥러닝이 주로 다루는 문제들

1. Association Rule Mining
   - 검색포탈 연관어 매칭
2. Supervised Learning
   - Classification: 문제 맞추기
   - Regression: 수식 문제
   - 문제가 있고 정답이 존재
3. Unsupervised Learning
   - Clustering
   - Feature Extraction
   - Dimensionality Reduction
   - 정답을 창조하지 않음
   - 문제에 있는 통계만을 이용하고 싶을 때
4. Reinforcement Learning



- Supervised Learning
  - 학습셋이 주어짐(문제&정답)
  - 학습셋은 정답이 Labelled 되어 있음
  - 주어진 학습셋을 근거로 학습
  - 새로운 데이터가 들어오면 정답을 예측
- Unsupervised Learning
  - 데이터가 주어짐(Unlabelled&Labelled)
  - 학습셋은 정답이 Labelled 되어 있거나 안되어 있거나
  - 주어진 데이터의 정보를 활용해서, 패턴을 추출하거나 관계를 구성
  - 명확하게 정해진 정답은 없음
- Reinforcement Learning
  - Unsupervised Learning의 일종
  - 정해진 데이터에 의해 학습되어지는 것은 아님
  - 변화는 상황에 대해 보상/벌점의 개념을 모델링
  - 모델의 행위에 맞게 일어나는 경험을 학습
  

## Ch 02.

### Step1. 딥러닝의 구조

노다가의 끝.
- 언제 계산을 멈출 수 있는가?
  - 무한한 h(x) 중 무엇이 좋은 함수인가
  - 찾는다면 어떻게 찾는가
- Idea
  - 나쁨/틀림(wrongness)를 정의
  - wrongness를 최소화 시키는 전략
  - cost/loss function을 통한 h(x)의 예측 y'와 주어진 학습셋의 y의 차이를 최소화 시키는 전략

### Step2. 비용 함수

![1-3](./img/1-3.gif)
최소화하는 전략

### Step3. 경사하강법

Idea
- 어떤 공간 임의의 위치에서 주어진 축에 대해 더 작은 위치로 내려가려면?
- 미분.

![1-4](./img/1-4.gif)
![1-5](./img/1-5.gif)