# survey-computer-vision（2021-2022）

## 计算机视觉综述论文分方向整理（持续更新）<br>

## 目录
* [目标检测](#1)<br>
* [图像分割](#2)<br>
* [医学影像](#3)<br>
* [目标跟踪](#4)<br>
* [人脸](#5)<br>
* [三维视觉](#6)<br>
* [网络架构设计](#7)
* [超分辨率](#8)
* [暂未分类](#100)

<br><br>

<a name="1"/>

## 目标检测（object detection）

#### 综述一：小样本目标检测｜[A Comparative Review of Recent Few-Shot Object Detection Algorithms](https://arxiv.org/pdf/2111.00201.pdf)

作者：Leng Jiaxu, Chen Taiyue, Gao Xinbo, Yu Yongtao, Wang Ye, Gao Feng, Wang Yue<br>
机构：Chongqing University of Posts and Telecommunications<br>
摘要：由于现实世界数据的长尾分布和削减数据收集和注释成本的迫切需求，学习适应具有少量标记数据的新类的少样本目标检测是一个迫切和长期的问题。近年来，一些研究探讨了如何在不需要目标域监督的情况下，在额外数据集中使用隐式线索来帮助少样本检测器完善鲁棒任务概念。本综述从当前的经典和最新研究成果，以及未来的研究展望，从多方面进行了综述。特别地，我们首先提出了基于数据的训练数据分类和在训练阶段访问的相应监督形式。按照这种分类法，我们对正式定义、主要挑战、基准数据集、评估指标和学习策略进行了重要的回顾。此外，我们还详细研究了如何相互作用的目标检测方法，以系统地发展这一问题。最后，总结了少样本目标检测的研究现状及未来的研究方向。<br>
- [近期小样本目标检测算法概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwqfqcvlsfj31ii0v07im.jpg)

<br><br>

#### 综述二：自监督小样本检测｜[A Survey of Self-Supervised and Few-Shot Object Detection](https://arxiv.org/abs/2110.14711)

[project](https://gabrielhuang.github.io/fsod-survey/)<br>
作者：Gabriel Huang, Issam Laradji, David Vazquez, Simon Lacoste-Julien, Pau Rodriguez<br>
机构：Université de Montréal<br>
摘要：标记数据通常是昂贵和耗时的，特别是对于目标检测和实例分割等任务，这需要密集的图像标记。虽然少样本目标检测是关于用很少的数据在新的(看不见的)目标类上训练模型，但它仍然需要在许多标记的基类(见)的示例上进行预训练。另一方面，自监督方法旨在从未标记的数据中学习表示，这些数据可以很好地转移到下游任务，如目标检测。将少样本和自监督目标检测相结合是一个很有前景的研究方向。在这个综述中，我们回顾和描述了最近的方法在少样本和自监督的目标检测。然后，我们给出了主要的结论，并讨论了未来的研究方向。<br>
- [文中所有目标检测方法分类](https://tva1.sinaimg.cn/large/006C3FgEgy1gww6r9136jj316w0xondm.jpg)
- [在 PASCAL VOC 和 MS COCO 数据集上的方法结果对比](https://tva1.sinaimg.cn/large/006C3FgEgy1gww77dhzkqj31d80ygk97.jpg)
- [在未标注的 ImageNet 上预训练的自监督目标检测方法比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gww78snik4j31f60oy4as.jpg)

<br><br>

#### 综述三：小样本目标检测｜[A Survey of Deep Learning for Low-Shot Object Detection](https://arxiv.org/pdf/2112.02814v2.pdf)

作者：Qihan Huang, Haofei Zhang, Jie Song, Mingli Song<br>
机构：浙江大学<br>
摘要：本文对少样本目标检测(few-shot Object Detection, FSOD)和零样本目标检测(zero-shot Object Detection, ZSD)进行了全面的研究阐述。将FSOD和ZSD的方法分为不同的类别，并讨论了它们的优缺点。其次，本综述回顾了FSOD和ZSD的数据集设置和评估指标，然后分析了不同方法在这些基准上的性能。最后，本综述讨论了FSOD和ZSD未来面临的挑战和发展方向。<br>
- [综述概述](https://tva1.sinaimg.cn/large/006C3FgEgy1gxmsv3g6i7j31g00xmasq.jpg)，本文将低样本目标检测分为单样本目标检测、少样本目标检测和零样本目标检测三个领域，用三种颜色演示了这三个域的更细粒度的分类，并总结了OSOD、FS和ZSD的基准，比较分析了不同LSOD方法在这些基准上的性能。
- [在MS COCO基准上的ZSD方法性能表现](https://tva1.sinaimg.cn/large/006C3FgEgy1gxmsy5yp31j31g00wetof.jpg)


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

<br><br>

#### 综述二：医学图像分割｜[A Review on The Division of Magnetic Resonant Prostate Images with Deep  Learning](https://arxiv.org/abs/2111.10683)

作者：Elcin Nizami Huseyn, Emin Taleh Mammadov, Mohammad Hoseini
机构：Azerbaijan State Oil and Industry University, Azerbaijan Medical University, Seraj Higher Education Institute
摘要：深度学习通常用于生物医学领域的图像分割过程。 近年来，利用深度学习进行的前列腺图像分割过程是前列腺癌诊治的重要步骤。 本文研究了从磁共振 (MRI) 成像设备获得的前列腺图像的深度学习分割程序。




<br><br> 

<a name="4"/> 

## 目标跟踪

#### 综述一：无人机检测与跟踪｜[Deep Learning for UAV-based Object Detection and Tracking: A Survey](https://arxiv.org/abs/2110.12638v1)

作者：Xin Wu, Wei Li, Danfeng Hong, Ran Tao, Qian Du<br>
机构：Beijing Institute of Technology, Chinese Academy of Sciences, Mississippi State University<br>
摘要：无人机(UAV)由于有效且灵活的数据采集，近年来已成为计算机视觉(CV)和遥感(RS)领域的研究热点。由于最近深度学习(DL)的成功，许多先进的目标检测和跟踪方法已被广泛应用于与无人机相关的各种任务，例如环境监测、精准农业、交通管理。本文全面综述了基于DL的无人机目标检测与跟踪方法的研究进展和前景。具体来说，我们首先概述了挑战，统计了现有的方法，并从基于DL的模型的角度提供了解决方案，这三个研究课题分别是:来自图像的目标检测，来自视频的目标检测，来自视频的目标跟踪。利用无人机主导目标检测与跟踪相关的开放数据集，利用4个基准数据集，采用最先进的方法进行性能评估。最后，对今后的工作进行了展望和总结。本文对基于DL的无人机目标探测与跟踪方法进行了综述，并对其进一步发展提出了一些思考，以期为来自遥感领域的研究人员提供参考。<br>
- [无人机静态目标检测典型方法发展历程](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzl4x6bkj31fy0vm4km.jpg) | [基于深度学习的无人机静态目标检测方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzn8zmgpj31gi0qu4g4.jpg)
- [无人机视频目标检测典型方法发展历程](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzojfwqij31hq0qw4aj.jpg) | [基于深度学习的无人机视频目标检测方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzoyf5hvj31gi0bkn2k.jpg)
- [无人机视频目标跟踪典型方法发展历程](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzpgghmaj31h20qugv4.jpg) | [基于深度学习的无人机视频目标跟踪方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzq2330tj31gi0lctls.jpg)
- [当前最先进的无人机基准和数据集的比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzqtb7b1j31i00wy1d2.jpg)
- [无人机专属检测网络和经典检测网络的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzsb90q8j317q0ze1ij.jpg) | [在 UAVDT-DET 测试集上的目标检测结果](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzta673sj31fo0bugsv.jpg)
- [以 MOTA、MOTP 等为评估指标的 UAVDT 数据集的 UAV 专属跟踪网络和经典跟踪网络的性能比较](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzu5r26aj31fg0g2alu.jpg) 
- [无人机专属统计目标检测方法的计算成本](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzuw3cfbj31dq0vyqnf.jpg) | [无人机专专属的基于深度学习的视频目标检测方法的计算成本](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzwdaab4j31ga0fs484.jpg) | [无人机专用的基于深度学习的多目标跟踪的计算成本](https://tva1.sinaimg.cn/large/006C3FgEgy1gwwzx80g32j31gq0q0k7u.jpg)


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

## 网络架构设计

#### 综述一：Attention | [Attention Mechanisms in Computer Vision: A Survey](https://arxiv.org/abs/2111.07624)

[code](https://github.com/MenghaoGuo/Awesome-Vision-Attentions)<br>
作者：Meng-Hao Guo, Tian-Xing Xu, Jiang-Jiang Liu, Zheng-Ning Liu, Peng-Tao Jiang, Tai-Jiang Mu, Song-Hai Zhang, Ralph R. Martin, Ming-Ming Cheng, Shi-Min Hu<br>
机构：Tsinghua University,Nankai University,Cardiff University<br>
摘要：人类可以自然有效地在复杂的场景中找到显著区域。为了模仿人类视觉系统的这一功能，注意力机制被引入到计算机视觉中。这种注意力机制可以看作是一个基于输入图像特征的动态权值调整过程。注意力机制在图像分类、目标检测、语义分割、视频理解、图像生成、三维视觉、多模态任务和自监督学习等视觉任务中取得了巨大的成功。本文综述了计算机视觉中的各种注意力机制，并对其进行了分类，如通道注意力、空间注意力、时间注意力和分支注意力。本文还提出了注意机力制研究的未来方向。
- [注意力机制关键发展历程1](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowdfj2z6j31g80o6ame.jpg) ｜ [注意力机制关键发展历程2](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowg3vxqxj312g11in5o.jpg)
- [有代表性的通道注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhg6uxxj31ea0q2qgj.jpg) | [有代表性的空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowhxdgenj31g40zoqmc.jpg) ｜ [有代表性的时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowilxvdrj31eq0fy46q.jpg) | [有代表性的分支注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowk45pqsj31e80euguj.jpg) | [有代表性的通道&空间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowl29j15j31280zm16o.jpg) | [有代表性的空间&时间注意力机制概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwowlt98lgj31fo0mg14i.jpg)<br><br>

#### 综述二：Transformer | [A Survey of Visual Transformers](https://arxiv.org/abs/2111.06091v2)<br>

作者：Yang Liu, Yao Zhang, Yixin Wang, Feng Hou, Jin Yuan, Jiang Tian, Yang Zhang, Zhongchao Shi, Jianping Fan, Zhiqiang He<br>
机构：University of Chinese Academy of Sciences, Southeast University, Lenovo Ltd
摘要：Transformer 是一种基于注意力的编码器-解码器架构，彻底改变了自然语言处理领域。受这一重大成就的启发，最近在将类似 Transformer 的体系结构应用于计算机视觉 领域方面进行了一些开创性工作，这些工作已经证明了它们在各种 CV 任务上的有效性。与 CNN 相比，visual Transformers 依靠有竞争力的建模能力，在 ImageNet、COCO 和 ADE20k 等多个基准测试中取得了令人印象深刻的性能。在本文中，我们全面回顾了针对三个基本 CV 任务（分类、检测和分割）的一百多种不同的视觉变换器，其中提出了一种分类法来根据它们的动机、结构和使用场景来组织这些方法. 由于训练设置和面向任务的差异，我们还在不同的配置上评估了这些方法，以方便直观地进行比较，而不仅仅是各种基准测试。此外，我们揭示了一系列基本但未开发的方面，这些方面可能使 Transformer 从众多架构中脱颖而出，例如，松弛的高级语义嵌入以弥合视觉和顺序 Transformer 之间的差距。最后，提出了三个有前景的未来研究方向，以供进一步研究。<br>
- 详细中文解读：[中国科学院、东南大学等联合发表最新的视觉 Transformer 综述](https://bbs.cvmart.net/articles/5763)<br><br>

#### 综述三：Attention| [Neural Attention Models in Deep Learning: Survey and Taxonomy](https://arxiv.org/pdf/2112.05909.pdf)

作者：Alana de Santana Correia, Esther Luna Colombini<br>
机构：University of Campinas<br><br>

#### 综述四：MLP | [Are we ready for a new paradigm shift? A Survey on Visual Deep MLP](https://arxiv.org/abs/2111.04060)<br>


<br><br>  

<a name="8"/>

## 超分辨率

#### 综述一：单图像超分 | [From Beginner to Master: A Survey for Deep Learning-based Single-Image Super-Resolution](https://arxiv.org/abs/2109.14335)

[project](https://github.com/CV-JunchengLi/SISR-Survey)<br>
作者：Juncheng Li, Zehua Pei, Tieyong Zeng<br>
机构：The Chinese University of Hong Kong<br>
摘要：单图像超分辨率(SISR)是图像处理中的一项重要任务，其目的是提高成像系统的分辨率。近年来，在深度学习(deep learning, DL)的帮助下，SISR取得了巨大的飞跃，并取得了可喜的成果。在本文中，我们概述了基于深度学习的SISR方法，并根据它们的目标，如重建效率、重建精度和感知精度进行分组。具体地，首先介绍了问题的定义、研究背景和研究意义。其次，介绍了相关工作，包括基准数据集、上采样方法、优化目标和图像质量评价方法。第三，详细介绍了系统集成研究的基本原理，并给出了系统集成研究的一些具体应用。第四，我们给出了一些经典的SISR方法的重构结果，直观地了解了它们的性能。最后，本文还讨论了该研究中存在的一些问题，并总结了一些新的发展趋势和未来的发展方向。这是对SISR的详细调研，有助于研究者更好地理解SISR，并激发更多的研究。<br>
- [四类单图像超分方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gx6iuh8bwsj31i40xetnx.jpg)
- [单图像超分数据集概括](https://tva1.sinaimg.cn/large/006C3FgEgy1gx6iw3r2kbj31gi0piduo.jpg)
- [PSNR/SSIM对比](https://tva1.sinaimg.cn/large/006C3FgEgy1gx6k5yg93sj31060zoh70.jpg)



<br><br>

<a name="100"/>

## 暂未分类

#### 自监督特征学习(TPAMI2021) | [Self-supervised Visual Feature Learning with Deep Neural Networks: A Survey](https://arxiv.org/abs/1902.06162v1)

作者：Longlong Jing, Yingli Tian<br>
机构：The City University of New York<br>
摘要：为了在计算机视觉应用中学习得到更好的图像和视频特征，通常需要大规模的标记数据来训练深度神经网络。为了避免收集和标注大量的数据所需的巨大开销，作为无监督学习方法的一个子方法——自监督学习方法，可以在不使用任何人类标注的标签的情况下，从大规模无标记数据中学习图像和视频的一般性特征。本文对基于深度学习的自监督一般性视觉特征学习方法做了综述。首先，描述了该领域的动机和一些专业性术语。在此基础上，总结了常用的用于自监督学习的深度神经网络体系结构。接下来，回顾了自监督学习方法的模式和评价指标，并介绍了常用的图像和视频数据集以及现有的自监督视觉特征学习方法。最后，总结和讨论了基于标准数据集的性能比较方法在图像和视频特征学习中的应用。<br>
- [自监督视觉特征学习的前置任务分类](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyh9d1wx4j31ao0xinj1.jpg)
- [常见的视频/图片数据集](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyhbxjbx5j31em0iqn8m.jpg)
- [基于前置任务分类的自监督图片特征学习方法概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyhd0kynhj31a00ve1ge.jpg) ｜ [基于前置任务分类的自监督视频特征学习方法概览](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyhe8goeej31bc0w8had.jpg)
- [使用来自 AlexNet 卷积层作为特征的激活在 ImageNet 和 Places 数据集上进行线性分类](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyhflvuqpj31ja0j24ao.jpg)
- [在 PASCAL VOC 数据集上比较自监督图片特征学习在分类、检测、分割任务上的表现](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyhzz3m8ej31h40o6gxe.jpg) | [在 UCF101 和 HMDB51数据上比较动作识别任务上的自监督特征学习方法](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyi1x1mfvj30s60lsdnf.jpg)<br><br>

#### 长尾学习 | [Deep Long-Tailed Learning: A Survey](https://arxiv.org/abs/2110.04596)

作者：Yifan Zhang, Bingyi Kang, Bryan Hooi, Shuicheng Yan, Jiashi Feng<br>
机构：National University of Singapore, Singapore, SEA AI Lab<br>
摘要：深度长尾学习是视觉识别中最具挑战性的问题之一，其目标是从大量遵循长尾类分布的图像中训练出性能良好的深度模型。在过去的十年中，深度学习已经成为一种学习高质量图像表示的强大的识别模型，并导致了一般视觉识别的显著突破。然而，长尾类不平衡是实际视觉识别任务中普遍存在的问题，这种不平衡往往限制了基于深度网络的识别模型在实际应用中的实用性，因为长尾类容易偏向主导类，在尾类上的表现较差。为了解决这一问题，近年来人们进行了大量的研究，在深度长尾学习领域取得了可喜的进展。鉴于该领域的快速发展，本文对深度长尾学习的最新进展进行了综述。具体地说，我们将已有的深度长尾学习研究分为三类(即类重平衡、信息增强和模块改进)，并根据这三类对这些方法进行了详细的回顾。之后，我们通过一种新提出的评价指标，即相对准确性，来评估它们在多大程度上解决了阶级失衡问题，从而对几种最先进的方法进行了实证分析。最后，我们强调了深度长尾学习的重要应用，并确定了未来研究的几个有前景的方向。<br>
- [2021年中之前在顶会上发表的深度长尾学习方法总结](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyifyaa9nj30rw0zathg.jpg),[code](https://github.com/Vanint/Awesome-LongTailed-Learning)
- [在 ImageNet-LT 上 90 或 200 个epochs下的Acc, UA, RA](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyiixbwofj30qe0t27dx.jpg) | [在 ImageNet-LT 上 90 或 200 个 epochs 下关于头部、中间和尾部类别的精度](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyijdp7c0j30o40tcaj2.jpg)
- [长尾学习方法在 200 个 epoch 下的精度和相对精度方面的性能曲线](https://tva1.sinaimg.cn/large/006C3FgEgy1gwyiwzde2fj313g0u848v.jpg)<br><br>

#### 激活函数 | [A Comprehensive Survey and Performance Analysis of Activation Functions in Deep Learning](https://arxiv.org/abs/2109.14545v1)

[code](https://github.com/shivram1987/ActivationFunctions)<br>
作者：Shiv Ram Dubey, Satish Kumar Singh, Bidyut Baran Chaudhuri<br>
摘要：近年来，神经网络在解决许多问题方面有了巨大的发展。不同类型的神经网络被引入来处理不同类型的问题。然而，任何神经网络的主要目标是将非线性可分的输入数据转换为更线性可分的抽象特征，使用层次结构。这些层是线性和非线性函数的组合。最流行和常见的非线性层是激活函数(AFs)，如Logistic Sigmoid、Tanh、ReLU、ELU、Swish和Mish。本文对深度学习神经网络中的激活函数AFs进行了全面的综述和研究。不同类别的AFs，如Logistic Sigmoid和基于Tanh，基于ReLU，基于ELU，和基于Learning。指出了AFs的输出范围、单调性和平滑性等特点。并对18种最先进的AFs在不同网络上的性能进行了比较。本文提出了AFs的见解，以帮助研究者进行进一步的研究，并帮助实践者在不同的选择中进行选择。用于实验比较的代码。<br><br>

#### 元学习 | [Multimodality in Meta-Learning: A Comprehensive Survey](https://arxiv.org/abs/2109.13576v1)

作者：Yao Ma, Shilin Zhao, Weixiao Wang, Yaoman Li, Irwin King<br>
摘要：作为一种比传统机器学习方法更有效的训练框架，元学习获得了广泛的欢迎。然而，在多模态任务等复杂任务分布中，其泛化能力尚未得到深入研究。近年来，基于多模态的元学习出现了一些研究。本综述从方法论和应用方面提供了基于多模态的元学习景观的全面概述。我们首先对元学习和多模态的定义进行了形式化的界定，并提出了这一新兴领域的研究挑战，如何丰富少样本或零样本情况下的输入，以及如何将模型泛化到新的任务中。然后我们提出了一个新的分类系统，系统地讨论了结合多模态任务的典型元学习算法。我们对相关论文的贡献进行了调研，并对其进行了分类总结。最后，提出了该领域的研究方向。<br><br>

#### 迁移学习 | [Bayesian Transfer Learning: An Overview of Probabilistic Graphical Models for Transfer Learning](https://arxiv.org/abs/2109.13233)

作者：Junyu Xuan, Jie Lu, Guangquan Zhang<br>
摘要：迁移学习是指从源领域提取可迁移知识并将其重用到目标领域的行为，已成为人工智能领域的研究热点。概率图模型(PGMs)作为一种建模复杂系统的强大工具，具有处理不确定性的能力和良好的可解释性。考虑到上述两个研究领域的成功，将PGMs应用于迁移学习似乎是很自然的。然而，尽管在文献中已经有一些优秀的迁移学习特异性PGMs，但PGMs在这一问题上的潜力仍然被严重低估。本文旨在通过以下几个方面促进迁移学习的知识迁移模型的发展:1)考察迁移学习的知识迁移模型的试点研究，即分析和总结现有的专门设计的知识迁移机制;2)讨论现有PGM成功应用于实际迁移问题的例子;3)利用PGM探讨迁移学习的几个潜在研究方向。<br><br>

#### 无监督域适应 | [A Survey of Unsupervised Domain Adaptation for Visual Recognition](https://arxiv.org/pdf/2112.06745v1.pdf)

作者：Youshan Zhang<br>
机构：Lehigh University<br>
摘要：虽然在许多领域生成并提供了大量未标记数据，但对自动理解可视化数据的需求比以往任何时候都要高。大多数现有的机器学习模型通常依赖于大量带标签的训练数据来实现高性能。不幸的是，这样的需求在真实的应用中无法满足。标签的数量是有限的，手动注释数据是昂贵和耗时的。通常需要将知识从现有的标记领域迁移到新的领域。然而，模型性能会因为域之间的差异而降低(域移位或数据集偏差)。为了克服标注的负担，领域适应(Domain Adaptation, DA)旨在缓解知识从一个领域转移到另一个相似但不同的领域时的领域转移问题。无监督DA (UDA)处理有标记的源域和无标记的目标域。UDA的主要目标是减少带标签源数据和未带标签目标数据之间的域差异，并在训练过程中学习跨两个域的域不变表示。本文首先定义了UDA问题。其次，我们从传统方法和基于深度学习的方法两方面概述了用于不同类别UDA的最新方法。最后，我们收集了常用的基准数据集，并报告了UDA在视觉识别问题上的最新方法的结果。<br>
- [方法分类](https://tva1.sinaimg.cn/large/006C3FgEgy1gxskidkxa1j316s0oy7ic.jpg)
- [在Office + Caltech-10上的精度](https://tva1.sinaimg.cn/large/006C3FgEgy1gxskl1gh8qj31es0hcam6.jpg)
- [在Office-Home上的精度](https://tva1.sinaimg.cn/large/006C3FgEgy1gxskmgct0bj31iw0qawxf.jpg)
- [在VisDA-2017上的精度](https://tva1.sinaimg.cn/large/006C3FgEgy1gxsko6wgunj31f40iqqg4.jpg)
- [在Office-31上的精度](https://tva1.sinaimg.cn/large/006C3FgEgy1gxskpaj0lcj30u00mo11z.jpg)













