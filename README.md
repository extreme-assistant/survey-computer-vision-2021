# survey-computer-vision（2021-2022）

## 计算机视觉综述论文分方向整理（持续更新）<br>

## 目录
* [目标检测](#1)<br>
* [图像分割](#2)<br>
* [医学影像](#3)<br>
* [目标跟踪](#4)<br>
* [人脸](#5)<br>
* [Attetion/Transformer](#6)

<br><br>

<a name="1"/>

## 目标检测（object detection）



<br><br>

<a name="2"/>

## 图像分割

### 全景分割

[1]  Panoptic Segmentation: A Review<br>
[paper](https://arxiv.org/abs/2111.10250) | [code](https://github.com/elharroussomar/Awesome-Panoptic-Segmentation)<br>
作者：Omar Elharrouss,Somaya Al-Maadeed,Nandhini Subramanian,Najmath Ottakath,Noor Almaadeed,Yassine Himeur<br>
机构：Qatar University<br>
摘要：用于视频分析的图像分割在智能城市、医疗保健、计算机视觉以及遥感应用等不同研究领域发挥着重要作用。在这方面，最近已经投入了大量精力来开发新的细分策略；最新的突出成就之一是全景分割。全景分割是语义分割和实例分割融合的结果。明确地说，目前正在研究全景分割，以帮助获得视频监控、人群计数、自动驾驶、医学图像分析等图像场景的更细致的知识，以及对一般场景的更深入理解。为此，我们在这篇论文中首次全面回顾了作者所知的现有全景分割方法。因此，根据所采用的算法、应用场景和主要目标的性质，对现有的全景技术进行定义良好的分类。此外，还讨论了使用全景分割通过伪标记对新数据集进行注释。接下来，进行了消融研究，从不同角度了解全景方法。此外，还讨论了适用于全景分割的评估指标，并对现有解决方案的性能进行了比较，以告知最新技术并确定其局限性和优势。最后，阐述了主题技术面临的当前挑战以及近期吸引大量兴趣的未来趋势，这可以作为即将进行的研究的起点。<br>
- [方法与数据集描述1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovitsn12j314w0zknet.jpg) | [方法与数据集描述2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovj8wosxj315g0zgka4.jpg) ｜ [公开数据集概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovk5lhpwj31gy0gin8q.jpg)
- [Cityscapes数据集上的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovl9ji77j312a0wowub.jpg) | [COCO数据集上的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovmozsa2j30ze0zo000.jpg) ｜ [Mapillary Vitas, Pascal VOC 2012 和 ADE20K上的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovne07rmj31d20qkaqo.jpg) | [KITTI 和 SemanticKITTI性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovr4acc9j31cc0i0gz8.jpg) | [两个组织病理学和荧光显微镜数据集的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovsf04cgj31cu0f2wps.jpg)
- [AP、IoU表现](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovomjwxhj312k0zw16u.jpg)

<br>



<br><br>

<a name="3"/>

## 医学影像

[1]  Medical Visual Question Answering: A Survey<br>
[paper](https://arxiv.org/abs/2111.10056)<br>
作者：Zhihong Lin,Donghao Zhang,Qingyi Tac,Danli Shi,Gholamreza Haffari,Qi Wu,Mingguang He,Zongyuan Ge<br>
机构：beResearch Center, Monash University, Clayton, VIC, Australia, NVIDIA AI Technology Center, Singapore, State Key Laboratory of Ophthalmology, Zhongshan Ophthalmic Center, Sun Yat-Sen University, Guangzhou, China<br>
摘要：医学视觉问答（VQA）是医学人工智能和流行的VQA挑战的结合。给定一幅医学图像和一个自然语言的临床相关问题，医学VQA系统预计将预测一个可信和令人信服的答案。虽然已经对一般领域的VQA进行了广泛的研究，但医学VQA由于其任务的特点，仍然需要具体的调查和探索。在本次调查的第一部分中，我们涵盖并讨论了最新公开的医疗VQA数据集，包括数据源、数据量和任务特征。在第二部分中，我们回顾了医学VQA任务中使用的方法。在最后一部分，我们分析了该领域面临的一些医学挑战，并讨论了未来的研究方向。
- [数据集概述](https://tva1.sinaimg.cn/large/006C3FgEgy1gwov9ewwy7j31460w8n5l.jpg)
- [方法概览1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovbb04b3j31ei0yk16f.jpg) | [方法概览2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovd0mpeej31eg0ysgzl.jpg)
- [编码器使用情况](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovfx69smj319e0xaqjp.jpg)

<br><br> 

<a name="4"/> 

## 目标跟踪


<br><br>  

<a name="5"/>

## 人脸

<br><br>

<a name="6"/>

## Attention/Transformer

[1] Attention Mechanisms in Computer Vision: A Survey<br>
[paper](https://arxiv.org/abs/2111.07624) | [code](https://github.com/MenghaoGuo/Awesome-Vision-Attentions)<br>
作者：Meng-Hao Guo, Tian-Xing Xu, Jiang-Jiang Liu, Zheng-Ning Liu, Peng-Tao Jiang, Tai-Jiang Mu, Song-Hai Zhang, Ralph R. Martin, Ming-Ming Cheng, Shi-Min Hu<br>
机构：Tsinghua University,Nankai University,Cardiff University<br>
摘要：人类可以自然有效地在复杂的场景中找到显著区域。为了模仿人类视觉系统的这一功能，注意力机制被引入到计算机视觉中。这种注意力机制可以看作是一个基于输入图像特征的动态权值调整过程。注意力机制在图像分类、目标检测、语义分割、视频理解、图像生成、三维视觉、多模态任务和自监督学习等视觉任务中取得了巨大的成功。本文综述了计算机视觉中的各种注意力机制，并对其进行了分类，如通道注意力、空间注意力、时间注意力和分支注意力。本文还提出了注意机力制研究的未来方向。
- [注意力机制关键发展历程1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowdfj2z6j31g80o6ame.jpg) ｜ [注意力机制关键发展历程2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowg3vxqxj312g11in5o.jpg)
- [有代表性的通道注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhg6uxxj31ea0q2qgj.jpg) | [有代表性的空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhxdgenj31g40zoqmc.jpg) ｜ [有代表性的时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowilxvdrj31eq0fy46q.jpg) | [有代表性的分支注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowk45pqsj31e80euguj.jpg) | [有代表性的通道&空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowl29j15j31280zm16o.jpg) | [有代表性的空间&时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowlt98lgj31fo0mg14i.jpg)



