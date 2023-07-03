# 소아 Chest X-Ray 영상 데이터 활용 폐렴 예측 모델

소아 Chest X-Ray 영상 데이터를 활용하여 정상군과 세균성 폐렴 및 바이러스성 폐렴으로 분류하는 예측 모델 개발.

우선 이미지 데이터에 폐를 가리는 이물질이 있을 경우, 해당 이미지는 사용하지 않았다.

VGGNet과 ResNet을 비교 분석하려고 하였으나, colab환경에서 ResNet이 돌아가지 않아 사용은 하지 못하였다.

grad-CAM은 GAP(glovbal average pooling)을 사용하지 않은, gradient를 이용한 CAM을 사용하였으며
fully-connected network에서의 가중치들의 미분값을 이용하여 마지막으로 시행한 convolution layer에 곱해준 값을
히트맵으로 나타내어 원본 이미지 위로 나타내었다.
