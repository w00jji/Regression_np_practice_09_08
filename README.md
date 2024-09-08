# Regression_np_practice_09_07

## 넘파이로 선형회귀 & 오차역전파
- 절차
  1) feature , Y 값 입력
  2) mse계산을 위한 feature 수
  3) 파라미터 초기화 w,b 0으로 초기화
  4) 경사하강법을 위한 학습률 , 학습 횟수 선정
  5) MSE 계산
  6) 기울기 계산
  7) 경사하강법 수행

### 사이킷런에서 제공하는 캘리포니아 주택 가격 예측
- 절차
   1) feature , Y 값 입력
   2) train_test_split (X_train, X_valid ,y_train, y_valid)
   3) 데이터 정규화
   4) mse계산을 위한 feature 수
   5) 파라미터 초기화 w,b 0으로 초기화
   6) 경사하강법을 위한 학습률 , 학습 횟수 선정
   7) MSE 계산
   8) 기울기 계산
   9) 경사하강법 수행

### wine.data 선형회귀 , alcohol 도수 예측
- 절차
   1) feature , Y 값 입력
   2) train_test_split (X_train, X_valid ,y_train, y_valid)
   3) 데이터 정규화
   4) mse계산을 위한 feature 수
   5) 파라미터 초기화 w,b 0으로 초기화
   6) 경사하강법을 위한 학습률 , 학습 횟수 선정
   7) MSE 계산
   8) 기울기 계산
   9) 경사하강법 수행
 
 느낀점 
 - StandardScaler는 각 특성(feature)이 2차원 배열로 주어져야 제대로 작동합니다.
    fit_transform과 transform 메서드는 2차원 배열을 입력으로 받아야 합니다.

- 그러나 X는 1차원 배열로 되어 있으므로, reshape(-1, 1)을 사용하여 2차원 배열로 변환한 후 정규화를 수행합니다. 이후, flatten() 메서드를 사용하여 다시 1차원 배열로 변환합니다.

- 1차원 배열로 다시 변환하는 이유 정규화 작업 후에는 결과를 다시 1차원 배열로 변환하는 이유는 원래 데이터의 형태로 복원하기 위해서입니다.


- 기울기에대한 w,b의 편미분 -> 경사하강법을 위해 사용함
  - 기울기 w 편미분
  
  ![image](https://github.com/user-attachments/assets/bfd083b8-67c3-463a-ac6d-f43161d59281)

  - 기울기 b 편미분
  
  ![image](https://github.com/user-attachments/assets/cf22ea25-cc52-441b-ac42-7fb9e812ef7c)


  
  
  
 
