<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/tensorflow_nlp.png" height='100'>

---
#### Why This Project?

* Good TensorFlow practice using [tf.data](https://www.tensorflow.org/api_docs/python/tf/data) and [tf.estimator](https://www.tensorflow.org/api_docs/python/tf/estimator) interfaces

* Lots of clean Jupyter Notebooks

---
#### Contents
* [Word Embedding（词向量）](https://github.com/zhedongzheng/finch#word-embedding%E8%AF%8D%E5%90%91%E9%87%8F)
* [Text Classification（文本分类）](https://github.com/zhedongzheng/finch#text-classification%E6%96%87%E6%9C%AC%E5%88%86%E7%B1%BB)
* [Text Generation（文本生成）](https://github.com/zhedongzheng/finch#text-generation%E6%96%87%E6%9C%AC%E7%94%9F%E6%88%90)
* [Text Matching（文本匹配）](https://github.com/zhedongzheng/finch/blob/master/README.md#text-matching%E6%96%87%E6%9C%AC%E5%8C%B9%E9%85%8D)
* [Sequence Labelling（序列标记）](https://github.com/zhedongzheng/finch#sequence-labelling%E5%BA%8F%E5%88%97%E6%A0%87%E8%AE%B0)
* [Sequence to Sequence（序列到序列）](https://github.com/zhedongzheng/finch#sequence-to-sequence%E5%BA%8F%E5%88%97%E5%88%B0%E5%BA%8F%E5%88%97)
* [Question Answering（问题回答）](https://github.com/zhedongzheng/finch/blob/master/README.md#question-answering%E9%97%AE%E9%A2%98%E5%9B%9E%E7%AD%94)
* [Knowledge Graph（知识图谱）](https://github.com/zhedongzheng/finch#knowledge-graph%E7%9F%A5%E8%AF%86%E5%9B%BE%E8%B0%B1)
* [TensorFlow Project Template（TensorFlow 项目模版）](https://github.com/zhedongzheng/finch/blob/master/README.md#tensorflow-project-templatetensorflow-%E9%A1%B9%E7%9B%AE%E6%A8%A1%E7%89%88)

---
#### Requirements 
* Python 3 and [Jupyter Notebook](http://jupyter.org/) are required

    ```
    (CPU User) $ pip3 install tensorflow sklearn scipy bunch tqdm
    
    (GPU User) $ pip3 install tensorflow-gpu sklearn scipy bunch tqdm
    ```
---

#### Word Embedding（词向量）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_6.png" height='100'>

* Penn Treebank（PTB 语料库）

    * Skip-Gram &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/word2vec_skipgram.ipynb)

    * CBOW &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/word2vec_cbow.ipynb)

#### Text Classification（文本分类）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_2.png" height='100'>

* IMDB Movie Reviews Sentiment（电影评论情感分类）

    * Text-CNN &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/concat_conv_1d_text_clf_imdb_test.ipynb)

    * Bi-RNN &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/rnn_text_clf_imdb_test.ipynb)

    * Self-Attention &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/only_attn_text_clf_imdb_test.ipynb)

    * TF-IDF + LR &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/dnnlinear_tfidf_imdb_test.ipynb)

#### Text Generation（文本生成）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_5.png" height='100'>

* Language Model（语言模型）

    * RNN LM &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/char_rnn_beam_test.ipynb)

    * Self-Attention LM &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/self_attn_lm_test.ipynb)

    * Character Aware LM &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/cnn_rnn_text_gen_test.ipynb)

* Generative Modelling（生成式建模）

    * VAE &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/tree/master/nlp-models/tensorflow/vae/train.ipynb)
    
    * Controlled VAE &nbsp; &nbsp; [Folder](https://github.com/zhedongzheng/finch/tree/master/nlp-models/tensorflow/toward_control)

* Speech Recognition（语音识别）

    * CTC &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/asr/train.ipynb)

#### Text Matching（文本匹配）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_10.jpeg" height='200'>

* Movielens（电影推荐）

    * User-Item Matching &nbsp; &nbsp; [Folder](https://github.com/zhedongzheng/finch/tree/master/nlp-models/tensorflow/movielens)

#### Sequence Labelling（序列标记）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_4.jpg" height='100'>

* POS Tagging（词性识别）

    * Bi-RNN + CRF &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/pos_birnn_crf_test.ipynb)

    * CNN + CRF &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/cnn_seq_label_pos_test.ipynb)

* Chinese Segmentation（中文分词）

    * Bi-RNN + CRF &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/chseg_birnn_crf_test.ipynb)

    * CNN + CRF &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-data-api/cnn_seq_label_chseg_test.ipynb)

#### Sequence to Sequence（序列到序列）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/decoration_1.png" height='100'>

* Learning to Sort（机器学习字母的排序）

    * Seq2Seq + Attention + Beam-Search &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/seq2seq_ultimate_test.ipynb)

    * Pointer Network &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/tf-estimator/pointer_net_test.ipynb)

    * Transformer &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/attn_is_all_u_need/train_letters.ipynb)
    
* Learning to Dialog（机器对话）

    * Transformer &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/attn_is_all_u_need/train_dialog.ipynb)
        
#### Question Answering（问题回答）
<img src="https://github.com/zhedongzheng/finch/blob/master/nlp-models/assets/dmn-details.png" height='100'>

* Facebook bAbI（逻辑回答）

    *  End-to-End Memory Network &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/end2end_mn/train.ipynb)

    *  Dynamic Memory Network &nbsp; &nbsp; [Notebook](https://nbviewer.jupyter.org/github/zhedongzheng/finch/blob/master/nlp-models/tensorflow/dmn/train.ipynb)

#### Knowledge Graph（知识图谱）
* [Course Notes](https://github.com/zhedongzheng/finch/blob/master/notes/kg/notes.md)

#### TensorFlow Project Template（TensorFlow 项目模版）
* [TF Estimator Template](https://github.com/zhedongzheng/finch/tree/master/templates/tf_estimator_template)

* [TF Dataset Template](https://github.com/zhedongzheng/finch/tree/master/templates/tf_dataset_template)

#### Resource（资源）
* Books（教材）
    
    * [NLP - Jacob Eisenstein](https://github.com/jacobeisenstein/gt-nlp-class/tree/master/notes)

* Applications（应用）

    * [NLP在百度的应用（13年）](https://github.com/zhedongzheng/finch/blob/master/notes/application/baidu_nlp.pdf)
