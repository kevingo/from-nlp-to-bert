# From NLP to Bert

In this repositoy, I will make some notes on the introductory from NLP to Bert.

## Agenda

- Introduction to NLP
  - Tradition NLP (WordNet / one-hot encoding)
  - lexical analysis
  - Syntactic analysis
  - Semantic analysis
- Basic NLP
  - tf-idf
  - bag-of-word (BoW)
  - n-gram language model
  - limitation of BoW and n-gram language model
- Deep NLP
  - Word2Vec
  - RNN
  - Sequence-to-sequence
  - Attention Model
  - Transformer (self-attention)
    - Transformer is a seq-to-seq model with self-attention layer
    - 用來改良 RNN 不容易平行化的缺點
    - 基本上原本用 RNN 的架構，都可以換成 self-attention 的 layer 來取代
    - 在 self-attention 的原本機制中，沒有位置 (position) 的資訊
      - 引入 positional encoding 機制：每一個 input vector 都會 append 上一個位置資訊的 vector，接著做 self-attention
- Bert
  - Bert introduction
    - Encoder of transformer
  - 訓練 Bert 的方法
    - Approach 1：Masked LM
    - Approach 2：Next sentence prediction
  - Bert on our work
- Conclusion


## Resources
- [從自然語言處理到文字探勘](https://www.slideshare.net/YiShinChen1/ss-104503736)：Comprehensive introduction from NLP to text mining.
- [CS224n: Natural Language Processing with Deep Learning](http://web.stanford.edu/class/cs224n/)
  - [The probability of a sentence? Recurrent Neural Networks and Language Models](http://web.stanford.edu/class/cs224n/slides/cs224n-2019-lecture06-rnnlm.pdf)：Introduction from n-gram language model to RNN
  - [Machine Translation, Sequence-to-sequence and Attention](http://web.stanford.edu/class/cs224n/slides/cs224n-2019-lecture08-nmt.pdf)
- [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf)：The original paper about Word2Vec proposed by Tomas Mikolov. 
- [Seq2seq pay Attention to Self Attention](https://medium.com/@bgg/seq2seq-pay-attention-to-self-attention-part-1-%E4%B8%AD%E6%96%87%E7%89%88-2714bbd92727)
- [矢量語義——從TF-IDF到Word2Vec你所需要知道的一切](https://blog.csdn.net/stupid_3/article/details/83184807)：Nice illustration about Word2Vec
- [The Illustrated BERT, ELMo, and co. (How NLP Cracked Transfer Learning)](http://jalammar.github.io/illustrated-bert/)
- [Transformer by 李宏毅](https://www.youtube.com/watch?v=ugWDIIOHtPA)
