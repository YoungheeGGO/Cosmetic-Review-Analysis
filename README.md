
- Period : Mar.20.2021 ~ May.30.2021

## Why did I analyze the data?
- Price competition is intensifying due to the rapid increase in various new brands, direct management stores, and franchises. -> Deteriorating profitability of cosmetic manufacturers
  - (ref: *Industrial Trends Report,* Cosmetics Industry Trends, and K-Beauty Global Competitiveness Analysis)
- The cosmetics market is attempting to apply the latest trend analysis techniques using big data such as SNS data.
  - (ref: 2018 Global Cosmetics Market Trend Analysis Seminar)
- Asia's share of skin care products is about 41%, which is overwhelmingly competitive.
  - (ref: Case analysis of brand concept development through big data analysis of cosmetics companies, Jumin Lee, Jounghae Bang)
- So, I decided to understand consumption trends through a review analysis of Skin Care's flagship product "Hand Cream."

## Analysis Process Description 
**1. Crawling**
- I had web crawling the website that exists revies about cosmetics.
- There was so many types of cosmetics, I had narrowed down the analysis object to "Hand cream".
- And There was ranking about handcream sales, I had crawl just high (ranking 1\~3), middle (ranking 50\~52), bottom ranked(ranking 98\~100).
- Also, The user information about age, gender, written date, skin type(dry, oily, sensitive, combination) were crawled. 

**2. EDA**
- I made the word clouds per its reviewr's age, gender, skin type with the review text.
- Word Cloud of 20's Female who has dry skin 
<img src="https://user-images.githubusercontent.com/102137580/160996581-9ce11c26-2d42-476e-b778-1a0a57b8d566.png" width="500" height="300">

- Word Cloud of  30's Male who has combination skin 
<img src="https://user-images.githubusercontent.com/102137580/160998036-8a6e8de1-45b3-4638-812d-b50dc798853f.png" width="500" height="300">

- Except for general word like *Hand, Cream, Product*, there was a common word not regarding age, gender, skin type : *Absorption, Price, Scent, Moisturizing*


**3. Word2vec**
- Using the shallow neural net, that has one hidden layer, I embedded the word in the high dimension.
- Especially I used the CBow(Continuous Bag of Words) method, not Skip-Gram.

**4. Conclusion & Significance**
- In an embedded word, I find out the correlation the word *Absorption, Price, Scent, Moisturizing* to "good".
- Top ranked

| word | rank 1 | rank 2 | rank 3 |
| ---- | ------ | ------ | ------ |
| Scent | 0.69 | 0.18 | 0.83 |
| Moisturizing | 0.70 | 0.18 | 0.83 |
| Absorption | 0.7 | 0.19 | 0.79 |
| Price | 0.56 | 0.11 | 0.71 |

- Further to the existing positive and negative analysis, the causes of positive/negative thoughts were analyzed from various angles in terms of *scent, price, moisturizing, and absorption.*

## What I felt.
- Originally started as part of a department class, it became an opportunity to think about how data analysis could be used in companies as it was linked to actual companies by winning the Capstone design project.
- The first project that I did by myself without team members or anyone else! I did a lot of useless things...! (Like raw material analysis)
- It was found that not only quantitative analysis but also qualitative analysis using domain knowledge is necessary.
- I found it difficult to persuade others with conclusions drawn through projects using deep learning.
- It felt similar to the analysis technique of structured data, especially time-series data, that the order of words was viewed as a change in time and predicted/classified/clustering (similarity measurement).
- Everyone was reluctant to deep learning because of the limitations of deep learning called the black box, which came out because of the hidden layer.
  - I thought studying XAI will be interesting.

## The point that need to improvement
- 딥러닝 돌릴만큼의 데이터가 충분히 확보되지 않았음.(top 랭크만 데이터가 많았다.) 하지만 그럼에도 불구하고 결과가 잘 나온 이유는 아마 문장에서 호불호가 명확하게 드러났기 때문으로 유추해 볼 수 있을 것 같다.
- 2위 데이터 오염 
