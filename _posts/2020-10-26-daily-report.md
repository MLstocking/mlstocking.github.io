---
layout: post
title:  "2020-10-26 데일리 리포트"
date:   2020-10-26 11:50:40
categories: daily_report
---

## 모델 예측 결과
예상 수익금 : 14,420,830 원 
<center><img src="/assets/20201029_225006_epoch_summary_1.png" width="400" height="400" ></center>

>
- ENV
    - 모델이 학습하는 환경을 의미
    - 여기서는 종목(삼성전자)의 실제 일봉 차트
- Agent
    - 에이전트의 매수을 빨간색, 매도을 파란색 배경으로 시각화 
    - 보유 주식 수를 라인차트로 시각화
- V
    - 에이전트의 행동에 대한 예측된 행동 가치를 라인차트로 시각화
    - 매수는 빨간색, 매도는 파란색으로 표기
    - 배경은 예측된 행동 가치 중 가장 높은 행동에 대한 색으로 시각화 
- P
    - 각 행동에 대한 정책 신경망의 출력을 시각화
    - 매수는 빨간색, 매도는 파란색으로 표기
    - 빨간선과 파란선 중 높이 있는 선의 행동을 수행함
- PV
    - 에이전트의 행동에 따른 자본금을 라인차트로 시각화
    - 초기 자본금은 가로선으로 표기

[모델에 대한 설명 자세한 내용은 여기를 참조하세요.][model_description]

[model_description]:http://https://mlstocking.github.io/model_description/2020/10/26/model_description.html