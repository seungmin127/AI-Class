# DL_Classification_abalone
              precision    recall  f1-score   support

           0       0.85      0.77      0.81       307
           1       0.79      0.90      0.84       478
           2       0.57      0.24      0.33        51

    accuracy                           0.81       836
   macro avg       0.74      0.63      0.66       836
weighted avg       0.80      0.81      0.80       836
[[235  72   0]
 [ 40 429   9]
 [  0  39  12]]
 
해당 분류 모델은 전체적으로 안정적이게 학습이 되었다.

그러나 클래스별 상세 성능을 확인한 결과 Class2에 대한 precision과 recall 낮은 값으로 나와 해당 클래스를 제대로 분류하지 못하는 문제가 발생하였다.

이는 데이터 분포에서 Class2의 샘플 수가 상대적으로 너무 적어 불균형 문제가 발생한 것으로 판단된다.

# DL_Regression_abalone

<img width="823" height="815" alt="image" src="https://github.com/user-attachments/assets/484352f2-b2df-43f2-b858-4f91d4ccd243" />

MSE: 4.05, MAE: 1.41

해당 회귀 모델은 학습 과정에서 모델이 빠르게 패턴을 학습하여 안정적인 모습을 보였다.

실제값 vs 예측값 그래프에서도 전체적으로 대각선 근처에 분포하여 기본적인 예측은 잘 수행하였지만 큰 값을 작게 예측하는 현상이 발생하였다.

이는 큰 값의 데이터가 부족하여 학습이 충분히 이루어지지 않는 이유로 판단된다.
