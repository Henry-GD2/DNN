# DNN
minist
通过神经网络算法处理手写数字辨识问题

一些要点：
# 损失函数的选择

本类题目是概率分类问题，使用的函数，输出是一个10维的概率分布，可以写成如下形式

 model.add(Dense(units=10,activation='softmax'))
# 损失函数选择交叉熵
model.compile(loss='categorical_crossentropy',optimizer=Adam(),metrics=['accuracy'])

accuracy代表以准确率为最终结果好坏的判断标准

loss='categorical_crossentropy'是使用交叉熵作为损失函数，在概率分类问题上一般用这个比较好
