# dacon-smishing-detection-14th
(https://dacon.io/competitions/official/235401/overview/)
---

## 프로젝트 개요
### 배경

올해 1월부터 7월까지 스미싱 범죄 건수는 17만6220건으로 지난해 같은 기간(14만5093건)에 비해 21.5% 증가했습니다.

특히 최근 교묘하고 지능적인 스미싱 문자 패턴으로 인해 고객들의 피해가 증가하고 있습니다. 이를 방지하기 위해 kb 금융그룹과 KISA는 데이코너들에게 도움을 요청합니다.

총 글자수 50,000,000개의 데이터를 활용해 스미싱 탐지 모델을 개발하고 명예와 상금을 동시에 누리세요!

### 규칙
평가 기준  / 평가 비율

private_test data를 통해 나타나는 auc score 순위  / 70%  
Inference time (스미싱 문자 예측에 걸리는 시간) 순위  / 30% 

(순위 동점자 발생시 Private score 순위가 더 상위권인 참가자가 더 높은 순위로 기록됨)

### 데이터
KB금융그룹 및 KISA(한국인터넷진흥원)에서 제공받은 정상문자와 스미싱 문자  
(스폰서의 요청으로 데이터는 공개할 수 없음을 양해 부탁드립니다)

## 프로젝트 구조
### 아이디어
[스미스 요원 최종 PPT](스미스_요원_PPT_제출.pdf)
### 폴더 구조
    ─14회_제출_스미스_요원 : 최종 제출폴더
    │  ├─(0_Data)
    │  ├─1_Model
    │  ├─2_Code_pred
    │  └─3_Code_train
    ├─(data) : Train/Test에 사용된 데이터
    ├─dict : User Dictonary 저장폴더
    ├─exp_code : hyperparameter 실험용 폴더
    ├─model : 모델파일
    ├─(pos_tagged) : 포스태깅 처리 완료된 데이터
    │  ├─(daum)
    │  ├─(kiwi)
    │  ├─(komoran)
    │  ├─(mecab)
    │  └─(okt)
    ├─research_code : 모델 리서치용 코드
    │  ├─eda-preprocessing
    │  ├─embedding-method
    │  ├─rule-based-model
    │  ├─naive-basian-model
    │  ├─RNN-model
    │  │  └─output
    │  ├─LSTM-model
    │  │  └─output
    │  ├─CNN-model
    │  └─visualization
