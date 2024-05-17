# Features
Model predicts american letters using sign language and return the output to use in gui.  <br>
Worked in a team of 4 people and managed to finish the project and test it in a short amount of time. <br>
Used dataset link ---> https://www.kaggle.com/datasets/grassknoted/asl-alphabet/data
# Bugs and Errors
Model faces an over-fit with accuracy 97% which can be easily fixed by using different dataset images from kaggle but in this project we had no time or the welfare of waiting
just make sure that <br>
1-you use a good amount of different training images and test images <br>
2-val folder is a mixture of training images and test images that allows you to increase accuracy <br>
3-you may add all the files to training folder and use the following code it will automatically divide them in a certain ratio that you can change yourself and create the needed folder (train-val-test)
<pre>
  import splitfolders
  train_src = "asl/asl_alphabet_train/asl_alphabet_train"

  splitfolders.ratio(train_src, output="datasets/asl_alphabet",
  seed=1337, ratio=(.8, .1, .1), group_prefix=None, move=False)
</pre>
4-for more details check documentation
