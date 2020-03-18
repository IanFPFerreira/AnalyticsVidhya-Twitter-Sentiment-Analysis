# AnalyticsVidhya: Twitter Sentiment Analysis

## Descrição do problema
O objetivo desta tarefa é detectar o discurso de ódio nos tweets. Por uma questão de simplicidade, dizemos que um tweet contém discurso de ódio se tiver um sentimento racista ou sexista associado a ele. Portanto, a tarefa é classificar os tweets racistas ou sexistas de outros tweets.

Formalmente, dada uma amostra de treinamento de tweets e rótulos, onde o rótulo '1' indica que o tweet é racista / sexista e o rótulo '0' indica que o tweet não é racista / sexista, seu objetivo é prever os rótulos no conjunto de dados de teste.

Página da Competição: https://datahack.analyticsvidhya.com/contest/practice-problem-twitter-sentiment-analysis/

## Versão Python
```python
3.8.0
```
## Bibliotecas utilizdas
```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import nltk
from nltk.corpus import stopwords 
from nltk.stem.wordnet import WordNetLemmatizer
import re
import collections
from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
from sklearn.linear_model import SGDClassifier
from sklearn.model_selection import train_test_split
from sklearn.pipeline import Pipeline
from sklearn.metrics import confusion_matrix
from sklearn.utils import resample
from sklearn.metrics import f1_score
from wordcloud import WordCloud
```

# Score obtido:
  **0.654748603351955**
