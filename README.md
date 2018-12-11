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

> 部分训练数据
```
0	商业秘密的秘密性那是维系其商业价值和垄断地位的前提条件之一
1	南口阿玛施新春第一批限量春装到店啦         春暖花开淑女裙、冰蓝色公主衫   气质粉小西装、冰丝女王长半裙、   皇
0	带给我们大常州一场壮观的视觉盛宴
0	有原因不明的泌尿系统结石等
0	23年从盐城拉回来的麻麻的嫁妆
0	感到自减肥、跳减肥健美操、
1	感谢致电杭州萧山全金釜韩国烧烤店，本店位于金城路xxx号。韩式烧烤等，价格实惠、欢迎惠顾【全金釜韩国烧烤店】
0	这款UVe智能杀菌机器人是扫地机的最佳伴侣
1	一次价值xxx元王牌项目；可充值xxx元店内项目卡一张；可以参与V动好生活百分百抽奖机会一次！预约电话：xxxxxxxxxxx
0	此类皮肤特别容易招惹粉刺、黑头等
```
> 部分测试数据
```
.x月xx日推出凭证式国债x年期x.xx.xx%，x年期x.xx%到期一次还本付息。真情邮政，为您竭诚服务！  咨询电话xxxx-xx
x强度等级水泥的必要性和可行性进行深入研究
Don’tSellaProduct
以上比赛规则由江苏科技大学教职工摄影协会负责解释
坐12个小时飞机身体已经疲惫不堪
```
## 数据预处理

- data_loading: 加载数据
- split_word: 对所有数据利用jieba分词并保存
- vector_word: 生成词向量矩阵并保存

