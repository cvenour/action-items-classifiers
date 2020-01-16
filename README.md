# action-items-classifiers
Here is the code for 5 action item classifiers I implemented: Two decision trees (xgboost and catboost), a Support Vector Machine (SVM), a Recurrent Neural Network that uses glove vectors in its embedding space. <br>

What is an action item classifier? It's fed sentences/utterances that were said at a meeting and it decides whether the utterance is an action item or not. (An "action item" is just a silly business term which means a task). So this system will automatically find, in the transcripts of meetings, tasks that were assigned to people.

For more information about the work here, see: https://www.youtube.com/watch?v=Oa9NZULXYdg&list=PLDZq-P7JWYyzzziWMkPlxPOH2-M0rsJGa&index=21


Of these 5 classifiers, the fastai Language Model with classifier on top yields the best results:<br>
**88.3% precision** <br>
**90.7% recall** <br>

But as the video in the link above talks about, I also implemented a BERT solution and that (6th solution which is not included in this repository) yielded the best results of all: <br>
**88.5% precision** <br>
**92.6% recall**
