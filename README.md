# Knowledge encoding by examples of Word2Vec and LLM training

This repository contains code for training a list of language models:
- Word2Vec: class `SkipGramNegSampling`. Embedding model trained on 150mil pairs of text tokens subsampled from text8 dataset. SkipGram method with negative sampling was used as described in the original [paper](https://arxiv.org/abs/1402.3722).
- MLP: class `MLPLanguageModel`. 2-layers MLP trained on the same dataset and using pretrained embeddings. There's a simple version of this model and a version utilizing LayerNorm for better scaling of the learned features distribution.

Weights for both models are stored here: https://huggingface.co/ruslandev/knowledge-encode
