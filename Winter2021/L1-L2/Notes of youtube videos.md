
# Lecture 1 - Intro & Word Vectors

## Notes

用dot product来计算word similarity是一种很常见的方法。 0\*0不影响结果，+ \* -减少结果，同号相成增大结果。  结果越大，说明两个词越相似



## Questions

softmax计算的时候，负数的dot product取了exp会变成正数，那不是相当于不相似的都变大了？不会，exp是整体单调递减，负数取完exp不会比正数大



# Lecture 2 - Neural Classifiers

SGD相比完全的plain gradient descent，不仅迭代速度快，效果也更好。 后者有点反直觉（counter intuitive）
>not only a performance hack, but also have a better job

word vector可以只搞一个，为啥要分成center word和outside word俩？  梯度下降多变量求导逻辑更清晰

在NLP中，评估word vector承载的知识是很重要的一部分（evaluate knowledge that things have）

manning很诚实啊：从GloVe诞生7年后回望，evaluation并不比word2vec好。数字好是因为用的数据好

## Questions
negative sampling为啥只取了一个positive sample？ 视频中间有学生提问，回答也没太听懂

GloVe 也没太懂？ 57:50有同学提问，教授有再解答一遍



# 术语表
[hypernym（上位词）](https://zh.m.wikipedia.org/zh/%E4%B8%8A%E4%B8%8B%E4%BD%8D%E9%97%9C%E4%BF%82) 语义关系树中的上下位关系。比如 浣熊科 是 熊猫 的上位词

denotational semantics（指称语义） symbol表达含义

distributional semantics  word2vec的核心思想，使用word contexts来表达word的含义

token/type. token是一个具体的词，types是一类词的example，代表了词的含义

**word vectors**: are also called **word embeddings** or **(nerual) word representations**. They are
a distributed representation

unigram distribution: 词在corpus中出现的频率

singular value decomposition 奇异值分解