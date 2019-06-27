# simple-binary-text-classification
simple tutorial of binary text classification

## Framework
- Tensorflow cpu-1.14
  - (it also works on tensorflow 2.0 alpha gpu. it need to do some adjustments for adapting the version)

## Run env
jupyter notebook

## Model:
1. Bidirectional GRU + glove `updated`
2. BiGRU + glove + attention `(updating)`
3. ELMo embedding model`(updating)`
4. Bert `(updating)` 
5. (*maybe have one GPT)

## issus may occur：
1. while import seaborn:
DLL load failed: The specified procedure could not be found.

please checking the traceback whether it causes of seaborn.
I met this because of scipy ---> 21 from scipy.sparse.linalg import LinearOperator
solution: remove conda version and reinstall pip one
$> conda remove --force numpy, scipy
$> pip install numpy, scipy
https://github.com/conda/conda/issues/6396

2. version issus: update the version or use the correct format of the current version

## References:
- [deep.ai cources](https://www.coursera.org/specializations/deep-learning?)
- [Illustrated Guide to LSTM’s and GRU’s: A step by step explanation](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)
- [A Step-by-Step NLP Guide to Learn ELMo for Extracting Features from Text](https://www.analyticsvidhya.com/blog/2019/03/learn-to-use-elmo-to-extract-features-from-text/)
- [NLP at IEST 2018: BiLSTM-Attention and LSTM-Attention via Soft
Voting in Emotion Classification](https://www.aclweb.org/anthology/W18-6226)
- [FEED-FORWARD NETWORKS WITH ATTENTION CAN
SOLVE SOME LONG-TERM MEMORY PROBLEMS](https://colinraffel.com/publications/iclr2016feed.pdf)
- [Overfitting in Machine Learning: What It Is and How to Prevent It](https://elitedatascience.com/overfitting-in-machine-learning#how-to-detect)
- [Transfer Learning using ELMO Embeddings](https://github.com/sambit9238/Deep-Learning/blob/master/elmo_embedding_tfhub.ipynb)
