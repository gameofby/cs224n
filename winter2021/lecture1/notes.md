
# Lecture

WordNet: 类属词典，包含同义词/上位词等，是早期nlp用来记录word meaning的手段
缺点
1. 缺乏对同义词间的细微差别的记录
2. 老词新意、新词等，人工很难维持up-to-date
3. 不能用于计算准确的word similarity

one-hot，视words为离散符号
缺点：vertor正交，无法计算word相似度




用dot product来计算word similarity是一种很常见的方法。 0\*0不影响结果，+ \* -减小结果，同号相乘增大结果。  结果越大，说明两个词越相似


## Q&A

![[Pasted image 20230802095917.png]]

![[Pasted image 20230802100059.png]]

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

- Q: Hierarchical Softmax的实现细节？