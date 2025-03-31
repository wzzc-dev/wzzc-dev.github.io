---
title: 算丰学院-LLM的概念与实践-LLM：世界知识的无损压缩
date: '2025-03-24 15:54:08'
updated: '2025-03-31 15:53:13'
permalink: >-
  /post/suanfeng-academy-concept-and-practice-of-llm-llm-lossless-compression-of-world-knowledge-zhftfu.html
comments: true
toc: true
---



# 算丰学院-LLM的概念与实践-LLM：世界知识的无损压缩

LM (language model)

统计语言模型(SLM)  
Statistical language models

* N 元模型

神经语言模型(NLM)  
Neural language models

* 前馈神经网络语言模型

  * 每个词用低维稠密向量表示,提升模型泛化能力。  
    假定,测试集中有一句话"猫|在|厨房|吃|鱼",训练集中没有出现过,但存在  
    "狗|在|卧室|吃|肉",由于{"猫","厨房","卧室"},{"鱼","肉"}语义相似  
    模型可以推断"猫|在|厨房|吃|鱼"是一句话的概率很高。
* 循环神经网络语言模型(RNNLM),引入循环结构,解决长序列依赖问题
* ‍

预训练语言模型(PLM)  
Pre-trained language models

大规模语言模型(LLM)  
Large language models

## LLM定义

LLM (Large Language Model)

LLM是一种基于深度学习的大型自然语言处理模型,通过大规模数据集的预训练和微调过程学习语言的模式和规律,具有强大的文本生成和理  
解能力,广泛应用于文本生成,智能对话等多个领域。

Pre-train:

* 从巨大的数据集中进行无监督训练
* 学习一般的语言模式和表征

Fine-tune:  
根据特定的任务和更小一点的数据集训练与微调

金融:情报分析,投资建议  
教育:个性化学习,辅助教学  
医疗:疾病诊断,药物研发  
艺术:自动生成作品,创意支持

‍

## Transformer模型

3.1 Attention机制

### 传统RNN模型

LSTM (Long-Short Term Memory)长短期记忆

GRU(Gate Recurrent Unit)门控循环单元

缺陷

顺序计算,模型的并行能力较差

长期依赖问题

### 注意力机制(attention)

* 神经网络中模仿人类认知注意力的技术
* 灵活性
* 可以从序列中任何先前点的状态中提取信息
* attention机制与FNN前馈神经网络的结合

可以在运行时改变权重

### 对知识的无损压缩

‍
