# kaggle
kaggle项目仓库

1.逻辑回归应用之Kaggle泰坦尼克之灾

泰坦尼克号问题之背景

豪华游艇倒了，大家都惊恐逃生，可是救生艇的数量有限，无法人人都有，副船长发话了『lady and kid first！』，所以是否获救其实并非随机，而是基于一些背景有rank先后的。

训练和测试数据是一些乘客的个人信息以及存活状况，要尝试根据它生成合适的模型并预测其他人的存活状况。

这是一个二分类问题，是我们之前讨论的logistic regression所能处理的范畴。

2.大学生助学金精准资助预测

 教育算法资格赛采用某高校2014、2015两学年的助学金获取情况作为标签，2013~2014、2014~2015两学年的学生在校行为数据作为原始数据，包括消费数据、图书借阅数据、寝室门禁数据、图书馆门禁数据、学生成绩排名数据，并以助学金获取金额作为结果数据进行模型优化和评价。
本次竞赛需利用学生在''2013/09~2014/09''的数据，预测学生在2014年的助学金获得情况；利用学生在''2014/09~2015/09''的数据，预测学生在2015年的助学金获得情况。虽然所有数据在时间上混合在了一起，即训练集和测试集中的数据都有''2013/09~2015/09''的数据，但是学生的行为数据和助学金数据是对应的。

（一）数据准备

精准资助主要集中反映在日常的消费数据中，我们先使用消费数据来构造特征数据和标记数据（答案数据）。

特征数据的一个要求是使用一行来描述一个对象，对象是不重复的，特征数据均为数字类型，不能出现其他类型，如果是字典类型，如性别男女也应该用0,1表示。

标记数据的要求是和特征数据一一对应，同样一行代表一个人（或物），标记需要使用整数形，一个数代表了一个分类。这里的专业叫法是标称型（变量），取值是有限的整数，不能是小数（分类再多总有个最大值的，小数就不知道是哪一类的了，呵呵）。和标称型对应的是数值型，如果标记的答案是数值型的，那就不是分类问题了，与之相对应的是机器学习的另一类应用回归
