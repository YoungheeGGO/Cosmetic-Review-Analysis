
- Period : Mar.20.2021 ~ May.30.2021

## Why did I analyze the data?
- Price competition is intensifying due to the rapid increase in various new brands, direct management stores, and franchises. -> Deteriorating profitability of cosmetic manufacturers
  - (ref: *Industrial Trends Report,* Cosmetics Industry Trends, and K-Beauty Global Competitiveness Analysis)
- The cosmetics market is attempting to apply the latest trend analysis techniques using big data such as SNS data.
  - (ref: 2018 Global Cosmetics Market Trend Analysis Seminar)
- Asia's share of skin care products is about 41%, which is overwhelmingly competitive.
  - (ref: Case analysis of brand concept development through big data analysis of cosmetics companies, Jumin Lee, Jounghae Bang)
- So, I decided to understand consumption trends through a review analysis of Skin Care's flagship product "Hand Cream."

## Analysis Process
**1. Crawling**
- I had web crawling the website that exists revies about cosmetics.
- There was so many types of cosmetics, I had narrowed down the analysis object to "Hand cream".
- And There was ranking about handcream sales, I had crawl just high (ranking 1\~3), middle (ranking 50\~52), bottom rank(ranking 98\~100).
- Also, The user information about age, gender, written date, skin type(dry, oily, sensitive, combination) were crawled. 

**2. EDA**
- I made the word clouds per its reviewr's age, gender, skin type with the review text.
- Word Cloud of 20's Female who has dry skin 
<img src="https://user-images.githubusercontent.com/102137580/160996581-9ce11c26-2d42-476e-b778-1a0a57b8d566.png" width="500" height="300">

- Word Cloud of  30's Male who has combination skin 
<img src="https://user-images.githubusercontent.com/102137580/160998036-8a6e8de1-45b3-4638-812d-b50dc798853f.png" width="500" height="300">

- Except for general word like *Hand, Cream, Product*, there was a common word not regarding age, gender, skin type : *Absorption, Price, Scent, Moisturizing*


**3. Word2vec**
- blah~~

**4. Conclusion & Significance**


## 느낀 점
- 원래 학과 수업의 일환으로 시작되었지만 어쩌다 보니 규모가 커지게 되었고 실제 데이터 분석이 기업에서 어떻게 쓰일 수 있을 것인지를 생각할 수 있는 기회가 되었다.
- 분석가의 관점뿐 만이 아니라 CEO의 관점에서 데이터 분석을 바라보는 것을 생각해보았다.
- 실제 회사에서 데이터 분석이 어떻게 쓰이는 지 경험해보고, 단순히 분석에서 끝나는 것이 아니라 분석 결과를 비즈니스 모델로 확장시킬 수 있는 지를 생각해 보았다.


- 팀원이나 다른 사람들 없이 나 혼자 진행했던 첫 플젝! 그래서 그런지 몰라도 삽질을 굉장히 많이 했다...! 너무너무 힘들었다.
- 이번 프로젝트를 통해서 내가 뭘 좋아하는지, 어떤 데이터에 흥미있어 하는지를 좀 더 알아본것 같다.


- 딥러닝을 사용한 프로젝트를 통해 도출된 결론을 가지고 남들을 설득시키는 것이 어렵다는 것을 알았다.
- 정량적 분석 뿐 만이 아니라 도메인 지식을 활용한 정성적 분석도 필요하다는 것을 알았다.

- 딥러닝에서 중요한 hidden layer (은닉층) 때문에 나온 블랙박스라는 딥러닝의 한계점 때문에 다들 딥러닝을 꺼려했다.

> 2020년도에 내가 가장 많이 생각했던 점이 예측만 잘 하면 되는거지 굳이 해석이 필요한가?라는 질문이다. 이 점이 아마도 머신러닝과 딥러닝의 차이점이 아닐까 싶은데 '블랙박스' 라는 특성이 왜 한계점인지를 잘 몰랐었다. 어쨋든 실제로 데이터 분석을 하는 곳에서는 예측이 목표라고 생각했던 과거의 나는 교수님한테도 물어보고, 여러 공모전도 나가면서 나름의 해답을 "설득"이라는 곳에서 찾았다. 데이터 분석 만으로 끝나는 것이 아니라 데이터 분석을 통해 매출을 증대시킨다던가, 정책 도입 등 다른 사람들이 데이터 분석의 결과를 이용하게 되는데, 이 때 정책 결정자나 회사의 CEO 등 다른 사람에게 분석 결과에 대해 설명하는데 '블랙박스'의 특성이 한계점이라고 생각했다. 이건 공모전에서 분석 결과를 파워포인트로 요약 정리 해서 발표하면서 느꼈다. 결국 데이터 분석 공모전이란, 나의 분석 결과를 심사위원들에게 설득시키는 과정이라고 느끼게 되었다. 모델구축 , 검증에서 끝나는 것이 아니라 한가지 단계가 더 남아있었던 것이다. 즉 데이터 분석의 목적은 예측 뿐 만이 아니라 예측값을 다른 사람들에게 설득시키기 위해 분석 결과에 대한 해석도 중요하다고 생각했다. 이 프로젝트에서 딥러닝을 많이 사용했는데, 다른 사람들이 은닉층에서 어떤 일이 일어나는 지를 궁금해했고, 나는 그저 "알 수 없다."라는 말 밖에 할 수가 없었다. 이 말은 받아들이는 사람도 답답해 했고, 딥러닝을 하나도 모르는 사람에게 분석 결과를 설명하면서 나도 조금 많이 엄청 답답했다. 

- 단어의 순서를 시간의 변화로 보고 예측 / 분류 / 군집(유사도 측정) 등을 진행한다는 것이 정형데이터, 특히 시계열 데이터의 분석기법과 비슷한 느낌이었다.

