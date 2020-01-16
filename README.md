# Action Item Classifiers
Here is the code for 5 action item classifiers I implemented: two decision trees (xgboost and catboost), a Support Vector Machine (SVM), a Recurrent Neural Network that uses previously built Glove vectors in its embedding space, and a fastai Language Model (pre-trained on wikitext-103) with a classifier added on top which is fine-tuned to recognize action items. <br>

What is an action item? An "action item" is just a silly business term which means a task that is assigned to someone. The action item classifiers I implemented will automatically find, in the transcripts of meetings, tasks that were assigned to people. You feed sentences/utterances that were said at a meeting to these action item classifiers and they decide whether the utterance is an action item or not. <br>

For more information about the work here, see: https://www.youtube.com/watch?v=Oa9NZULXYdg&list=PLDZq-P7JWYyzzziWMkPlxPOH2-M0rsJGa&index=21


Of these 5 classifiers, the fastai Language Model with classifier on top yields the best results:<br>
**88.3% precision** <br>
**90.7% recall** <br>

But as the video in the link above talks about, I also implemented a BERT solution and this solution, which is not included in this repository, yielded the best results of all: <br>
**88.5% precision** <br>
**92.6% recall**
