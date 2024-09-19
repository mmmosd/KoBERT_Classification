KoBERT를 이용한 글 Tag 적용 시스템
============================

이 프로젝트는 창업 아이디어들의 내용을 토대로 Tag를 적용하기 위해 KoBERT를 사용한 분류 모델이다.
Tag는 여러 개가 있을 수 있으므로 Multi-Label 분류를 하였다. 

Multi-Label Classification
-----------------------

일반적인 분류 모델과는 다르게 다중 레이블 분류 (Multi-Label Classification)는 데이터가 동시에 여러 카테고리에 속할 수 있는 상황을 다룬다. 이를 통해 여러 종류에 속하는 창업 아이디어의 Tag를 적용할 수 있었음.

학습 데이터
-----------

학습 데이터는 ChatGPT를 통해 임의로 생성해 낸 약 2500개의 문장들을 사용하였다.

학습 하이퍼파라미터
-----------

max_len = 64
batch_size = 64
warmup_ratio = 0.1
num_epochs = 10
max_grad_norm = 1
learning_rate =  5e-5

학습 결과
-----------

![train_result](![image](https://github.com/user-attachments/assets/b2f707b6-a1b2-4f6b-9710-b76d48b57008)
)
(학습 결과)

![test_result](![image](https://github.com/user-attachments/assets/139f2f3f-28cb-4f61-9e82-a63d31d7610d)
)
(테스트 결과)

![test](![image](https://github.com/user-attachments/assets/a1e552b8-12be-4a95-8805-d3fc9aa1fb97)
)
(실제로 잘됨)

하지만 이럼에도 불구하고 학습 데이터의 양이 많지 않았으며, 학습 데이터의 품질도 좋지 않아 분류가 잘 되지 않는 Tag들도 있었다. 이러한 문제는 추후에 데이터를 얻게 된다면 해결될 문제인 듯 하다.
