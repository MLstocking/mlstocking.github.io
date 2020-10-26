---
layout: post
title:  "주가 예측 모델 설명"
date:   2020-10-26 11:50:40
categories: model_description
---


## 1. 학습 알고리즘

    - A2C(Advantage Actor Critic)
    - 가치 신경망 : LSTM(Long Short-Term Memory)
    - 정책 신경망 : LSTM(Long Short-Term Memory)
    
## 2. 학습 데이터 기간

    - 시작 일자 : 2016-01-01
    - 종료 일자 : 2018-12-31

## 3. 학습 피쳐

    - OHLCV(시가, 고가, 저가, 종가, 거래량)
    - 전일 종가 대비 당일 시가 비율
    - 당일 종가 대비 당일 고가 비율
    - 당일 종가 대비 당일 저가 비율
    - 당일 종가 대비 전일 종가 비율
    - 전일 거래량 대비 당일 거래량 비율
    - (5, 10, 20, 60, 120)일 평균 종가 대비 당일 종가 비율
    - (5, 10, 20, 60, 120)일 평균 거래량 대비 당일 거래량 비율

## 4. 하이퍼 파라미터

|하이퍼 파라미터|값|
|---------------------------------------------|----------|
|학습률(learning rate)|0.9|
|할인 요인(discount factor)|0.9|
|에포크(epoch)|1000|
|지연 보상 임계치(delayed reward threshold)|0.05|
|시작 탐험률(epsilon)|1|
|초기 자본금|10,000,000원|


<img src="https://github.com/favicon.ico" width="100">
    






[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help