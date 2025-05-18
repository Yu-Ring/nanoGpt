# 从头训练一个GPT

## 模型架构：
Tokenization使用字符级分词，未使用分词算法。

Embedding和Position Encoding都是仅映射到指定嵌入维度向量进行训练。

Attention沿用经典Transformer：pre-norm->self-attention->残差链接->pre-norm->FFN->残差链接

MHA：使用4个多头注意力。

## 评估方式：
模型的评估方式计算为平均损失，每个loss通过交叉熵计算得到。


