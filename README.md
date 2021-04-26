# Cosmetic-Review-Analysis

- 진행날짜 : 2021.03.02 ~ (ing)

- 이번 플젝은 대외비여서 많은 코드를 올리지는 못할듯 싶다.
- 그래도 기본적인 모델 코드는 올려야지~
- 일단 이 플젝이 다 끝나고 올려야겠다.

</br>

- 원래 학과 수업의 일환으로 시작되었지만,,,
- 어쩌다 보니 규모가 커지게 되었고 실제 데이터 분석이 기업에서 어떻게 쓰일 수 있을 것인지를 생각할 수 있는 기회가 되었다.
- 분석가의 관점뿐 만이 아니라 CEO의 관점에서 데이터 분석을 바라보는 것을 생각해보았다.
- 실제 회사에서 데이터 분석이 어떻게 쓰이는 지 경험을 해봤다고나 할까...?


</br>

- 자연어 처리는 조금 재미가 없었다.
- 재미가 아닌 책임감으로 하고 있는 프로젝트......
- 데이터가 sparse 했지만 그건 문제가 아니였던 것 같고, 뭔가 숫자가 아닌 텍스트 분석 자체가 재미가 없었다.
- sparse한 데이터는 pca와 t-sne를 통해 차원축소로 해결하였다.
</br>

- 하,,, 비지도 학습으로 딥러닝 돌릴라고 했는데ㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠ
- 하하하하하하하하ㅏ하하 
- 전처리 너무해,,,
- 한국어가 힘든건가? 
- ~만은 부정의 의미? 아니야,,, 제한 or 한정의 의미도 있기 때문에 부정이라고 단정 지을 수 없어,,,,
- 하지만 무향이지만 이건 긍정? 부정?
- 데이터 라벨링 진짜 하나하나 해야하나...?
- 근데 만약 데이터 라벨링 했다고 쳐
- 그럼 그 문장에 대한 긍/부정이지 향기에 대한 긍/부정인지 파악하기 힘들듯
- 그럼 "향기"라는 단어 바로 앞/ 뒤에 나오는 단어가 긍정/부정인지 파악해야해...?
- 하지만 이런경우가 있었어,, -> 제가 좋아하는 향기는 아니지만 흡수가 좋아요-> 이건 좋아하는 + 아니지만 -> 긍정 +1, 부정 -1  -> 0점
- 이건 중립으로 나오는데 but 향기에 대해서는 부정!
- 하 진짜 데이터 전처리 오바다,,,,
- ㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠㅠ


- 걍 아싸리 딥러닝 돌릴까...?
- 교수님이 자꾸 은닉층가지고 뭐라고 하는데!!!
- 그래서 감성사전 통해서 나름 수학적으로 풀었는데 결과가 안조아ㅠㅠㅠ
- 일단 교수님한테 말해볼거야,,,,



</br>

- NLP를 할 바에는 차라리 vision을 할테야

# 느낀 점
- 2020년만 해도 나는 통계보다는 코딩이 더 좋다고 생각했는데 막상 컴퓨터 공학을 많이 사용하는 인공지능 중에서 자연어 처리 프로젝트를 하니까 통계가 더 좋다고 느꼈다ㅋㅋㅋㅋㅋㅋ
- 역시 사람은 겪어봐야지 아는 것 같다.

- 텍스트 분석보다는 비전이 더 좋은 것 같고 비전보다는 그냥 숫자와 같은 정형데이터 분석이 더 재미있는 것 같다.
- 이런 딥러닝을 사용한 프로젝트를 통해 도출된 결론을 가지고 남들을 설득시키는 것이 어렵다는 것을 알았고, 이 이유는 딥러닝에서 중요한 hidden layer (은닉층) 때문에 나온 블랙박스라는 딥러닝의 한계점이 있는 것 같다.

> 2020년도에 내가 가장 많이 생각했던 점이 예측만 잘 하면 되는거지 굳이 해석이 필요한가?라는 질문이다. 이 점이 아마도 머신러닝과 딥러닝의 차이점이 아닐까 싶은데 '블랙박스' 라는 특성이 왜 한계점인지를 잘 몰랐었다. 어쨋든 실제로 데이터 분석을 하는 곳에서는 예측이 목표라고 생각했던 과거의 나는 교수님한테도 물어보고, 여러 공모전도 나가면서 나름의 해답을 "설득"이라는 곳에서 찾았다. 데이터 분석 만으로 끝나는 것이 아니라 데이터 분석을 통해 매출을 증대시킨다던가, 정책 도입 등 다른 사람들이 데이터 분석의 결과를 이용하게 되는데, 이 때 정책 결정자나 회사의 CEO 등 다른 사람에게 분석 결과에 대해 설명하는데 '블랙박스'의 특성이 한계점이라고 생각했다. 이건 공모전에서 분석 결과를 파워포인트로 요약 정리 해서 발표하면서 느꼈다. 결국 데이터 분석 공모전이란, 나의 분석 결과를 심사위원들에게 설득시키는 과정이라고 느끼게 되었다. 모델구축 , 검증에서 끝나는 것이 아니라 한가지 단계가 더 남아있었던 것이다. 즉 데이터 분석의 목적은 예측 뿐 만이 아니라 예측값을 다른 사람들에게 설득시키기 위해 분석 결과에 대한 해석도 중요하다고 생각했다. 이 프로젝트에서 딥러닝을 많이 사용했는데, 다른 사람들이 은닉층에서 어떤 일이 일어나는 지를 궁금해했고, 나는 그저 "알 수 없다."라는 말 밖에 할 수가 없었다. 이 말은 받아들이는 사람도 답답해 했고, 딥러닝을 하나도 모르는 사람에게 분석 결과를 설명하면서 나도 조금 답답했다.



**자연어 처리 절대 다시는 안 할거야... **
*누가 그랬지...? 자연어 처리 하면 빨리 늙는 다고,,, 그 말 뭔지 이제 알겠다,,,, 이성배 오빠가 그랬나...? 대체 그 오빠는 왜 자연어 처리가 좋을 걸까? 뇌구조 궁금하다*
