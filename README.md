#2021-Sodic-water  A、B榜top10交流方案
#基本思路
#1.EDA,探索训练集数据规律
#2.stage1，通过滑动窗口、滞后以及相关时间特征进行预测，
#使用daybyday的预测方法进行预测，每次将预测所得的值加入到训练集，
#构建动态训练测试集进行预测
#3.stage2，stage1会导致误差累加，故stage1只预测了2020年11月到12月，
#stage2单单从时间特征出现进行预测，主要涉及的方法有prophet、
#树模型(kfold、holdout），并融入一定的规则进行上分

