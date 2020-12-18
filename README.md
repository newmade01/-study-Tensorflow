# Tensorflow 
Tensorflow 기본

#출처: 유투브 김성 교수님 강의자료


###[]

anaconda, vscode, python



[Hypothesis, 가설]  H(x)=W*x+b #W와 b의 값을 학습하게 된다.

-regression:

  --one-variale one-feature EX)exam Score값 예측
  
  --multi-variable feature EX) final  점수 (w와x의 값이 늘어남)
    
   ---Matrix multiplication => H(X)=XW #TensorFlow



[Cost function] 실제값과 예측값의 제곱값



[Gradient Descet algorithm] cost의 최적화 알고리즘

-Convex function
  
  --항상 답을 찾아나감
  
  --cost function의 형태 확인
  
  
  
[Simplified hypothesis]
  
 -H(x)=W(x) #+b 함수가 사라짐 #W가 최저되는 



[classification] 분류예측

-EX)주식, facebook 카테고리 검색 등



[Logistic Hypothesis]

-1과 0사이의 Hypothesis

-Sigma 형태

-[cost fuction]: 실제와 예측값이 같으면 cost값은 작아짐, 틀리면 cost값이 커짐

   --y=1: -log(H(x)) #0에 가까워짐
   
   --y=0: -log(1-H(x)) #0이면 거의 0, 1이면 무한대에 가까워짐
   
   --  ylog(H(x))-(1-y)log(1-H(x))
   
 #cost function
 
  cost=tf.reduce_mean(-tf.reduce_sum(Y*tf.log(hypothesis)+(1-Y)*tf.log(1-hypothesis)))
   
-[Minimize cost]

  -cost(w): 미분한 값에 
  
  #Minimize
  
  a=tf.Variable(0.1)
  
  optimizer=tf.train.GradientDescentOptimizer(a)
  
  train=optimizer.minimize(cost)
  
-[Gradient decent algorithm]




[Logistic Regression]

-cost(W)값을 작게하는 값을 구해야한다.

-양쪽 W를 구함



[Multinomial classification]

  
  
   
   
   


