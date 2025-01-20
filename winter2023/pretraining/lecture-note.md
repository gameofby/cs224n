what metrics do you use to evaluate the pretrained models?
- perplexity for general purpose
- tons of evaluation tasks built by the community


the encoder has bidirectional information, but decoder only has unidirection


BERT
- pretrain on 64 TPU for 4 days, but fine-tuning can be done on only one GPU. This maybe the one of reasons that it successed.


From word embedding to pretraining method: a same word has different meanings in different context, but the word embedding is fixed after word pretraining.

GPT3 just trained on more data with Decoder architecture(language model), it suddenly emerges from examples learning capability from what you provide within their contexts.



paradigm from a paper [Don't Stop Pretraining](https://arxiv.org/pdf/2004.10964)
1. pretrain on big corpus
2. pretrain on the data of your own tasks without labels
3. fine-tuning on the data of your tasks with labels