
# Video
用dot product来计算word similarity是一种很常见的方法。 0\*0不影响结果，+ \* -减少结果，同号相成增大结果。  结果越大，说明两个词越相似


## Q&A

- Q: softmax计算的时候，负数的dot product取了exp会变成正数，那不是相当于不相似的都变大了？
- A: 不会，exp是整体单调递减，负数取完exp不会比正数大



## 术语表
[hypernym（上位词）](https://zh.m.wikipedia.org/zh/%E4%B8%8A%E4%B8%8B%E4%BD%8D%E9%97%9C%E4%BF%82) 语义关系树中的上下位关系。比如 浣熊科 是 熊猫 的上位词

denotational semantics（指称语义） symbol表达含义

distributional semantics  word2vec的核心思想，使用word contexts来表达word的含义

token/type. token是一个具体的词，types是一类词的example，代表了词的含义

**word vectors**: are also called **word embeddings** or **(nerual) word representations**. They are
a distributed representation


# cs224n-2019-notes01-wordvecs1

## Q&A
- Q: P8 cross entropy和CBOW最终的objective function有啥关系？