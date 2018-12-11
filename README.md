# spam-message-classifier 中文垃圾短信分类器
This a a project from Web Data Mining course of UCAS

使用jieba分词包及多种机器学习分类法进行中文文本分类

国科大网络数据挖掘课程大作业

本项目基于python中文分词包jieba进行分词，使用了Logistic Regression, GDBT, Forest Classifier等分类器进行分类，达到了较好的效果

jieba分词包的使用参考：https://github.com/fxsjy/jieba

## 环境

- Python 2/3
- pandas
- numpy
- jieba
- scikit-learn
- PHP
## 数据集

使用老师给的带有标签的数据集进行训练与验证

使用老师给的不带有标签的数据集进行测试

数据集划分：

- 训练集：50000
- 测试集：10000

## 数据预处理

- data_loading: 加载数据
- split_word: 对所有数据利用jieba分词并保存
- vector_word: 生成词向量矩阵并保存

