# Video
SGD相比完全的plain gradient descent，不仅迭代速度快，效果也更好。 后者有点反直觉（counter intuitive）
>not only a performance hack, but also have a better job

word vector可以只搞一个，为啥要分成center word和outside word俩？  梯度下降多变量求导逻辑更清晰

在NLP中，评估word vector承载的知识是很重要的一部分（evaluate knowledge that things have）

manning很诚实啊：从GloVe诞生7年后回望，evaluation并不比word2vec好。当时结果好是因为用的数据好（wikipedia）


## HW2
sigmoid替代了softmax，因为用更少的计算量可以起到类似的效果。不像softmax，denominator要扫一遍vocabulary全集


## Q&A
- Q（P15）: negative sampling的objective function？ 视频中间有学生提问(25:19)，回答也没太听懂
- A: [cs224n-2019-notes01-wordvecs1](obsidian://open?vault=cs224n&file=Winter2021%2FLecture1%2Fcs224n-2019-notes01-wordvecs1.pdf) 4.4小节的解释比较易懂

- Q: GloVe 的objective function也没太懂？ 57:50有同学提问，教授有再解答一遍
- 



## 术语表

unigram distribution: 词在corpus中出现的频率

singular value decomposition 奇异值分解

