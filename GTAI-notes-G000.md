# GTAI-G000工作日记

## 2018-9-10

1. 查看LYB数据问题，训练。  60%，训练仍有问题。
2. 查看个人公积金社保缴费事宜。

## 2018-9-11

1. LYB提交一个0.027的版本：网络用Xception，16个属性
2. checkle test，30%

## 2018-9-12

1. check test 完成；吻合
2. 检查发现某些属性，如动物分类效果非常差
3. 收到摄像头、舵机、小车几份快递
4. 和童嘉老师确定，下周四上午去紫金小镇注册公司

## 2018-9-13

1. 针对某些类的效果比较差的问题尝试了以下手段
   1. 尝试，没有成效的
      1. 分析训练图像数据
      2. 降低初始学习率
      3. 将2类softmax改成sigmoid
      4. 将训练图片数据除255归一
      5. 在最后一层fc前加dropout(0.5)
   2. 有待继续尝试
      1. 用一个更小的网络
      2. 进行数据增强
      3. 搜相关工作
2. 将ipynb的代码函数化，文件化，转成py格式
3. 掌握tmux分屏用法

## 2018-9-14

1. 将测试数据中的十个之前判定是未知类的，和训练数据中的类绑定。
2. 调整每个类的属性值
3. 用keras训练190类的分类器（14日晚~15日晨，用笔记本）

## 2018-9-15

1. 显示训练-测试相似度矩阵，发现有些相似度很怪异，发现和调整属性标注里面存在的歧义标注
2. 测试190类分类器在所有训练图片上的准确率约为96% 

