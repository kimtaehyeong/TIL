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
     
       
* 확률 모형 & 확률 변수?
   * 확률 변수는 확률로 표현하기위해 sample space를 정의하는 것. 다양하게 정의가 가능하므로, 일반적으로 변수라는 말을 사용하며 0~1사이의 값으로 매핑 시키는 함수를 확률 함수라고 표현한다.
   * 확률 모형은 불확실성을 확률로써 계량화하기 위해 수학적으로 만든 모형이 바로 확률모형입니다. 그리고 함수에 쓰인 계수들을 모수(parameter)라고 부릅니다. 통계학에서 모수(parameter)를 추정한다는 말을 표현하는데, 데이터 분포를 알고자하는것이 모수를 추정하는것이다.  
  
  
* 확률밀도함수(Probability Density Function)
  * PDF라고 약자로 많이 사용하며, 확률밀도함수는 연속적인 변수에 의한 확률 분포 함수를 의미한다.
  * 특정구간이 다른 구간에 비해 상대적으로 얼마나 높은가를 나타낸 형식인데, 항상 양의 값을 가지며, 모든 PDF를 합하면 1이된다는 특성을 가지고 있다.
  * 어떠한 일정 범위의 확률은 구간 PDF 넓이 즉, 적분값이 된다.
  
* 누적분포함수(Cumulative Distribution Function)
  * CDF라고 약자로 많이 사용하며, 어떠한 확률분포에 대해서 확률변수가 특정값보다 작거나 같은 확률을 나타낸다.
  * CDF를 미분하면 PDF가 나오며, 반대로 PDF를 적분하면 CDF가 나온다.  



* Reference

  https://zzsza.github.io/data/2018/02/17/datascience-interivew-questions/

  https://www.cpuheater.com/deep-learning/deep-learning-interview-questions-and-answers/

  
