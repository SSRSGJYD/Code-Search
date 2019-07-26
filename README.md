# Code-Search

This is a project of summer internship in Microsoft.

#### Data
+ Python & JavaScript files with most stars on Github
+ JavaScript packages from npm
+ Python & JavaScript answers with most stars on StackOverflow
+ Python codes from BigQuery

#### Method: Code2Vec
First, extract path-contexts from Python & JavaScript files respectively. Code is at https://github.com/SSRSGJYD/astminer.

Then run
```shell
python makeDataset.py
```

to generate dataset for training and validation.

After that, feed the code files into a baseline model to generated label from training and validation set. Code is at https://github.com/maoyutao/baseline.

Finally, train the model in 