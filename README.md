**코드 분석**

사전 훈련된 모델 로딩
사전 훈련된 VisionEncoderDecoderModel내용을 검색하여 GPU로 옮겨 가속 훈련을 실시

구성 조정
모델 구성 내의 특정 속성( model.config)이 조정됩니다. 여기에는 어휘 크기, 최대 캡션 길이, 빔 검색 매개변수 설정 등이 포함

훈련 논증
학습 인수는 를 사용하여 정의되며 Seq2SeqTrainingArguments학습, 평가, 모델 검사점에 대한 매개변수를 지정

모델 훈련
Seq2SeqTrainer모델은 지정된 훈련 및 검증 데이터 세트를 사용하여 훈련되고 평가
