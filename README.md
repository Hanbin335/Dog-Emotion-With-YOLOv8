CNN과 YOLOv8을 활용한 실시간 강아지 이모션 인식 시스템
---
![image](https://github.com/user-attachments/assets/49c74c58-be4c-40d3-a106-49e434c9b66c)


프로젝트 소개
---
CNN을 활용해 강아지 감정을 분류하고, YOLOv8을 활용해 강아지 탐지 성능을 최적화하여 실시간으로 변화하는 강아지의 감정 상태를 'Happy', 'Angry', 'Relaxed', 'Sad' 4가지 범주로 실시간 감정 분석 시스템을 구현한 프로젝트

프로젝트 전체 과정 및 YOLOv8을 활용한 이유
---
![image](https://github.com/user-attachments/assets/742c14ae-bf77-4bb6-96d7-eb132916f3b1)

주요 기능
---
● 데이터 전처리 및 라벨링 : 이미지 파일에서 레이블을 자동으로 추출하고, 이미지를 크기 조정하여 훈련 데이터셋을 생성

● 모델 구축 및 훈련 : CNN 기반의 딥러닝 모델을 정의하고, 이미지 데이터를 넘파이 배열 형태로 훈련하여 강아지 감정을 분류하는 모델 생성

● 모델 평가 : Matplotlib을 사용하여 학습 과정에서의 정확도, 손실 및 혼동 행렬(Confusion Matrix) 시각화

● 이미지 예측 : 새 이미지를 로드하고 전처리하여 훈련된 모델로 감정 예측

● 비디오 스트리밍에서 강아지 감정 감지 : YOLOv8을 사용하여 비디오에서 강아지를 감지하고, 감정 예측 결과를 실시간으로 표시

● 결과 시각화 : 예측된 감정 클래스를 비디오 프레임에 오버레이하여 사용자에게 표시

개발 환경
--
● Google Colab : 클라우드 기반 Python 개발 환경으로 , GPU를 사용한 딥러닝 모델 학습에 사용

● Python : 주요 프로그래밍 언어로 사용

● Google Drive : 데이터를 저장하고 불러오는 파일 시스템으로 사용

● VSCode : 동영상 재생 기능이 지원되지 않는 Google Colab 대신, 결과 시각화부터는 VSCode 사용

기술 스택
--
● Tensorflow & Keras : 딥러닝 모델 구축 및 학습을 위해 사용

● OpenCV : 이미지 전처리 및 동영상 스트리밍 기능 구현하는 데 사용

● Numpy : 배열 및 행렬 연산을 수행하며, 이미지 데이터를 넘파이 배열 형태로 변환하는 데 사용

● Scikit-learn : 학습 데이터와 검증 데이터를 분리하는 데 사용 (train_test_split 함수)

● Matplotlib : 학습 과정에서의 정확도, 손실 및 혼동 행렬(Confusion Matrix)그래프 시각화

● YOLOv8 : 실시간 객체 탐지를 위한 모델로, 개를 감지하고 감정 분석을 수행하는 데 사용

성능 평가
---
![image](https://github.com/user-attachments/assets/7d5e614b-fe32-43a7-b5ef-a088e24a7520)

● 훈련, 검증 데이터에서 정확도가 99%, 99.7% 손실이  3%, 0.3%로 안정적으로 높은 성능을 확인

● Epoch 150 까지의 훈련을 통해 모델이 최적의 파라미터에 도달했으며, Confusion Matrix 결과 모든 클래스를 정확하게 예측한 것으로 확인

실시간 강아지 감정 분석
---
![image](https://github.com/user-attachments/assets/f189bfd3-1f9a-4de1-ba69-2e6914b691d7)

