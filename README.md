# 2019 KBO타자 성적 예측 대회 (DACON)

> 대회 개요 및 설명 - [DACON](https://dacon.io/cpt6/62885)



### Predict

- 2019년 타자들의 상반기 **OPS** 예측



### Evaluation

- **Weighted Root Mean Squared Error(WRMSE)**

  $WRMSE = \sqrt{ \frac {\sum( (trueOPS - predOPS)^2 \times AB)} {\sum{AB}} }$ ,  $AB$ : 타수

- 



### 코드 검증 절차

1) Data Cleansing

2) Visualization

3) Feature Engineering

4) Model Building



### 데이터 설명

1) Regular_Season_Batter.csv : KBO에서 활약한 타자들의 역대 정규시즌 성적을 포함하여 몸무게, 키 ,생년월일 등의 기본정보

2) Regular_Season_Batter_Day_by_Day.csv: KBO에서 활약한 타자들의 일자 별 정규시즌 성적

3) Pre_Season_Batter.csv : KBO에서 활약한 타자들의 역대 시범경기(정규시즌 직전에 여는 연습경기) 성적

4) submission.csv : 참가자들이 예측해야 할 타자의 이름과 아이디 목록