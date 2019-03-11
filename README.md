# style-transfer

## 项目相关

这是[杨超越杯编程大赛](https://github.com/ccyyycy/ycy)风格迁移小组的repo，主要用于放置与比赛相关的通知与链接。

本项目是饱和式编程的一个尝试。从羊村长期的理念来讲：个人为主，追星为辅，所以建议大家优先完成自己的工作/任务，再考虑这个项目的内容。后续大家可以继续寻找有哪些可以完成的点，如果有时间+热情的同学，可以选择其中喜欢的项目进行训练/测试，最后再放上去展示。

[项目地址](https://ycy-cup-style-transfer.github.io)





## 整体框架

目前项目整体框架主要分为两个部分：第一部分是图像风格迁移模块，第二部分是基于ONNX.js将模型在浏览器上加载运行。

### 为什么是ONNX.js？

[Open Neural Network Exchange (ONNX)](https://onnx.ai) 是一种开放式的文件格式，用于存储训练好的模型，能够使不同人工智能框架能够采用相同的数据存储模型并产生交互。他由微软、亚马逊、Facebook、IBM等公司共同开发。目前官方支持ONNX模型的深度学习框架由：Caffe2，Pytorch，MXNet，ML.NET，TensorRT，CNTK，并且Tensorflow也非官方支持ONNX。因而它能极大程度地兼容不同的框架的使用，从而减少后期的工作量。

而[ONNX.js](https://github.com/Microsoft/onnxjs) 则是微软基于ONNX开发的一个javascript library，它能够将预训练好的ONNX模型在浏览器中加载并使用。

正式由于ONNX具有上面描述的性质，同时大家使用的框架各有不同，所以这里选择了ONNX.js。

目前已经使用Github Pages搭建了ONNX.js，由于进度问题，目前上面展示的模型暂时是两个分类模型，具体可点击[链接](https://ycy-cup-style-transfer.github.io)查看。

备注：这个部分



### 图像风格迁移模块

本项目风格迁移的形式不限，使用的模型不限，框架不限，大家可以寻找感兴趣的模型进行训练与测试。同时因为最终模型是通过网络传输加载到浏览器的，所以希望大家在能力范围内选择较轻量的backbone模型。

由于最终要求与ONNX.js进行对接，所以最后训练好的模型需要转化为ONNX格式，具体转化方式可以参照官方的tutoral或者相关的网络教程。

- [官方Tutorial](https://github.com/onnx/tutorials)



**备注：目前是否使用ONNX.js处于讨论中，也许会使用tf.js，大家可以先主要进行模型训练，暂时忽略迁移的问题。**



## 比赛进程

目前暂时处于任务组队阶段，组队时间截止到3月16日。

空闲时间相对多的朋友可以进行报名，没有报名的朋友也可以选择喜欢的项目进行训练。大家相互交流学习。





## 相关链接

此部分主要放置可选方案的论文以及github链接。

- [超越的图链](https://github.com/ccyyycy/ycy/blob/master/超越图链)



###相关学习链接 

建议可以先从资源汇总链接中的review paper开始学习，或者是后面的图像风格迁移三部曲/图像风格迁移简史开始，对整个领域有简单了解再选择感兴趣的内容展开深入学习。

- [图像风格迁移资源汇总](https://github.com/ycjing/Neural-Style-Transfer-Papers)
- [人像表情修改](https://zhuanlan.zhihu.com/p/40803572)
- [图像风格迁移简史](https://zhuanlan.zhihu.com/p/26746283)
- [图像风格迁移三部曲](https://zhuanlan.zhihu.com/p/36238178)



### 相关开源项目

建议可以直接通过github按关键词展开搜索，选择需要的内容即可。下面这几个链接是微信群上提到的，所以在此列出。

- [Style2Paint]( https://style2paints.github.io/README_zh)
- [Deep Photo Style Transfer](https://github.com/luanfujun/deep-photo-styletransfer)
- [Fast Photo Style Transfer](https://github.com/NVIDIA/FastPhotoStyle)



### 深度学习框架入门

- 建议参照框架的官方Tutorial文档，这是最有效的学习资料。

- 基本常见的框架在知乎都有关于如何入门的问题，选择高赞答案提供的某个链接使用即可，例如：

  - [新手如何入门Pytorch](https://www.zhihu.com/question/55720139)

  - [Tensorflow如何入门](https://www.zhihu.com/question/49909565)

    



## 已认领任务

此部分包含已认领任务以及认领人（格式：认领任务+认领人）， 一个任务可以多人认领。





## 备注

- 关于某个项目的讨论，可以通过微信群或者issue进行。

- 可以通过fork&pull request形式进行贡献。

  



