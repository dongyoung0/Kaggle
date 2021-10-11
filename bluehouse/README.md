# 청와대 청원 : 청원의 주제가 무엇일까?
https://dacon.io/competitions/open/235597/

- NLP 연습을 위해서 시도해보는 문제
- 일단 baseline 코드를 그대로 따라가보고, 추가로 여러가지 시도해 볼 예정

## 전처리
### Okt 
- stopwords = ['의','가','이','은','들','는','좀','잘','걍','과','도','를','으로','자','에','와','한','하다','을']
를 기준으로 나눔
- 코랩으로 작업하기 때문에 런타임이 초기화될 때마다 30분의 okt 변환 과정을 반복하기 싫음.
- okt로 변환한 결과를 train_okt.csv / test_okt.csv로 저장해두고 불러와서 사용

### Tokenizer
- tokenizer를 통해 text를 sequence로?

### 결측치
- train set에 'data'부분이 비어있는 결측이 8개 존재.
- 일단 결측치 제외한 39992개 데이터만 사용해보기로 함.
- y_train 생성시에 결측부분 제외하고 생성

## 모델링
### LSTM
- baseline 코드 그대로~

## Submission
|날짜|파일명|점수|전처리|모델|내용|
|-----|---|---|------|---|------|
|21/10/11|Sub1.csv|0|Okt|LSTM| 제출 파일 실수로 인해서 0점
|21/10/11|Sub2.csv|**0.8376**|Okt|LSTM|baseline 코드 그대로 따라가서 제출. </br> 결과 제출시에 tensorflow 버전 문제인지, model.predict_classes가 작동을 안함. </br> y_pred = model.predict(X_test)로 (5000,3)의 array를 구한 후, argmax를 사용해서 각 행마다 값이 가장 큰 인덱스를 반환.
