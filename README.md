# BIO-sequence-label
BIO模式的-命名实体识别等任务的序列标注工具<br>
[对应的CSDN博客链接：](https://blog.csdn.net/broccoli2/article/details/103561708)<br>

笔者研究方向为NLP知识抽取，做实体识别实验过程中需要对训练数据进行标注。</br>
(1)先使用jieba分词对原文本进行分词和pos词性标注。</br>
(2)然后基于pos词性标注抽取出文本中的公司名、证券、基金名称（这部分也可以使用正则方法）等，保存到word_dict.txt中作为词典。</br>
(3)然后基于该词典对原文本中进行的数据进行标注。</br>
INT与BON为文本对应的标签。</br>
占位词 NONE，这一行必须要有，作为词典的停止关键词</br>

word_dict.txt文件如下图所示：<br>
![标注词典](image/word_dict.png)<br>



标注好的数据如下图所示。<br>
启 B-INT<br>
迪 I-INT<br>
设 I-INT<br>
计 I-INT<br>
集 I-INT<br>
团 I-INT<br>
股 I-INT<br>
份 I-INT<br>
有 I-INT<br>
限 I-INT<br>
公 I-INT<br>
司 I-INT<br>
于 O <br>
今 O<br>
日 O<br>



有问题可提issues。




