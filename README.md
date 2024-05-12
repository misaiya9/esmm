# 一、esmm模型的原理介绍
https://arxiv.org/abs/1804.07931
Entire Space Multi-Task Model: An Effective Approach for Estimating Post-Click Conversion Rate
# 二、脚本介绍  
1、test.py 构造tfrecords数据，数据是我瞎造的，为了跑通并调试脚本。  
2、esmm.py 训练esmm模型  
3、numeric_column.py 练习tf.feature_column API和模型无关，不感兴趣，可忽略。
# 三、脚本使用：  
1、运行test.py构造data.tfrecord数据  
2、运行esmm.py文件  

# 四、训练代码
1、 模型的两个loss是ctr loss 和 ctcvr loss 为什么不用 除法（除0和天然偏大 方差问题吧？）
2、essmm模型的一个天然缺陷： no click but pay .这个是这个模型天然cvr 偏大的原因。
