# AIFFEL Socar Campus Code Peer Review Templete

코더 : [정영진]

리뷰어 : [채화정]

---

🔑 **PRT(Peer Review Template)**

- [ O ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 잘 첨부되었습니다.
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 퀘스트 문제 요구조건 등이 모두 만족되었습니다.
      <img width="998" alt="image" src="https://github.com/HwajeongChae/AIFFEL_jyj/assets/77561358/67b9c163-8124-4632-a67e-f45702c6f98d">

    
- [ O ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 코드마다 주석이 잘 달려있어 이해하기 쉽습니다.
    - 특히 모델별 학습 및 예측값을 구하는 부분을 함수로 구현하며, 해당 부분에 대한 설명이 명확하게 적혀있습니다.
      <img width="992" alt="스크린샷 2023-09-06 오후 4 52 13" src="https://github.com/HwajeongChae/AIFFEL_jyj/assets/77561358/d1d9d1bb-7d62-4f7e-a57c-2dfd96764fe7">

        
- [ O ]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
”새로운 시도 또는 추가 실험을 수행”해봤나요?**
    - 경고문의 예시와 경고문이 뜨는 이유에 대해 잘 설명해주셨습니다.
      <img width="991" alt="image" src="https://github.com/HwajeongChae/AIFFEL_jyj/assets/77561358/43b89fc8-f92a-4c07-8234-be5644c0addf">

        
- [ O ]  **4. 회고를 잘 작성했나요?**
    - 성과부터 아쉬운 점까지 잘 작성해주셨습니다.
      <img width="931" alt="image" src="https://github.com/HwajeongChae/AIFFEL_jyj/assets/77561358/89ce9fbb-cca7-4c03-955f-450f7bf5b021">


- [ X ]  **5. 코드가 간결하고 효율적인가요?**
    - 라이브러리를 호출할 때, 동일한 라이브러리에서 가져오는 경우
      ```
      from sklearn.datasets import load_digits, load_wine, load_breast_cancer
      
      또는
      
      from sklearn import datasets
      
      digits = datasets.load_digits()
      wine = datasets.load_wine()
      breast_cancer = datasets.load_breast_cancer()
      ```
      로 처리하여 조금 더 간편하게 적어줄 수 있습니다.
  - 또한, 전체 코드의 상위에서 공용함수를 정의했는데, 아래에서 굳이 데이터마다 함수를 재정의하여 사용하지 않아도 됐을 것 같습니다.
---
### 느낀점
> 각 데이터마다 불균형도를 확인하고, 그 데이터의 특성에 맞게 각각의 성능지표를 선정한 이유를 논리적으로 적어주신 부분이 인상 깊습니다. 마지막에 그러한 성능지표를 바탕으로 어떤 모델을 선택했는지도 함께 적어주시면 더욱 좋을 것 같습니다. 이번에 영진님의 코드를 보고, 다음번에 제 프로젝트에서는 어떻게 응용할 수 있는지 배울 수 있었습니다. :+1:
