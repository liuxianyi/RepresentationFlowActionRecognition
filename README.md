# RepresentationFlowActionRecognition
 百度顶会论文复现--Representation Flow For Action Recognition
# 论文心得
## 摘要
由光流算法得启发，提出了一种光流表示的卷积层。将该卷积层与传统的CNN结合在一起，提高了动作识别的能力。实验中，与传统的识别模型相比，无论在计算速度还是在表现上都具有很大的优势。
## 相关方法介绍
###CNN是最主要的方法：
1. 双流网络：RGB 与 光流
2. 3D时空卷积
3. I3D：XYT + RGB + flow

缺点：Flow计算代价高，Flow和CNNs需要并行，实时性差
###很早之前的方法
4. ActionFlowNet/motion feature networks： 虽然在计算速度和参数数量上由很大的优势，但是与双流网络相比表现能力很差。
## paper提出的方法
不需要计算光流，提出了representation flow layer 能够捕获光流，光流参数与模型参数同时学习。通过堆叠表示光流层实现了flow to flow 的表现。
## 
# 代码要点