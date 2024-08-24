KoBERT를 이용한 글 Tag 적용 시스템
============================

이 프로젝트는 창업 아이디어들의 내용을 토대로 Tag를 적용하기 위해 KoBERT를 사용한 분류 모델이다.
Tag는 여러 개가 있을 수 있으므로 Multi-Label 분류를 하였다. 

Multi-Label Classification
-----------------------

일반적인 분류 모델과는 다르게 다중 레이블 분류 (Multi-Label Classification)는 데이터가 동시에 여러 카테고리에 속할 수 있는 상황을 다룬다. 이를 통해 여러 종류에 속하는 창업 아이디어의 Tag를 적용할 수 있었음.

학습 결과
-----------

![train_result](https://github.com/mmmosd/KoBERTag/blob/main/train_img/train_history.png)
(학습 결과)

![test_result](https://github.com/mmmosd/KoBERTag/blob/main/train_img/test_history.png)
(테스트 결과)
