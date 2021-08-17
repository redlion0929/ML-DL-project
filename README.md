# ML-DL-project
--------

## NLP
### 1. 스팸 분류기
> 데이터는 텍스트+label(스팸인지 아닌지)로 구성되어있다. 
> TfidfVectorizer와 MultinomialNB를 Pipeline을 이용하여 전처리와 학습을 한 번에 수행하였다. 
> 교차검증으로 인해 정확도가 높았다.
### 2. 감정 분석기
> review에서 'review_text'라는 태그에 포함된 내용들을 BeautifulSoup를 이용하여 추출한다. 
> 이 text를 전처리한 후 LogisticRegression모델에 적용하여, review가 들어왔을때 그 text에 담긴 감정을 추측할 수 있게끔 모델을 학습시켰다.
### 3. 잠재적 감정 분석기
> 책의 제목들을 받는다. 이후 text를 전처리한 후 dimensionality reduction(차원 축소)를 하여 데이터를 2차원으로 변형한다. 
> 만들어진 2차원 데이터를 이용하여 비지도학습을 수행한다.
--------

## 의료 데이터를 활용한 ML
### 1. 헌혈 분석
> 헌혈로 받은 피 중에서 실제로 사용할 수 있는 피는 많지않다. 헌혈했던 사람들에 대한 데이터를 바탕으로 사용할 수 있는 피를 가진 사람들을 식별하는 모델을 구현하였다.
> Logistic Regression, SVC, RandomForestClassifier, Decision Tree Classifier, MLP classifier를 이용하여 모델을 구축하였다. (Classification)
### 2. DNA 분류
> 염기서열을 분석하여 인간과 침팬지에게 공통으로 나타는 7가지 단백질을 각 염기서열을 바탕으로 분류한다. 
> Decision Tree Classifier, RandomForest Classifier, xgboost, Multinomial NB를 이용하여 모델을 구축하였다. (Classification)
### 3. 척추후만증 질병 분류 
> 수술 후에 척추후만증에 걸린 사람과 그렇지 않은 사람들에 대한 데이터가 주어진다. 
> 데이터간의 상관관계를 파악하고 이를 바탕으로 데이터를 전처리하였다.
> DecisionTreeClassifier를 이용하여 모델을 구축하였다. (Classification)
### 4. 응급실 사망률 예측
> 응급실에서 사망한 사람과 그렇지 않은 사람들에 대한 데이터가 주어진다. 
> 데이터간의 상관관계를 파악하고 이를 바탕으로 데이터를 전처리하였다.
> ANN를 이용하여 모델을 구축하였다. 
### 5. 자살률 추세 분석
> 1985년부터 자살한 사람들에 대한 정보가 담긴 데이터가 주어진다.
> 그래프를 그려 자살률 추이, 각 변수와 자살률 사이의 관계를 파악했다.
> RandomForestRegressor, DecisionTreeRegressor, LinearRegression, SVR를 이용하여 모델을 구축했다. (Regression)
-------

## kaggle
### 1. NLP - Getting Start
> 재난이 발생하면 사람들은 트위터에 관련 글을 올리고 전세계 사람들은 이러한 글을 바탕으로 다른 지역에 재난이 발생했다는 것을 추측할 수 있다.
> 하지만 재난이 발생하지 않았는데도 이러한 글을 올려 사람들에게 혼동을 주는 경우도 있다. 
> 트위터에 재난 발생 올라온 글을 보고 재난이 사실인지 아닌지 구분해주는 모델을 pipeline을 이용하여 구축하였다. 
### 2. 타이타닉 데이터 분석
> 타이타닉 탑승자 명단과 사망 유무가 담긴 데이터를 분석해보았다. 
> 분석 후 AdaBoostClassifier를 이용하여 모델을 구축했다. (Classification)
--------

## 그 외
### 1. CNN을 이용한 이미지 분류
> cifar10에서 10가지 class에 해당하는 60000개의 이미지를 받아온다. 
> 이후 Convolution, Pooling, Dropout, flatten의 과정에 Dense layer를 추가하여 CNN모델을 구축한다.
> 이 모델에 이미지들을 학습시켜 새로운 이미지가 주어졌을 때 그 것이 어떤 class에 속하는지 구분할 수 있다.
### 2. ANN을 이용한 자동차 구매 가격 예측 모델
> 고객에 대한 정보(나라, 성별, 카드 부채, 순자산 등)가 담긴 데이터가 주어진다.
> 고객이 자동차를 얼마에 구매했는지와 여러 변수 사이의 관계를 파악한 후 ANN을 이용한 모델을 학습시킨다. 
> 이후 새로운 고객에 대한 정보가 주어지면 그 사람이 자동차를 얼마에 구매할지를 예측할 수 있다. 
--------
## 수강 인증서

> + Start OpenCV with Python : Real-time Processing with Webcam
> + Machine Learning Practical : Real world Projects in Healthcare

-------
## 총평
> 어렵게만 생각했던 ML, DL에 대해 좀 더 직관적으로 이해할 수 있었던 시간이었다. 
> 날 것의 데이터를 컴퓨터가 알아볼 수 있게끔 처리하여 적절한 모델에 대입하면 신뢰할 수 있을 만한 결과를 가져온다는 사실이 흥미로웠다.
> 유용하게 사용될 수 있는 함수를 배웠고, 언어 처리에 대한 여러 함수를 제공하는 nltk에 대해 공부했다.
> 이제 첫 걸음을 뗀 상태라 아직 갈 길이 멀다. 
> tensorflow, keras등 ML에 필요한 다양한 라이브러리를 공부해봐야겠다.
