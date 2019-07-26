# Questions on Code Search Literature

### A Survey of Machine Learning for Big Code and Naturalness

paper: [A Survey of Machine Learning for Big Code and Naturalness](https://arxiv.org/pdf/1709.06182.pdf)

#### Question 1

In 'Traceability' part of section 6.2 on page 27, generic text (e.g. from newspapers) and technical text in conversation environments(e.g. chatbots, Stack Overflow) are discriminated. I am wondering the criterion of discriminating two corpus, i.e., when to treat two corpus as same genre and when not to?

feedback: experiments are done in *When Deep Learning Met Code Search*

#### Question 2

In the second paragraph of section 7, the relationship between probabilistic programming and static code models:

> Probabilistic programming seeks to deploy programming language concepts to make it easier for developers to write new machine learning algorithms. Statistical code models seek to apply machine learning concepts to make it easier for developers to write new programs. In some sense, the two areas are dual to each other. That being said, one can certainly imagine completing the cycle and attempting to develop statistical code models for probabilistic programming languages.

As far as I know, probabilistic programming produces programs that simulating some probabilistic model, while statistical code models refer to the code. So I cannot understand why the two areas are dual to each other.

feedback: both concern probabilistic model and code



### code2vec: Learning Distributed Representations of Code

paper: [code2vec: Learning Distributed Representations of Code](https://arxiv.org/pdf/1803.09473.pdf)

#### Question 1

In '*evaluation metric*' part of section 6 (Evaluation) on page 16, it is mentioned that models are evaluated by precision, recall and F1 score over *sub-tokens*. However, the method of generating sub-tokens is not mentioned here. I wonder how method names and tags are split into sub-tokens. 

feedback: usually subtoken-splitting techniques include camel case, underscore; different PL may use different techniques.

#### Question 2

In '*element-wise soft-attention*' part of section 6.2, it is mentioned that different attention to different elements within a same context vector is of less meaning. I assume that there may be some points here. Different elements play different role in AST, and their importance in predicting tags may vary. It remains to further research on.

feedback: token names is not important here.



### Maybe Deep Neural Networks are the Best Choice for Modeling Source Code

paper: [Maybe Deep Neural Networks are the Best Choice for Modeling Source Code](https://arxiv.org/pdf/1903.05734.pdf)

#### Question 1

In section 7.3, it is mentioned that it is of no meaning to compare between different PLs, since training corpora varies in size and PLs vary in characteristic. So I am wondering how could the point that '*performance on C and Python is at least as good as Java*' be drawn, which is also mentioned in section 7.3.

feedback: experiment issues.



### How To Create Natural Language Semantic Search For Arbitrary Objects With Deep Learning

website: https://towardsdatascience.com/semantic-code-search-3cd6d244a39c

#### Question 1

I am curious about the design of general architecture. This article learns sentence embeddings using LSTM and proposes another FC layer to learn mapping from the output of encoder to the embeddings. I think it is more straightforward to use the output of encoder as embeddings and propose a network to generate embeddings from docstring. I am not sure whether my idea makes sense.

feedback: need further experiments.



### Deep API Learning

paper: [Deep API Learning](https://guxd.github.io/papers/deepapi.pdf)

#### Question 1

It is mention in section 4.2 that 2 RNNs are used in encoder, one forward and the other backward. There is no further justification of backward RNN in the paper, so I am wondering whether reverse RNN makes sense.

feedback: bidirectional RNN



### Deep Code Search

paper: [Deep Code Search](https://guxd.github.io/papers/deepcs.pdf)

#### Question 1

In this paper, method names and tokens in code snippet are split into sub-words by camel case, and code snippets come from github. Obviously, performance of this method rely heavily on coding style of code snippets, i.e., code snippets following camel case rule yield better result. I assume that may be other methods of subword-splitting may yield better performance here.

feedback: mentioned above.

#### Question 2

What is the advantage of bidirectional LSTM here compared to other RNNs?

feedback: bidirectional RNN generally works better.



### Aroma: Code Recommendation via Structural Code Search

paper: [Aroma: Code Recommendation via Structural Code Search](https://arxiv.org/pdf/1812.01158.pdf)

#### Question 1

In the second line from bottom of the first sub-section of section 3.2, page 6, there is a word called '*alpha-rename*'. I guess it may share similar meaning as rename or represent, but I am unable to find its meaning in the Internet. 

feedback: maybe similar meaning as $\alpha-equivalent$ .

#### Question 2

The evaluation part is not convincing enough, for example:  (1) in section 4.1, code snippets are selected manually, and (2) in both section 4.1 and 4.2, the criterion of judging whether recommended code matches expectation is ambiguous.

feedback: there is few objective metrics.



### When Deep Learning Met Code Search

paper: [When Deep Learning Met Code Search](https://arxiv.org/pdf/1905.03813.pdf)

#### Question 1

In section 4.4, an evaluation pipeline is introduced, which first determine a similarity threshold manually and applies it to evaluation. However, a small distance in vector space does not necessarily denotes a satisfying query result. Besides, use the mean value of correct results' distribution may loss correct query results and make evaluation results less convincing.

feedback: may be this could lead to some objective evaluation methods.