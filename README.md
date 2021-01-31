介绍
===
本次C3D模型用的是pytorch框架，我们在UCF101和HMDB51数据集上训练这些模型，本次实验以UCF101为实验对象。
---
文件介绍
===
>1.aesst (demo展示)<br>

>2.data(把下载好的UCF101数据集放在这里，输出的路径也可以放在这里)<br>
>>UCF101（数据集）<br>
>>ucf101（分成train,val,test）<br>
>>>train<br>
>>>val<br>
>>>test<br>

>3.dataloaders(数据载入，视频和图片与标签一一对应)<br>
>>ucf_labels(数据集标签)<br>
>>...<br>

>4.models(把下载好的预训练权重放这个位置)<br>

>5.network(网络模型)<br>
>>C3D_model<br>
>>...<br>

>6.run(保存训练出来的权重文件)<br>

>7.inference(预测文件)<br>

>8.mypath(路径文件)<br>

>9.train(训练文件)<br>

UCF101数据集下载地址：https://www.crcv.ucf.edu/data/UCF101/UCF101.rar<br>

从百度云下载预训练的模型，当前仅支持C3D的预训练模型。<br>
链接：https://pan.baidu.com/s/1iEkK5aV51UvG1Ul5kgUkHw  ，提取码：ch8y<br>

如果不想训练，单纯想拿来检测也可以，下载以下的文件，然后找到inference文件把相对于的路径改成你自己设置的路径，就可以实现。<br>
链接：https://pan.baidu.com/s/1DC_tF2lyVlvhNV9htunk4g ，提取码：3v4h <br>

操作流程
====
创建一个data文件夹，一个models文件夹，把下载的UCF101文件放在data文件内，把下载的预训练权重文件放在models文件内。然后修改mypath.py文件相关的路径，inference.py文件标签路径，然后运行train.py文件便可。
---

更详细的过程可以查看：<br>
CSDN:https://blog.csdn.net/weixin_47349091/article/details/113484959 <br>

知乎：https://zhuanlan.zhihu.com/p/348402763 <br>

本次实验是借鉴某位大神的github：https://github.com/jfzhang95/pytorch-video-recognition   在此表示感谢 <br>

以上均为原创，请勿转载，如需转载，请注明出处<br>

