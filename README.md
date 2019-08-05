# Use-cases of Hugging Face's BERT

Hugging Faceが公開している[pytorch-transformers](https://github.com/huggingface/pytorch-transformers)のBERTを利用して、

- [言い換え生成](https://github.com/marucha80t/use-cases_of_bert/blob/master/lexical_substitution_with_bert.ipynb)
- [教師なし抽出型要約](https://github.com/marucha80t/use-cases_of_bert/blob/master/unsupervised_extractive_summarization_with_bert.ipynb)
を行う。

<br>


## 言い換え生成

ここでは、2種類の方法で言い換え生成を行う。

- BERTのマスク単語予測を利用した言い換え生成 
- 出力単語に制約を設けた言い換え生成

<br>


## 教師なし抽出型要約
BERTを用いて、入力文書及びその文書中に含まれる各文をそれぞれベクトル化する。
各文をEmbedRank++を用いてランキングし、上位n件を要約文として抽出する。

<br>


## 参考

- [https://github.com/huggingface/pytorch-transformers](https://github.com/huggingface/pytorch-transformers)
- [A Simple BERT-Based Approach for Lexical Simplification](https://arxiv.org/abs/1907.06226)
- [Conditional BERT Contextual Augmentation](https://arxiv.org/abs/1812.06705)
- [Simple Unsupervised Keyphrase Extraction using Sentence Embeddings](https://arxiv.org/abs/1801.04470)
