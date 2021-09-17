# COVID19-Fake-News-Detection-Using-BERT
This project finetunes the  pre-trained Bidirectional  Encoder  Representations  from  Transformers  (BERT)  model as our base model. We add BiLSTM layers and CNN layers on the top of the finetuned BERT model with frozen parameters, or not frozen parameters methods respectively. The model performance evaluation results showcase that our best model (BERT finetuned model with frozen parameters plus BiLSTM layers) achieves state-of-the-art results towards COVID-19 fake news detection task. We also explore keywords evaluation methods using our best model and evaluate the model performance after removing keywords, so users can aware those vocabs when identify fake news.

## Description
* Training and testing dataset: _Constraint_train.csv, _Constraint_Val.csv
* Notebook: _ _Final_submission_.ipynb
* Report: _Final_Paper.pdf


## Notebook Description
The notebook section can be summarized as followings:

* 0-Set up
* 1-Load the dataset, set up the GPU, install the transformer
* 2-Begin Tokenize the data
* 3-Train and test Procedure
  * 3.1-BERT Fine Tune
  * 3.2-BERT+CNN
    * 3.2.1 Without Freeze Parameters
    * 3.2.2 With Freeze Parameters

  * 3.3-BERT+Bidirectional LSTM
    * 3.3.1 Without Freeze Parameters
    * 3.3.2 With Freeze Parameters
* 4-Top frequent words in fake news (test dataset)
* 5-Words that carry significant weights in the model
* 6-Top frequent words and model performance
