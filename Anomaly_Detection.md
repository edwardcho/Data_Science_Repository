
Anomaly Detection : Normal sample 과 Abnormal sample 을 구별해 내는 문제

1. Normal Sample : 단일 Class

  a. Supervised   <br>
     : 모든 sample (Normal sample 과 Abnormal sample) 에 대해 Label 필요
     
     : training 후 Abnormal 에 대해 정확도 높음
     : Abnormal sample 취득에 많은 시간/비용
     : training 시 데이터 개수 balance 문제 발생 예상
     
  b. One-Class Classification (다른 말로 semi-supervised 라고 부르는 곳에 있음)  <br>
     : Normal sample 에 대해 label
     : Normal sample 만 training
     : boundary 벗어나는 것에 대해 abnormal 판정
     
     -. One-Class SVM (Support Vector Nachine)   
     -. Deep Learning 기반의 Deep SVDD (Support Vector Data Description)
     -. Enerpy-based 방법 (?)
     -. Deep Autoencoding GMM (Gaussian Mixture Model) 방법
     -. GAN 기반 방법
     
  c. Unsupervised   <br>
     : 대부분의 데이터가 Normal sample 이라는 가정
     : 차원 축소 후 복원 과정을 통해 Abnormal 검출
     
     -. Auto-Encoder 방법
        (Normal sample 로 AUto-Encoder training)
        (Normal sample 은 input/output 거의 동일)
        (Abnormal sample 은 input/output 차이 발생)
        
   * 용어  <br>
     Novelty Detection : 같은 종류, 보지 못했던 타입, 등장할 가능성이 있는 것에 대한 detection  <br>
     Outlier Detection : 다른 종류, 등장할 가능성이 거의 희박한 것에 대한 detection   <br>
     
2. Normal Sample : 여러 Class
 
       : (normal sample : 단일 class)    ===>   (normal sample : 여러 class)  <br>
       :       Normal sample                      In-distribution sample        <br>
       :      Abnormal sample                    Out-of-distribution sample     <br>
         
   Out-of-distribution Detection : In-distribution sample 로 training    <br>
                                   test 에서 out-of-distribution 검출     <br>
                                   
                                   

