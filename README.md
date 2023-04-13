### Hi there 👋
### Name : Do Sungjin
### 
### --------------------

# Blackcoal price

## 유연탄 가격의 trend 예측

<aside>
💡 유연탄 가격 trend 예측을 통해 남부발전과 같은 해당 기업의 의사결정시  정보를 제공하여 현실적인 이득을 안겨다 준다.

</aside>

---

### 유연탄 프로젝트 정리 및 일정 링크     기존 유연탄 프로젝트 -마인즈 앤 컴퍼니

[](https://www.notion.so/42b6686cdff44bdbbf2c0ac04eed07e7?v=5e4f786153294a9ca23c4db1a4fa9774)

---

[](https://mnc.ai/?p=11)

---

[Project_MLOPs](https://www.notion.so/Project_MLOPs-9b5e5fcda61f4e9f9f2b2cc1987b2a1f)

# 🕋B**lackcoal_price**

# ❓**Why is forecasting important?**

- There has always been a demand for price prediction. From a company's point of view, inventory management of raw materials is the key to cost control. In this way, from the raw material market, which is the basis of business, the production volume that determines the production of goods, that is, the demand itself, is also required. If you derive insight into the market while modeling, and go through the process of developing the model through the derived information, prediction can give a lot of information to business management, not just prediction.

## 📅Period

- For 2022-05-23 ~ 2022-07-20

# **Purpose**

When the firm buy ‘Blackcoal’, we want to give information about price. Furthermore we want the stock is managed effectively

![https://user-images.githubusercontent.com/100894816/172108400-d6088db0-4ace-48b2-9f9c-8aa6be37c200.png](https://user-images.githubusercontent.com/100894816/172108400-d6088db0-4ace-48b2-9f9c-8aa6be37c200.png)

# **Procedure**

Fist of all, there is a model about price. And then we do backtesting for profit.

1. Reference
2. Data crawling
3. EDA
4. Modeling
5. Evaluation
6. Back testing - plan

# **EDA**

![https://user-images.githubusercontent.com/100894816/174795217-06686582-9984-44d4-a4f7-37d72a2b76e3.png](https://user-images.githubusercontent.com/100894816/174795217-06686582-9984-44d4-a4f7-37d72a2b76e3.png)

![https://user-images.githubusercontent.com/100894816/174795239-26ad8397-61fb-4c39-ba2a-bc95bd44942f.png](https://user-images.githubusercontent.com/100894816/174795239-26ad8397-61fb-4c39-ba2a-bc95bd44942f.png)

![https://user-images.githubusercontent.com/100894816/174795264-a07d818e-4b73-41ba-925a-6b7b243c3c25.png](https://user-images.githubusercontent.com/100894816/174795264-a07d818e-4b73-41ba-925a-6b7b243c3c25.png)

- Advance to decline ratio
- Simple moving Average

```jsx
In time series prediction, correlation is not important. However, we used it as a reference.
```

![https://user-images.githubusercontent.com/100894816/174796891-9fd5f554-c77c-4b92-9e87-fde638bd3536.png](https://user-images.githubusercontent.com/100894816/174796891-9fd5f554-c77c-4b92-9e87-fde638bd3536.png)

 상관관계 분석, 민감도 분석, 토네이도 차트와 스파이더 차트, 다중공선성 분석, 부트스트랩핑, 집락 세분화, 데이터진단, 분포조정, 분포확률(PDF, CDF, ICDF), 가설검정, 오버레이 차트, 통계 분석

[변수영향력(토네이도 차트)개념 ](https://www.notion.so/a59c4e1b89304776877181103c5808f7)

- 상관관계 분석

```
우리는 종종 어떤 두 사건 간의 연관성을 분석해야 할 경우가 많습니다.둘 또는 그 이상의 변수들이 서로 관련성을 가지고 변화할 때 그 관계를 분석해야 하는데,가장 잘 알려진 방법 중 하나가상관분석과회귀분석 입니다.예를 들어, GDP와 기대수명 간의 관계, 키와 몸무게 간의 관계를 보자면,각각 두 변수 간의 선형적 관계를 상관(Correlation)이라고 하며, 이러한 관계에 대한 분석을 상관분석(correlation analysis)라고 합니다.
```

먼저 상관계수를 파악하기 전에 산점도를 그려 두 변수 간에 관련성을 시각적으로 파악하겠습니다.

[산점도 결과 ](https://www.notion.so/f7d955c5de3f4820a94fe7192ce39e94)

공분산 및 상관계수

[
Corrcoef ](https://www.notion.so/Corrcoef-0c4fe9aff61f47aa8828f2a195914ab0)

[covarian/correlation/p-value ](https://www.notion.so/covarian-correlation-p-value-1bc3a7f4338e4e9cbe36cfe65f9152fd)

[linear regression](https://www.notion.so/linear-regression-ef985825e6f94fa991c9a9e2f9ad4065)

[Graph with ‘Coal’](https://www.notion.so/Graph-with-Coal-62ae8d33fbac466d88df2e5a8b6bfda7)

# **Modeling**

1. Whole

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/14a36523-5aa1-4a73-b0a0-6d19c3edabb8/Untitled.png)

1. Task 1
: X-Feature 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a3081094-2070-4459-9d8a-3b4004bd12f7/Untitled.png)

1. Task 2
: y 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/272a2cab-0ecd-4417-a61a-1a0d305cbd3c/Untitled.png)

Result 

Date : 2018-10-25 (3 month)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3712eeab-8775-4cd5-be72-b67729bbbd34/Untitled.png)

Date : 2019-02-04 (3 month)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1665e143-65fa-496f-8eab-3e5d503135ff/Untitled.png)

Date : 2019-01-01 (3 month)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/981b593d-ebdb-4b83-8fe0-590aaa1699d5/Untitled.png)

Date : 2019-04-01 (3 month)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a49161a7-8aed-4ed0-935b-b1ac8609a922/Untitled.png)

Comparing profit with 남부발전

Date : 2019-01-01~2019-04-01

Buying point :

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80cc2d9f-95b6-497b-9ea1-5418ed8a3b73/Untitled.png)

- Profit

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/160cd343-4da5-4790-9e4e-ac84e8a33970/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9db090d4-098f-4801-a83b-3a8258d80c09/Untitled.png)

## For Time Series Forcasting

-First of all, we have to know all about Models for Time Series. **This is our trial and error and procedure.**

1. arima
- one-to
- check the data is stationary
- (Make ACF, PACF graphs)
- (Make Differenced Data(Stationary)
- seasonal decomposition

[Result page - Arima](https://www.notion.so/Result-page-Arima-3485b841894a44229d0755bfabf7ff8d)

1. prophet one-to
- Basic model Prophet make well if the data has a Seanality & Trend. Also, if there is a event that we can't expect we can set the event as we know. But Blackcoal is a raw materials product that is effected by spply and demand. So I expect the result is poor as long as i do the prophet on blackcoal only. As we know, Prophet is good at Supply, Demand and Economic indicators like USD/AUD, S&P. So we will use the prophet as a feature that can predict the blackcoal price.
- Equation of Prophet

[💼**Our file**](https://www.notion.so/Our-file-2ac42bd92374445a9074cf11f971e4d0)

1. Prophet + XGBoost
- many-to-many
- with prophet prediction we test the XGBoost Model, it works well.

[ Result Page - Prophet +XGBoost](https://www.notion.so/Result-Page-Prophet-XGBoost-062a9534fb9f45f29e99f7411bc794b4)

1. XGBoost(AR+Recursive)
- X feature make

[Result Page - XGBoost(AR + Recursive)](https://www.notion.so/Result-Page-XGBoost-AR-Recursive-f0a6982c358144c2b68cc889bcf41211)

1. lstm many-to-many
2. 1D convolution many-to-many

## 💼Reference

---

[**An Analysis on the Price Predictability of Steam Coal**](https://www.notion.so/An-Analysis-on-the-Price-Predictability-of-Steam-Coal-845aee8c84984963ba96b8dc72a9ab7f)

    **Korean Energy Economic Review** v.5 no.2 , 2006

[**Development of a Forecast Model for Thermal Coal Price**](https://www.notion.so/Development-of-a-Forecast-Model-for-Thermal-Coal-Price-7caa511d51d4440c9c5867a9a7d08303)

 **Journal of service research and studies** v.6 no.4 , 2016년, pp.75 - 85

[**Comparison of Coal Procurement Strategies Using Forecasting Models**](https://www.notion.so/Comparison-of-Coal-Procurement-Strategies-Using-Forecasting-Models-5464e6c41c724cdda6eb57e5e10437eb)

**자원·환경경제연구 = Environmental and resource economics review** v.16 no.2 , 2007년, pp.337 - 361

[**Oil Price Forecasting Based on Machine Learning Techniques**](https://www.notion.so/Oil-Price-Forecasting-Based-on-Machine-Learning-Techniques-802779dbe10640b8a703a9f6308e6d8d)

**대한산업공학회지 = Journal of Korean institute of industrial engineers** v.37 no.1 , 2011년, pp.64 - 73

[**Stock Price Prediction Based on Time Series Network**](https://www.notion.so/Stock-Price-Prediction-Based-on-Time-Series-Network-dbc6dd8a458048f7b0a579b48056689b)

**經營 科學 = Korean management science review** v.28 no.1 , 2011년, pp.53 - 60

**원자재 가격예측 및 구매 의사결정지원 시스템 개발**

**📔Experimental Study on Long-Term Prediction of Rebar Price Using Deep Learning Recursive Prediction Meothod
 
📔Experimental Study on the Expansion of the Short-term Prediction Range of Rebar Prices Using Deep Learning
 
📔Long-term Settlement Prediction of Railway Concrete Track Based on RNN**

[JPX Tokyo Stock Exchange Prediction](https://www.notion.so/JPX-Tokyo-Stock-Exchange-Prediction-e1fa755adea74b0580a12ba1fdc0bf3a)

[Lendingclub data : Default prediction](https://www.notion.so/Lendingclub-data-Default-prediction-c87f261478de481a8d42c991bce2fa0c)

[Kore 2022](https://www.notion.so/Kore-2022-c9d3e6634e0b4051af5b59c3f5c68283)

[Mlflow(MLOPs)](https://www.notion.so/Mlflow-MLOPs-d315cc1d324943abbf11ce7216f3f4d4)

[Cycle GAN, styleGAN](https://www.notion.so/Cycle-GAN-styleGAN-1ae80411649944e9bb7c40abb5e49059)

[Apple sugar grade prediction](https://www.notion.so/Apple-sugar-grade-prediction-3fd90b37b5db4f9c8f8061f4ee49bf92)

[Feedback Prize](https://www.notion.so/Feedback-Prize-abceb25b66074d0a99ac71cb8a20f15d)

[**제주도 도로 교통량 예측 AI 경진대회**](https://www.notion.so/AI-03f764f1c386425faccbc56dc36c8482)

[****American Express - 기본 예측****](https://www.notion.so/American-Express-e17c4240227a4da1b9fe64a6c933a9b5)

[Traffic prediction](https://www.notion.so/Traffic-prediction-77aac1da508244a890d1aa340a344523)

<!--
**DoSungjin/Dosungjin** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
