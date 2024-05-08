# -DACON-Bird_image_classification

# <프로젝트를 하면서 배운점>

- 데이터 전처리 (라벨 인코딩 vs 원핫 인코딩)

- 라벨 인코딩 : 라벨들을 정수형 변수로 변환.

                선형회귀 모델에 사용하면 좋지 않음! -> 숫자간의 크고 작음이 영향을 줄 수 있음

                 트리형 모델은 사용 괜찮(ex) 랜덤포레스트

                  순서가 있는 데이터형일 때 효과적(ex) 직급
                  

  -원핫인코딩 : 라벨들을 이진 변수로 변환.

                2차원으로 변환됨 --> 따라서 나중에 백터화 시켜줘야함

                종류가 너무나도 많을 경우, overfitting의 위험이 있음

                Softmax함수를 사용할 경우 좋다함 + 데이터간 순서X + 데이터양이 적을 때

                판다스(get_dummies를 이용 & OneHotDecoder(사이킷런) 사용가능

                사이킷런을 사용할 경우, 희소행렬로 반환(DataLoader 사용 불가) , 데이터형 바꿔줘야함..

- CNNModel (Lesnet vs Densenet)

- Lesnet : Residual learning(잔여학습 개념 도입)

            잔여학습이란 -> 이전 결과를 추가해서 학습시킴
-Densenet : Lesnet의 장점을 가져옴 (잔여학습)
             
             차이점->  모든 레이어값을 계속해서 concat해준다는 점.

  

  
