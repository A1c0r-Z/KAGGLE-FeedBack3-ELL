# KAGGLE-FeedBack3-ELL
This is a conclusion of Feedback Prize - English Language Learning [here](https://www.kaggle.com/competitions/feedback-prize-english-language-learning).\

# Table of contents
* [OVERVIEW](#-OVERVIEW)
  - [Train](##-Train)
    - [model used](###-model-used)
  - [Inference](##-Inference)
* [LOG](#-LOG)
# OVERVIEW
## Train

During the competition I only used deberta-v3-base and deberta-v3-large with mean pooling and attention pooling.\
This time I'm going to train more model
### model used:
1. deberta-v3-base
2. deberta-v3-large
3. deberta-v2-xlarge
4. roberta-large
5. distilbert-base-uncased
## Inference
# LOG
## 12.14
info:\
  1. deberta-v3-base
  2. attention head
  3. layerwise learning rate decay
  4. last layer reinitialization(kaiming normal)
  5. Different loss rates per target `{'cohesion':0.21, 'syntax':0.16, 'vocabulary':0.10, 'phraseology':0.16, 'grammar':0.21, 'conventions':0.16}`
  6. Finetuned with optuna
 got 0.4502 in cv
 
 




During the competition, I got 129/2654 on public lb,but got only 591/2654 on private lb.So I want to do this competition again and make a late submission.
