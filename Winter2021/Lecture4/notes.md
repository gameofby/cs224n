# lecture and official notes

两种语言结构的观点:

1.Constituency = phrase structure grammar = context-free grammars (CFGs)

words -> nested phrases

2.Dependency structure
大概从2000年开始，NLP研究者主要使用dependency grammar

英语中有很多prepositional phrases，很容易造成歧义。寻找head的基本原则是，不造成crossing attachment
![[Screenshot 2023-07-27 at 09.56.21.png]]
在编程语言的编译设计中，通常是不存在歧义的。不像自然语言，需要听者来消歧

projectivity：arcs之间不存在交叉。  但dependency theory是允许出现一些交叉的
>dependency theory normally does allow non-projective structures to account for displaced constituents



# PyTorch Tutorial Session

questions
- uniform distribution
- normal distribution

