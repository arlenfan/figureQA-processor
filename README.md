Please note that the `png/` directory and the `annotations.json` are linked.
The json file contains the labels for all the stuff in the png file.

I only used a small sample of the FigureQA dataset from
`figureqa-sample-train-v1.tar.gz(21.24 MB)`


To build a model with bigger datasets, please find the figureQA archives at:
https://msropendata.com/datasets/85596452-0fe3-4335-bc00-ae83ee8ffcfd

or

https://drive.google.com/drive/folders/16cVHT7ZRjhgBuS0TgpHT9cjAuBWnSj3l?usp=sharing



The structure of the code is here. You may replace `png/` and `annotations.json` with another version to build those bigger datasets.


Please run `scrapper.ipynb` to preprocess all the data.

then run `transfer_learn_charts.ipynb` to get the results of the classification.
Please note that this is similar to the ants and bees classification task.


Instead of 2 layers at the end, there are 5 layers at the end.


```
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
```

This is how the dataloader works.