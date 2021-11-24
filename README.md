# survey-computer-vision（2021-2022）

## 计算机视觉综述论文分方向整理（持续更新）<br>

## 目录
* [目标检测](#1)<br>
* [图像分割](#2)<br>
* [医学影像](#3)<br>
* [目标跟踪](#4)<br>
* [人脸](#5)<br>
* [三维视觉](#6)<br>
* [Attetion/Transformer](#7)

<br><br>

<a name="1"/>

## 目标检测（object detection）

#### 综述一：小样本目标检测｜[A Comparative Review of Recent Few-Shot Object Detection Algorithms](https://arxiv.org/pdf/2111.00201.pdf)

作者：Leng Jiaxu, Chen Taiyue, Gao Xinbo, Yu Yongtao, Wang Ye, Gao Feng, Wang Yue<br>
机构：Chongqing University of Posts and Telecommunications<br>
摘要：由于现实世界数据的长尾分布和削减数据收集和注释成本的迫切需求，学习适应具有少量标记数据的新类的少样本目标检测是一个迫切和长期的问题。近年来，一些研究探讨了如何在不需要目标域监督的情况下，在额外数据集中使用隐式线索来帮助少样本检测器完善鲁棒任务概念。本综述从当前的经典和最新研究成果，以及未来的研究展望，从多方面进行了综述。特别地，我们首先提出了基于数据的训练数据分类和在训练阶段访问的相应监督形式。按照这种分类法，我们对正式定义、主要挑战、基准数据集、评估指标和学习策略进行了重要的回顾。此外，我们还详细研究了如何相互作用的目标检测方法，以系统地发展这一问题。最后，总结了少样本目标检测的研究现状及未来的研究方向。<br>
- [近期小样本目标检测算法概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfqcvlsfj31ii0v07im.jpg)



<br><br>

<a name="2"/>

## 图像分割

#### 综述一：全景分割｜[Panoptic Segmentation: A Review](https://arxiv.org/abs/2111.10250)

[code](https://github.com/elharroussomar/Awesome-Panoptic-Segmentation)<br>
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

#### 综述一：医疗视觉问答｜[Medical Visual Question Answering: A Survey](https://arxiv.org/abs/2111.10056)

作者：Zhihong Lin,Donghao Zhang,Qingyi Tac,Danli Shi,Gholamreza Haffari,Qi Wu,Mingguang He,Zongyuan Ge<br>
机构：beResearch Center, Monash University, Clayton, VIC, Australia, NVIDIA AI Technology Center, Singapore, State Key Laboratory of Ophthalmology, Zhongshan Ophthalmic Center, Sun Yat-Sen University, Guangzhou, China<br>
摘要：医学视觉问答（VQA）是医学人工智能和流行的VQA挑战的结合。给定一幅医学图像和一个自然语言的临床相关问题，医学VQA系统预计将预测一个可信和令人信服的答案。虽然已经对一般领域的VQA进行了广泛的研究，但医学VQA由于其任务的特点，仍然需要具体的调查和探索。在本次调查的第一部分中，我们涵盖并讨论了最新公开的医疗VQA数据集，包括数据源、数据量和任务特征。在第二部分中，我们回顾了医学VQA任务中使用的方法。在最后一部分，我们分析了该领域面临的一些医学挑战，并讨论了未来的研究方向。
- [数据集概述](https://tva1.sinaimg.cn/large/006C3FgEgy1gwov9ewwy7j31460w8n5l.jpg)
- [方法概览1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovbb04b3j31ei0yk16f.jpg) | [方法概览2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovd0mpeej31eg0ysgzl.jpg)
- [编码器使用情况](https://tva1.sinaimg.cn/large/006C3FgEgy1gwovfx69smj319e0xaqjp.jpg)

#### 综述二：医学图像分割｜[A Review on The Division of Magnetic Resonant Prostate Images with Deep  Learning](https://arxiv.org/abs/2111.10683)

作者：Elcin Nizami Huseyn, Emin Taleh Mammadov, Mohammad Hoseini
机构：Azerbaijan State Oil and Industry University, Azerbaijan Medical University, Seraj Higher Education Institute
摘要：深度学习通常用于生物医学领域的图像分割过程。 近年来，利用深度学习进行的前列腺图像分割过程是前列腺癌诊治的重要步骤。 本文研究了从磁共振 (MRI) 成像设备获得的前列腺图像的深度学习分割程序。




<br><br> 

<a name="4"/> 

## 目标跟踪


<br><br>  

<a name="5"/>

## 人脸

<br><br>  

<a name="6"/>

## 三维视觉

#### 综述一：三维点云｜[A Comparative Review of Recent Few-Shot Object Detection Algorithms](https://arxiv.org/abs/2111.00201)

[code](https://github.com/QingyongHu/SoTA-Point-Cloud)<br>
作者：Yulan Guo, Hanyun Wang, Qingyong Hu, Hao Liu, Li Liu, and Mohammed Bennamoun<br>
机构：Sun Yat-sen University, Information Engineering University, University of Oxford, National University of Defense Technology, University of Oulu, the University of Western<br>
摘要：点云学习近年来受到越来越多的关注，因为它在许多领域都有广泛的应用，比如计算机视觉、自动驾驶和机器人技术。作为人工智能的主要技术之一，深度学习已经成功地用于解决各种二维视觉问题。然而，由于使用深度神经网络处理点云所面临的独特挑战，对点云的深度学习仍处于起步阶段。最近，点云上的深度学习变得越来越流行，人们提出了许多方法来解决这一领域的不同问题。为了激发未来的研究，本文对点云深度学习方法的最新进展进行了综述。它涵盖了三个主要任务，包括三维形状分类，三维目标检测和跟踪以及三维点云分割。我们还提供了一些可公开获得的数据集的比较结果，以及有见地的观察和启发性的未来研究方向。<br>
- [基于深度学习的3D点云方法分类](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfcai9cxj31gs0o0wpf.jpg) ｜ [用于3D形状分类、3D对象检测和跟踪以及3D点云分割的现有数据集概况](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfeqrrdnj319s0uq1da.jpg)
- [基于深度学习的3D形状分类方法的时间线](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqffpl2mfj31lq0gwtq9.jpg) ｜ [在 ModelNet10/40 基准上比较3D形状分类方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfgx1wptj30zi0zqka3.jpg)
- [基于深度学习的3D目标检测方法的时间线](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfi3qbxxj31bw0msanp.jpg) | [在 KITTI 3D 检测基准上比较3D目标检测方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfizd6jbj314y0xungi.jpg) | [在 KITTI BEV 检测基准上比较3D目标检测方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfkdtijkj314g0wq4gw.jpg)
- [基于深度学习的3D语义分割方法的时间线](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfl445n5j31iy0f0h1p.jpg) | [在 S3DIS 上的比较语义分割方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqflv54urj31600zangl.jpg)
- [基于深度学习的3D实例分割方法的时间线](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfmh0l90j30uy0dqn4e.jpg)



<br><br>

<a name="7"/>

## Attention/Transformer

[1] Attention Mechanisms in Computer Vision: A Survey<br>
[paper](https://arxiv.org/abs/2111.07624) | [code](https://github.com/MenghaoGuo/Awesome-Vision-Attentions)<br>
作者：Meng-Hao Guo, Tian-Xing Xu, Jiang-Jiang Liu, Zheng-Ning Liu, Peng-Tao Jiang, Tai-Jiang Mu, Song-Hai Zhang, Ralph R. Martin, Ming-Ming Cheng, Shi-Min Hu<br>
机构：Tsinghua University,Nankai University,Cardiff University<br>
摘要：人类可以自然有效地在复杂的场景中找到显著区域。为了模仿人类视觉系统的这一功能，注意力机制被引入到计算机视觉中。这种注意力机制可以看作是一个基于输入图像特征的动态权值调整过程。注意力机制在图像分类、目标检测、语义分割、视频理解、图像生成、三维视觉、多模态任务和自监督学习等视觉任务中取得了巨大的成功。本文综述了计算机视觉中的各种注意力机制，并对其进行了分类，如通道注意力、空间注意力、时间注意力和分支注意力。本文还提出了注意机力制研究的未来方向。
- [注意力机制关键发展历程1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowdfj2z6j31g80o6ame.jpg) ｜ [注意力机制关键发展历程2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowg3vxqxj312g11in5o.jpg)
- [有代表性的通道注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhg6uxxj31ea0q2qgj.jpg) | [有代表性的空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhxdgenj31g40zoqmc.jpg) ｜ [有代表性的时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowilxvdrj31eq0fy46q.jpg) | [有代表性的分支注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowk45pqsj31e80euguj.jpg) | [有代表性的通道&空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowl29j15j31280zm16o.jpg) | [有代表性的空间&时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowlt98lgj31fo0mg14i.jpg)

[2] A Survey of Visual Transformers<br>
[paper](https://arxiv.org/abs/2111.06091v2)<br>
作者：Yang Liu, Yao Zhang, Yixin Wang, Feng Hou, Jin Yuan, Jiang Tian, Yang Zhang, Zhongchao Shi, Jianping Fan, Zhiqiang He<br>
机构：University of Chinese Academy of Sciences, Southeast University, Lenovo Ltd
摘要：Transformer 是一种基于注意力的编码器-解码器架构，彻底改变了自然语言处理领域。受这一重大成就的启发，最近在将类似 Transformer 的体系结构应用于计算机视觉 领域方面进行了一些开创性工作，这些工作已经证明了它们在各种 CV 任务上的有效性。与 CNN 相比，visual Transformers 依靠有竞争力的建模能力，在 ImageNet、COCO 和 ADE20k 等多个基准测试中取得了令人印象深刻的性能。在本文中，我们全面回顾了针对三个基本 CV 任务（分类、检测和分割）的一百多种不同的视觉变换器，其中提出了一种分类法来根据它们的动机、结构和使用场景来组织这些方法. 由于训练设置和面向任务的差异，我们还在不同的配置上评估了这些方法，以方便直观地进行比较，而不仅仅是各种基准测试。此外，我们揭示了一系列基本但未开发的方面，这些方面可能使 Transformer 从众多架构中脱颖而出，例如，松弛的高级语义嵌入以弥合视觉和顺序 Transformer 之间的差距。最后，提出了三个有前景的未来研究方向，以供进一步研究。<br>
- 详细中文解读：[中国科学院、东南大学等联合发表最新的视觉 Transformer 综述](https://bbs.cvmart.net/articles/5763)



