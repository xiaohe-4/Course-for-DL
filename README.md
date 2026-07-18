# Course-for-DL
A repository for Learning DeepLearning course.
## 第 1 周：人工智能与深度学习导论
- 1、人工智能发展历程;
- 2、深度学习基本概念与机器学习的关系；
- 3、深度学习分类与机器学习的演进史；
- 4、深度学习的应用领域。
## 第 2 周：神经网络基础与多层感知机（MLP）
- 神经元模型： 生物神经元到数学模型的抽象，感知机（Perceptron）原理。
- 多层感知机（MLP）架构： 输入层、隐藏层、输出层的全连接（Fully Connected）结构。
- 激活函数（Activation Functions）： 为什么需要非线性？Sigmoid、Tanh、ReLU 及其变体的对比与选择。
- 前向传播与损失函数： 均方误差（MSE）、交叉熵（Cross-Entropy）的数学原理与应用场景。
## 第 3 周：卷积神经网络（CNN）基础
- 核心组件剖析： 卷积层（Convolutional Layer）、特征图（Feature Map）、填充（Padding）与步长（Stride）。
- 池化层（Pooling）： 最大池化（Max Pooling）与平均池化（Average Pooling）的作用与区别。
- 经典 CNN 架构演进： LeNet-5（经典开端）、AlexNet（深度突破）、VGG（小卷积核复用）。
- 残差网络（ResNet）： 残差连接（Skip Connection）如何解决超深网络中的梯度消失问题。
## 第 4 周：反向传播与模型优化基础
- 反向传播算法（Backpropagation）： 链式法则（Chain Rule）的推导，误差如何从输出层向后传递。
- 梯度下降算法（Gradient Descent）： BGD、SGD、Mini-batch SGD 的优缺点。
- 经典优化器（Optimizers）： Momentum、AdaGrad、RMSprop、Adam 的原理与调参经验。
- 梯度异常问题： 梯度消失（Vanishing Gradient）与梯度爆炸（Exploding Gradient）的成因及初步解决方案。
## 第 5 周：循环神经网络与序列模型（RNN/LSTM）
处理时间序列、文本等前后有依赖关系的数据。
- 序列数据建模： 为什么传统 MLP/CNN 难以处理变长序列？RNN 的循环结构与时间反向传播（BPTT）。
- 长程依赖问题： 传统 RNN 的“健忘”问题（梯度消失）。
- 门控机制：
  - LSTM（长短期记忆网络）： 输入门、遗忘门、输出门与细胞状态（Cell State）的运作机制。
  - GRU（门控循环单元）： 更新门与重置门的简化结构。
- 应用场景： 文本生成、情感分析、时间序列预测。
## 第 6 周：前沿序列模型：Transformer 基础
现代大语言模型（LLM）的基石，颠覆了传统的循环结构。
- 注意力机制（Attention Mechanism）： 从 Seq2Seq + Attention 谈起，Query、Key、Value 的概念。
- 自注意力（Self-Attention）： 数学推导与缩放点积注意力（Scaled Dot-Product Attention）。
- 多头注意力（Multi-Head Attention）： 为什么要“多头”？如何捕捉不同子空间的特征。
- Transformer 整体架构： 位置编码（Positional Encoding）、层归一化（Layer Normalization）、Encoder-Decoder 结构解析。
## 第 7 周：自动编码器（AE）与表征学习
从监督学习转向自监督/无监督学习，探索数据的低维流形。
- 传统自动编码器（Autoencoder, AE）： 编码器（Encoder）、瓶颈层（Bottleneck/Latent Space）、解码器（Decoder）与重构损失。
- 常见变体： 降噪自动编码器（DAE）、稀疏自动编码器（SAE）的原理与应用。
- 变分自动编码器（VAE）： 从确定性编码到概率分布，KL 散度（Kullback-Leibler Divergence）在隐空间重构中的作用。
- 应用： 数据降维、特征提取、图像去噪。
## 第 8 周：生成对抗网络（GAN）基础
开启生成式 AI 的第一扇大门，理解“博弈”的思想。
- 对抗生成博弈论： 生成器（Generator）与判别器（Discriminator）的博弈机制。
- GAN 的损失函数： Minimax 目标函数的数学意义。
- 训练困境与优化： 模式崩溃（Mode Collapse）、纳什均衡难达到、梯度消失问题。
- 经典变体： DCGAN（深度卷积 GAN）、WGAN（使用推土机距离解决训练不稳定问题）。
## 第 9 周：扩散模型（Diffusion Models）基础
当代图像生成（如 Midjourney, Stable Diffusion）的核心技术。
- 扩散模型核心概念： 为什么扩散模型能超越 GAN？
- 前向过程（Forward Process）： 逐步加噪的马尔可夫链过程。
- 反向过程（Reverse Process）： 神经网络如何学习去噪、从随机噪声中恢复图像。
- 经典架构解析： DDPM（Denoising Diffusion Probabilistic Models）的基本数学框架与训练流程简介。
## 第 10 周：图神经网络（GNN）基础
处理非欧几里得空间数据（如社交网络、分子结构、知识图谱）。
- 非欧几何数据： 图（Graphs）的表示，邻接矩阵（Adjacency Matrix）与度矩阵（Degree Matrix）。
- 图卷积网络（GCN）： 空域卷积与频域卷积（谱图理论简化）的区别，核心更新公式。
- 图注意力网络（GAT）： 将 Attention 机制引入图结构，动态分配邻居节点权重。
- 常见任务： 节点分类（Node Classification）、边预测（Link Prediction）、图分类。
## 第 11 周：强化学习（Reinforcement Learning）
让智能体在与环境的交互中通过“试错”来学习策略。
- 强化学习要素： 智能体（Agent）、环境（Environment）、状态（State）、动作（Action）、奖励（Reward）。
- 马尔可夫决策过程（MDP）： 状态转移概率与折扣因子。
- 经典算法：
  - 基于价值的方法：Q-Learning, Deep Q-Network (DQN) 融合深度学习。
  - 基于策略的方法：Policy Gradient 简介。
- 应用场景： 游戏 AI（如 AlphaGo）、机器人控制、大模型对齐（RLHF）。
## 第 12 周：模型优化与部署
将模型从“实验室训练”推向“工业界落地”的必备技能。
- 过拟合应对策略： 正则化（L1/L2）、Dropout 机制、数据增强（Data Augmentation）。
- 规范化技术（Normalization）： 批规范化（Batch Normalization）与层规范化（Layer Normalization）的适用场景。
- 模型轻量化： 模型量化（Quantization，如 FP32 转 INT8）、模型剪枝（Pruning）、知识蒸馏（Knowledge Distillation）。
- 部署简介： 模型导出（ONNX 格式）、推理加速引擎（TensorRT）与云端/边缘端部署流程。
