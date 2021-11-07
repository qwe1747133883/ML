# 朴素贝叶斯分类器在中文垃圾邮件分类上的实现
## 介绍
朴素贝叶斯算法是一种简单有效的分类算法，被广泛运用在文本分类与垃圾邮件、信息过滤中。

## 利用朴素贝叶斯实现中文垃圾邮件过滤

我们通过以下步骤来实现一个现实可用的垃圾邮件过滤器
1. 根据数据集产生训练集与测试集
2. 提取文本数据，对文本进行分词，过滤停用词、数字、特殊符号。
3. 统计词汇，产生词典
4. 训练分类器


### 数据集
使用 [滑铁卢大学](https://plg.uwaterloo.ca/~gvcormac/treccorpus06/) 提供的中文邮件数据集，数据集共有超过60000封中文邮件，并且已经做好了标注。停用词列表使用 github 上整理的停用词库，[中文停用词](https://github.com/dongxiexidian/Chinese/blob/master/stopwords.dat) 。我们选用其中30000封中文邮件，29400封用作训练集，600用作测试集。


### 实验结果
最后统计得出对测试集的预测准确率高达0.9766666666666667。
