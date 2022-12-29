# Natural language processing (determination of the toxicity of comments)

## Description of the project

The online store is launching a new service. Now users can edit and supplement product descriptions, as in wiki communities. That is, clients offer their edits and comment on the changes of others. The store needs a tool that will search for toxic comments and send them for moderation.

Train the model to classify comments into positive and negative. At your disposal is a data set with markup on the toxicity of edits. Build a model with the value of the quality metric *F1* at least 0.75.

## Description of data

The `text` column in it contains the comment text, and `toxic` is the target.

## Tools used

`spacy` `pymystem3` `re` `sklearn` `pandas` `numpy` `matplotlib`

## Models used

`LogisticRegression` `CatBoostClassifier`

## Addition tools

`TfidfVectorizer` `Lemmatizer` `Lookups` `GridSearchCV`

## Metrics

`f1_score`