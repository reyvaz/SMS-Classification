
<br>

**[See notebook in Jupyter nbviewer](https://nbviewer.jupyter.org/github/reyvaz/SMS-Classification/blob/master/sms_spam.ipynb)**


## SMS Spam Classification

### Tests different classification algorithms to detect spam in SMS messages  


Different specifications of Naïve-Bayes, Logistic-Regression, and Support Vector Machine models with varying features complexity are tested in order to classify SMS messages as spam or legitimate.  

The dataset contains 5,574 SMS messages in English, tagged according to being ham or spam. It was downloaded from [Kaggle](https://www.kaggle.com/uciml/sms-spam-collection-dataset) on November 15, 2017, and can also be found at the [UCI](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) Machine Learning Repository. Acknowledgements to Tiago A. Almeida and José María Gómez Hidalgo, creators of the original dataset. More information can be found [here](http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/).  

The best performing algorithms are a Naïve-Bayes specification on the entire training dataset dictionary. And a Support Vector Machine specification on character ngrams, plus 3 additional features regarding type and length of character content.  
<br>

```
                           Param  Accuracy    Recall  Precision   ROC AUC
MultinomialNB        alpha = 0.1  0.992103  0.944162   1.000000  0.972081
SVC                     C = 1000  0.993539  0.959391   0.994737  0.979277
```
<br>
The Naïve-Bayes specification is slightly superior in terms simplicity, speed, and better precision on the test dataset. While the SVC specification performs slightly better in all of the other metrics.

#### Contents 
* [sms_spam.ipynb](sms_spam.ipynb) Jupyter Notebook containing classification algorithms in Python 
* [README.md](README.md) this file


