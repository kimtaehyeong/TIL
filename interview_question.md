# 면접질문 모음

## 

* 왜 eigenvector & eigenvalue ?
 def: n x n 크기의 A martix가 있을때, AK = λK를 만족하는 K가 있을때, K를 eigenvector라고 하며, 숫자 λ를 eigenvalue라고 한다.
  * AK = λK, AK-λK =0, (A-λI)K=0 으로 묶을수 있고, (A-λ)의 역행렬이 존재한다면, K=0이 될수 있으므로 K는 0이 아니라는 가정이 들어간다. (그래프로 그려놓고 이해하면 쉽다)
  * 그렇다면 기하학적으로 생각해보면 어떠한 선형변환 A가 있을때, 크기만 변하고 방향이 변하지 벡터에 이용가능하며 얼마나 변한지에 대해서 λ를 이용해서 확인이 가능하다.
  
* Sampling & Resampling?
   * Sampling은 크게보면 비복원 추출법과, 복원 추출법이 있으며 대표적으로 jackknifing, bootstrapping이 대표적이다.  
     * 복원추출은 한번 시행한 결과를 다시 얻을 수 있도록 모집단에 다시 포함시켜 시행하는 추출방법이여서 같은 원소가 계속 뽑힐수 있는 점이다.
     * 비복원 추출은 한번 시행한 결과를 다시 모집단에 포함하지 않고 시행하는 추출방법이다.
   * Resampling은 표본을 추출하면서 원래 데이터 셋을 복원할 수 있는데, 이를 통해 가정도 필요 없이 표본만으로 추론이 가능하고 통계학적으로 신뢰 구간을 추론할 수 있다. 즉, 모집단 데이터에 가정이나 정보 없이도 분포 성질을 분석할 수 있다는 점!  
   
  
* Bagging & Bootstrapping?
   * bagging의 경우는 bootstrap aggregation의 줄임말로, 주어진 데이터에 대해서 bootstrap 자료를 생성하고 각 bootstrap된 자료를 각 모델링에 대해 나온 결과를 최종 결과물로 산출하는 방법이다. 일반적으로 예측 모형의 변동성이 큰 경우, 변동성 감소를 위해 사용한다.
   * Bootstrapping은 통계학에서 가설 검증을 하거나 평가지표를 계산하기 전에 랜덤 샘플링을 적용하는 방법이다. (중복허용)





* Reference

  https://zzsza.github.io/data/2018/02/17/datascience-interivew-questions/

  https://www.cpuheater.com/deep-learning/deep-learning-interview-questions-and-answers/

  
