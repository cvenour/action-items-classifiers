# action-items-classifiers
Here is the code for 5 action item classifiers I implemented: xgboost, catboost, support vector machine, RNN + glove vectors. <br>

What is an action item classifier? You feed the classifier sentences/utterances that were said at a meeting and this system decides whether the utterance is an action item or not. (An "action item" is a silly business term which means a task  - i.e. a something someone has to do).

For more information about the work here, see: https://www.youtube.com/watch?v=Oa9NZULXYdg&list=PLDZq-P7JWYyzzziWMkPlxPOH2-M0rsJGa&index=21


Of these 5 classifiers, the fastai Language Model with classifier on top yields the best results:<br>
precision: 0.8828828828828829 <br>
recall: 0.9074074074074074 <br>

But as the video in the link above talks about, I also implemented a BERT solution and that (6th solution) yielded even better results.
