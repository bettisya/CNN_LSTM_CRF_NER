# CNN_LSTM_CRF_NER
neural network architecture to do named entity recognition

### 1. 模型架构
    底层CNN提取character embedding + 预训练的Glove word embedding
    中间bi-LSTM
    上层CRF进行标注
    
### 2. 框架
    theano + lasagne
    
### 3. NER标注
    1）输入格式：参考data/test.txt，文档开头#begin doc_id num_of_sentences, 每个token一行，每句之间以空行隔开；
    
    2) 测试结果：./test.sh
    
    3) 结果处理：结果处理相关函数都在divide_text.py文件中
    
### 4. 训练
    1）文本格式与3中相同
    2）参照run2.sh
      
