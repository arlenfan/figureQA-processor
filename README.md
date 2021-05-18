Please run scrapper.ipynb to preprocess all the data.

then run transfer_learn_charts.ipynb to get the results of the classification.
Please note that this is similar to the ants and bees classification task.


Instead of 2 layers at the end, there are 5 layers at the end.


 data
   |-train
       |- dot_line
       |- hbar_categorical
       |- line
       |- pie
       |- vbar_categorical
   |-val
       |- dot_line
       |- hbar_categorical
       |- line
       |- pie
       |- vbar_categorical


This is how the dataloader works.