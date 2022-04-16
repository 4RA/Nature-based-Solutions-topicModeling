## NbS(Nature-based Solutions) 연구 동향 분석

### 분석 주제 
nbs(Nature-based Solutions) 자연기반해법 활용 - 기후변화 대응을 위한 신림부문의 자연기반해법 활용 논문

### 분석 목표 
nbs 관련 논문의 연구 동향을 파악하고 이를 어떻게 국내 산림 분야에 응용할 수 있는지 결론 도출 

### 분석 방법 
- nbs 관련 논문 파악하여 분류 후 연도별 연구동향 분석 
- Topic Modeling : LDA
- Association Analysis


### 세부 

### 프로젝트 목적

자연기반해법에 대한 **연구 및 주요 주제**에 대한 관심에 대한 동향 분석

### 데이터 수집

- NbS를 관련 키워드에 포함하고 있는 논문들을 모집단으로 구축한 후 제목, 초록, 발행연도 등의 정보를 수집하여 NbS에 대한 그동안의 연구동향을 분석하고자 한다.

### 데이터 전처리

- 대문자를 소문자로 변경
- 띄어쓰기 공백과 모든 구두점을 제거하여 토큰화 작업 수행
- 빈번하게 사용되는 전치사, 관사, 특수 문자 등 불용어 제거
- 동일 의미 단어를 하나의 단어로 변환하는 어간추출(Stemming) 작업 수행
- 최소 100개 이상의 논문에서 공통적으로 등장하는 키워드들만으로 분석 단위 한정

### 데이터 분석

- 분석에 활용된 전체 단어노드에 대한 빈도를 분석해 핵심 키워드 도출
- 전체 단어노드의 평균 TF-IDF는 284.40으로 본 연구에서는 TF-IDF 값 0.1을 임계치로 설정하여 이보다 큰 가중치 값을 갖는 단어들을 대상으로 LDA 분석에 활용
