# Aspect Term Extractor (ATE)


An ATE is a model that extracts aspect terms from a review, i.e. for each word of a review, your model should predict if the word is an aspect term or not of the reviewed product.
The input data has the following format: review → list of aspect terms, e.g. "The battery life is really good and its size is reasonable" → “battery life”, “size”. Recommend to change it and use the BIO format instead. Example:

```
Converting this sentence to BIO would look like this -

The O
barrery B
life I
is O
really O
good O
and O
its O
size B
is O
reasonable O
```

With this format, we can see that the role of an ATE is to assign to each word one of the three possible classes:
```
O = not an aspect (Outside)
B = first word of an aspect (Beginning)
I = second, third, ... word of an aspect (Inside)
```

## Required Libraries:
NLTK, Sklearn, Pandas, matplotlib, Stanford corenlp


