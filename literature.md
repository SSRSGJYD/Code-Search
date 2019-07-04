# Questions on Code Search Literature

### A Survey of Machine Learning for Big Code and Naturalness

paper: [A Survey of Machine Learning for Big Code and Naturalness](https://arxiv.org/pdf/1709.06182.pdf)





### code2vec: Learning Distributed Representations of Code

paper: [code2vec: Learning Distributed Representations of Code](https://arxiv.org/pdf/1803.09473.pdf)

#### Question 1

In '*evaluation metric*' part of section 6 (Evaluation) on page 16, it is mentioned that models are evaluated by precision, recall and F1 score over *sub-tokens*. However, the method of generating sub-tokens is not mentioned here. I wonder how are method names and tags split into sub-tokens. 

#### Question 2

In '*element-wise soft-attention*' part of section 6.2, it is mentioned that different attention to different elements within a same context vector is of less meaning. I assume that there may be some points here. Different elements play different role in AST, and their importance in predicting tags may vary. It remains to further research on.



### Maybe Deep Neural Networks are the Best Choice for Modeling Source Code

paper: [Maybe Deep Neural Networks are the Best Choice for Modeling Source Code](https://arxiv.org/pdf/1903.05734.pdf)

#### Question 1

In section 7.3, it is mentioned that it is of no meaning to compare between different PLs, since training corpora varies in size and PLs vary in characteristic. So I am wondering how could the point that '*performance on C and Python is at least as good as Java*' be drawn, which is also mentioned in section 7.3.



### How To Create Natural Language Semantic Search For Arbitrary Objects With Deep Learning

website: https://towardsdatascience.com/semantic-code-search-3cd6d244a39c

#### Question 1

I am curious about the design of general architecture. This article learns sentence embeddings using LSTM and proposes another FC layer to learn mapping from the output of encoder to the embeddings. I think it is more straightforward to use the output of encoder as embeddings and propose a network to generate embeddings from docstring. I am not sure whether my idea makes sense.



### Deep API Learning

paper: https://guxd.github.io/papers/deepapi.pdf

#### Question 1

It is mention in section 4.2 that 2 RNNs are used in encoder, one forward and the other backward. There is no further justification of backward RNN in the paper, so I am wondering whether reverse RNN makes sense.