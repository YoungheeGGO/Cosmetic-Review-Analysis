# Cosmetic-Review-Analysis
- 진행날짜 : 2021.03.02 ~ 2021.05.30

## 분석과정
1. 크롤링
2. EDA
3. Word2vec


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

- 자연어 처리를 하면서 한국어가 복잡하고 분석하기 까다로운 언어라는 것을 알게되었다.
- 또한 NLP가 시계열 데이터 분석과 비슷한 방향성을 가지고 분석한다는 것을 알았다.
- 단어의 순서를 시간의 변화로 보고 예측 / 분류 / 군집(유사도 측정) 등을 진행한다는 것이 정형데이터, 특히 시계열 데이터의 분석기법과 비슷한 느낌이었다.
- NLP도 딥러닝, 컴퓨터 공학이라고 생각했지만 결국 끝까지 파고 들어가면 통계가 나온다는 것을 알았다. 통계 이론 공부 열심히 공부해야겠다.


## 덧,
> 이 때 헷갈렸던 개념이 one-hot encoding 부분인데 통계학에서 배우는 dummy variable과 뭐가 다른건지 이해가 잘 안되었다. dummy variable은 한 컬럼에 속성 값이 A,B,C,D가 있으면 A,B,C 컬럼을 만들어 0과 1의 값만으로 컬럼을 증폭시켰지만, (이 때 D라는 컬럼은 존재하지 않음) one-hot encodnig은 새로운 컬럼들이 나타난 데이터 개수-1 이 아니라 나오는 단어마다 0과 1의 값으로 변환시켰다. 결국 컬럼개수는 출현하는 단어의 개수가 되었다. 이 플젝을 끝내고 곰곰히 생각해보니, 이제는 왜 그런지 조금은 알 것 같다. 내 나름대로 내린 결론은 **표본공간의 크기** 가 달라서 이런 차이가 생기는 것이라고 생각했다! 결론적으로 말하면 원-핫 인코딩과 가변수는 같은 말이다. 단지, dummy variable은 나타나는 속성값에 제한, 즉 sample space에 제한이 있어서 (위 경우, sample sampe={A,B,C,D}) A값도 아니고 B값도 아니고 C값도 아니면 자동적으로 D값이 할당된다. 따라서 D라는 컬럼이 생기면 여러 컬럼에 동일한 정보를 담고있어 다중공선성 문제도 발생하게 되니까 D열을 제거한다. 하지만, "나는 강아지를 좋아해."라는 자연어를 원핫인코딩을 시킨다면, sample space는 무수히 많은 단어가 될 것이다. 다시 말하면 '나는'이라는 자리에 '너는', '우와', 등등 많은 단어가 올 수 있기 때문에 sample space를 정의할 수 없다. 따라서 \[나는, 강아지를, 좋아해] 라는 컬럼들이 생긴다. 즉 '나는' , '강아지' 컬럼이 모두 0이면 '좋아해'라는 단어일 것이라는 확신을 하지 못하기 때문에 원핫인코딩을 하면 컬럼 개수가 (가변수와는 다르게) 나타난 단어수 즉 3개가 될 것이다. 이렇게 이해하니까 결국은 가변수와 원핫인코딩은 같은 개념이었고 표본공간의 크기만 다르다는 생각을 하게 되었다.
