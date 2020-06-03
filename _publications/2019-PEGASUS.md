---
title: "PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization"
collection: publications
permalink: /publication/2019-PEGASUS
date: 2019-12-18
venue: 'Thirty-seventh International Conference on Machine Learning (ICML 2020)'
paperurl: 'https://arxiv.org/abs/1912.08777'
citation: '<b>Jingqing Zhang</b>, Yao Zhao, Mohammad Saleh, Peter J. Liu. "PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization." Thirty-seventh International Conference on Machine Learning (ICML). 2020. '
authors: '<b>Jingqing Zhang</b>, Yao Zhao, Mohammad Saleh, Peter J. Liu'
---

Paper Link: [arXiv](https://arxiv.org/pdf/1912.08777.pdf) 

Code is available on Github: [https://github.com/google-research/pegasus](https://github.com/google-research/pegasus)

## Abstract
Recent work pre-training Transformers with self-supervised objectives on large text corpora has shown great success when fine-tuned on downstream NLP tasks including text summarization. However, pre-training objectives tailored for abstractive text summarization have not been explored. Furthermore there is a lack of systematic evaluation across diverse domains. In this work, we propose pre-training large Transformer-based encoder-decoder models on massive text corpora with a new self-supervised objective. In PEGASUS, important sentences are removed/masked from an input document and are generated together as one output sequence from the remaining sentences, similar to an extractive summary. We evaluated our best PEGASUS model on 12 downstream summarization tasks spanning news, science, stories, instructions, emails, patents, and legislative bills. Experiments demonstrate it achieves state-of-the-art performance on all 12 downstream datasets measured by ROUGE scores. Our model also shows surprising performance on low-resource summarization, surpassing previous state-of-the-art results on 6 datasets with only 1000 examples.

## State-of-the-art Results on 12 Datasets

| Dataset | C4 | HugeNews | Mixed & Dynamic|
| ---- | ---- | ---- | ----|
| xsum | 45.20/22.06/36.99 | 47.21/24.56/39.25 | 47.60/24.83/39.64|
| cnn_dailymail | 43.90/21.20/40.76 | 44.17/21.47/41.11 | 44.16/21.56/41.30|
| newsroom | 45.07/33.39/41.28 | 45.15/33.51/41.33 | 45.98/34.20/42.18|
| multi_news | 46.74/17.95/24.26 | 47.52/18.72/24.91 | 47.65/18.75/24.95|
| gigaword | 38.75/19.96/36.14 | 39.12/19.86/36.24 | 39.65/20.47/36.76|
| wikihow | 43.07/19.70/34.79 | 41.35/18.51/33.42 | 46.39/22.12/38.41 *|
| reddit_tifu | 26.54/8.94/21.64 | 26.63/9.01/21.60 | 27.99/9.81/22.94|
| big_patent | 53.63/33.16/42.25 | 53.41/32.89/42.07 | 52.29/33.08/41.66 *|
| arxiv | 44.70/17.27/25.80 | 44.67/17.18/25.73 | 44.21/16.95/25.67|
| pubmed | 45.49/19.90/27.69 | 45.09/19.56/27.42 | 45.97/20.15/28.25|
| aeslc | 37.69/21.85/36.84 | 37.40/21.22/36.45 | 37.68/21.25/36.51|
| billsum | 57.20/39.56/45.80 | 57.31/40.19/45.82 | 59.67/41.58/47.59|

The "Mixed & Dynamic" model has the following changes:
- Trained on both C4 and HugeNews (dataset mixsure is weighted by their number of examples). 
- Trained for 1.5M instead of 500k (we observe slower convergence on pretraining perplexity).
- The model dynamicly choose 15%-45% important sentences to generate
- Importance sentences are sampled instead of using a fixed strategy (This is done by adding a 20% noise to importance scores.) 
- The sentencepiece tokenizer is updated to be able to encode newline character.


(*) The numbers of wikihow and big_patent datasets are not comparable because of change in tokenization and data:
- Wikihow dataset contains newline characters which is useful for paragraph segmentation, the C4 and HugeNews model's sentencepiece tokenizer doesn't encode newline and loose this information.
- We update the BigPatent dataset to preserve casing, some format cleanings are also changed, please refer to change in TFDS.


## Citation
```
@misc{zhang2019pegasus,
    title={PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization},
    author={Jingqing Zhang and Yao Zhao and Mohammad Saleh and Peter J. Liu},
    year={2019},
    eprint={1912.08777},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
```
