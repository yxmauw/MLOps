# MLOps Topics

## Model drift
* [Reference](https://home.mlops.community/home/videos/making-software-better)
* Detect drift is happening
* Alert when drift is important enough to do something about
* 2 branches: data drift and concept drift
  * Data drift: changes in distribution of input variables or in labels associated with input variables
  * Concept drift: changes in the relationship between input and output variables
* Schema drift: changes in structure or semi-structured data in data pipelines that don't break things but for some reason they alter the features that are being sent to the model
  * E.g. use one character to describe gender, then changed to a string with more options. So kinds of categories that are represented also change
* Label drift: input distribution has not changed much, but the answers have changed. E.g if get a human to relabel which fashion items are trendy last year, that labels will change this year
* Input drift: affected models that are live. For recommendation or search model, what people search for in summer may be different in winter. different keywords e.g. sandals. distribution of keywords has shifts.
  Or stock level prediction model for various products in different branches, and new products are added to the catalog
