what metrics do you use to evaluate the pretrained models?
- perplexity for general purpose
- tons of evaluation tasks built by the community


the encoder has bidirectional information, but decoder only has unidirection


BERT
- pretrain on 64 TPU for 4 days, but fine-tuning can be done on only one GPU. This maybe the one of reasons that it successed.