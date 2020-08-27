# BIO-sequence-label
BIO模式的-命名实体识别等任务的序列标注工具<br>
[对应的CSDN博客链接：](https://blog.csdn.net/broccoli2/article/details/103561708)<br>

笔者研究方向为NLP知识抽取，做实体识别实验过程中需要对训练数据进行标注。</br>
##处理流程如下：
（1）使用规则提取出要标注的实体，如“盈方微电子股份有限公司”，将提取出的实体保存至word_dict.txt文件中作为词典，并为每一类实体自行设计创建一类标签。</br>
（2）将待标注样本处理成一行，也就是一行是一个样本。
（3）根据自己需要选择标注好的文件的格式，可以是“taken空格labe”在一个文件中，也可以将token和label分开来。</br>

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



有问题可提issues。觉得有用的话，欢迎star~




