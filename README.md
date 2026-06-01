# 从向量到神经流形：大脑计算的几何原理 | From Vectors to Neural Manifolds: Geometric Principles of Brain Computation

---

## 中文版 | Chinese Version

### 📖 讲义介绍

这是一份面向**缺乏计算背景**的神经科学学生的教学讲义，旨在跨越数学与生物学的鸿沟，构建连贯的认知框架：

**向量 → 线性变换 → 频域（傅立叶/小波）→ 稀疏性 → 神经流形**

### 🎯 核心逻辑链

- **表示（Representation）**：神经元活动如何抽象为向量空间中的点与轨迹
- **变换（Transformation）**：神经网络如何通过矩阵运算与基变换（傅立叶/小波）处理信息
- **结构（Structure）**：这种处理如何在高维数据中显现低维几何结构（神经流形/拓扑）

### 📚 学习目标

完成本讲义，你将能够：

1. 把群体神经活动写成 $\mathbf{r}(t)\in\mathbb{R}^N$，并用"状态空间轨迹"思考
2. 用点积/余弦相似度解释"神经匹配""模板响应""去相���"
3. 用矩阵解释跨脑区投射与层间变换，并理解行列式（体积缩放）与特征值（动力学稳定性）
4. 把傅立叶变换理解为"坐标系变换"：时域基 → 频域基；理解欧拉公式的"旋转含义"
5. 面对非平稳神经信号，理解 STFT 的窗长权衡，并用小波实现多分辨率分析
6. 理解"稀疏性"为什么暗示低维结构，并自然过渡到"流形假设"
7. 用 PCA/Isomap 等方法在玩具数据上"展开纸团"，并理解环/环面/旋转动力学等典型结构
8. 了解 Takens 时间延迟嵌入：仅靠少量观测，也能恢复动力系统流形的拓扑结构（直觉版）

### 📑 讲义大纲

| 节 | 模块 | 主题 | 核心概念与技能 |
|---:|---|---|---|
| 1 | 基础 | 向量与神经编码 | 状态空间、轨迹、高维直觉（维数灾难/祝福） |
| 2 | 线代 | 矩阵与线性变换 | 矩阵乘法、行列式（体积）、特征值/特征向量 |
| 3 | 度量 | 相似度与几何距离 | 点积、余弦相似度、欧氏距离、赫布学习几何解释 |
| 4 | 频域 | 傅立叶变换基础 | 正弦基、幅值/相位、功率谱 |
| 5 | 复数 | 欧拉公式与旋转 | 复平面、旋转矩阵、相位编码、旋转动力学 |
| 6 | 非平稳 | STFT 与测不准 | 加窗、谱图、时频权衡 |
| 7 | 小波 | 多分辨率与重构 | 母小波、尺度/平移、MRA、能量图 |
| 8 | 过渡 | 稀疏编码与降维 | 感受野作为基、稀疏性、去噪、PCA 局限 |
| 9 | 流形 | 流形假设与拓扑 | 揉皱纸团、内蕴维度 vs 外嵌维度、测地线 |
| 10 | 实例 | 环形吸引子与 HD | 连续吸引子、1D 环流形、头朝向解码直觉 |
| 11 | 实例 | 环面与网格细胞 | torus 直觉、周期边界、TDA 概念入口 |
| 12 | 应用 | 动力学与重构/解码 | 旋转动力学、Takens 嵌入、基于流形的解码 |

### 🚀 快速开始

#### 📱 在线运行（推荐）- 一键打开

**点击下方按钮直接在浏览器中打开并运行讲义：**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/blob/main/20260121%E4%BB%8E%E5%90%91%E9%87%8F%E5%88%B0%E7%A5%9E%E7%BB%8F%E6%B5%81%E5%BD%A2%E8%AE%B2%E4%B9%89.ipynb)

**优点：**
- ✅ 无需安装任何软件
- ✅ 免费使用 GPU/TPU
- ✅ 所有依赖预装
- ✅ 支持保存您的修改

#### 💻 本地运行

1. 克隆仓库：
```bash
git clone https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds.git
cd From-Vectors-to-Neural-Manifolds
```

2. 安装依赖：
```bash
pip install numpy matplotlib scipy pywavelets scikit-learn jupyter
```

3. 启动 Jupyter：
```bash
jupyter notebook "20260121从向量到神经流形讲义.ipynb"
```

### 📦 依赖环境

- **Python** 3.7+
- **numpy** - 数值计算
- **matplotlib** - 绘图
- **scipy** - 信号处理
- **pywavelets** - 小波变换
- **scikit-learn** - 机器学习与降维

### ✨ 讲义特点

- 📝 **由浅入深**：每一节遵循"当前问题 → 如何解决 → 推导到下一步"的逻辑
- 💡 **直觉优先**：先建立几何直觉，再给出数学形式
- 🎨 **丰富的可视化**：每个概念配合交互式图示
- 🧪 **玩具数据演示**：在瑞士卷、环形吸引子等典型例子上展示
- 🔗 **知识串联**：从向量的点积一路到流形的拓扑性质

### 🧠 适用人群

- 计算神经科学的初学者
- 想理解神经信号处理数学基础的研究者
- 对大脑几何结构感兴趣的学生
- 想了解维数约简和流形学习在神经科学中应用的人

### 📖 建议学习方式

1. **按顺序阅读**：讲义设计成递进式，后续章节依赖前面的概念
2. **动手复现**：修改代码参数，观察不同的可视化结果
3. **做笔记**：在每个核心概念处暂停，用自己的话复述一遍
4. **对比理论与实验**：用真实神经数据与讲义中的玩具例子做类比

### 📞 反馈与贡献

如有建议、错误或改进方向，欢迎：
- 提出 [Issues](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/issues)
- 提交 [Pull Requests](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/pulls)

---

## English Version | 英文版

### 📖 About This Lecture

This is a comprehensive teaching guide designed for **neuroscience students without computational backgrounds**, bridging the gap between mathematics and biology through a coherent cognitive framework:

**Vectors → Linear Transformations → Frequency Domain (Fourier/Wavelets) → Sparsity → Neural Manifolds**

### 🎯 Core Logic Chain

- **Representation**: How neural activity translates into points and trajectories in vector space
- **Transformation**: How neural networks process information through matrix operations and basis transformations (Fourier/wavelets)
- **Structure**: How this processing reveals low-dimensional geometric structures in high-dimensional data (neural manifolds/topology)

### 📚 Learning Objectives

Upon completing this lecture, you will be able to:

1. Express population neural activity as $\mathbf{r}(t)\in\mathbb{R}^N$ and reason about "neural state space trajectories"
2. Use dot products and cosine similarity to interpret "neural matching," "template responses," and "decorrelation"
3. Use matrices to explain inter-region projections and inter-layer transformations, and understand determinants (volume scaling) and eigenvalues (dynamic stability)
4. Understand Fourier transforms as "coordinate system transformations": time domain basis → frequency domain basis; grasp the "rotational meaning" of Euler's formula
5. Handle non-stationary neural signals: understand STFT window-length tradeoffs and multi-resolution analysis via wavelets
6. Understand why "sparsity" implies low-dimensional structure and naturally transition to the "manifold hypothesis"
7. Use methods like PCA/Isomap to "unfold crumpled paper" on toy data; understand typical structures like rings/tori/rotational dynamics
8. Learn about Takens time-delay embedding: how to recover the topology of dynamical system manifolds from limited observations (intuitive version)

### 📑 Lecture Outline

| Section | Module | Topic | Core Concepts & Skills |
|---:|---|---|---|
| 1 | Fundamentals | Vectors & Neural Coding | State space, trajectories, high-dimensional intuition (curse/blessing of dimensionality) |
| 2 | Linear Algebra | Matrices & Linear Transforms | Matrix multiplication, determinants (volume), eigenvalues/eigenvectors |
| 3 | Metrics | Similarity & Geometric Distance | Dot products, cosine similarity, Euclidean distance, Hebbian learning geometry |
| 4 | Frequency Domain | Fourier Transform Basics | Sine bases, magnitude/phase, power spectra |
| 5 | Complex Numbers | Euler's Formula & Rotation | Complex plane, rotation matrices, phase encoding, rotational dynamics |
| 6 | Non-Stationary | STFT & Uncertainty | Windowing, spectrograms, time-frequency tradeoff |
| 7 | Wavelets | Multi-resolution & Reconstruction | Mother wavelets, scale/shift, MRA, energy plots |
| 8 | Transition | Sparse Coding & Dimensionality Reduction | Receptive fields as bases, sparsity, denoising, PCA limitations |
| 9 | Manifolds | Manifold Hypothesis & Topology | Crumpled paper analogy, intrinsic vs. extrinsic dimension, geodesics |
| 10 | Example | Ring Attractors & HD Cells | Continuous attractors, 1D ring manifolds, head direction decoding intuition |
| 11 | Example | Torus & Grid Cells | Torus intuition, periodic boundaries, TDA conceptual entry |
| 12 | Applications | Dynamics & Reconstruction/Decoding | Rotational dynamics, Takens embedding, manifold-based decoding |

### 🚀 Quick Start

#### 📱 Run Online (Recommended) - One Click

**Click the button below to open and run the lecture directly in your browser:**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/blob/main/20260121%E4%BB%8E%E5%90%91%E9%87%8F%E5%88%B0%E7%A5%9E%E7%BB%8F%E6%B5%81%E5%BD%A2%E8%AE%B2%E4%B9%89.ipynb)

**Advantages:**
- ✅ No software installation required
- ✅ Free access to GPU/TPU
- ✅ All dependencies pre-installed
- ✅ Save your modifications

#### 💻 Run Locally

1. Clone the repository:
```bash
git clone https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds.git
cd From-Vectors-to-Neural-Manifolds
```

2. Install dependencies:
```bash
pip install numpy matplotlib scipy pywavelets scikit-learn jupyter
```

3. Launch Jupyter:
```bash
jupyter notebook "20260121从向量到神经流形讲义.ipynb"
```

### 📦 Requirements

- **Python** 3.7+
- **numpy** - Numerical computing
- **matplotlib** - Data visualization
- **scipy** - Signal processing
- **pywavelets** - Wavelet transforms
- **scikit-learn** - Machine learning & dimensionality reduction

### ✨ Key Features

- 📝 **Progressive Difficulty**: Each section follows the logic: "Current Problem → Solution → Transition to Next Topic"
- 💡 **Intuition First**: Geometric intuition precedes mathematical formalism
- 🎨 **Rich Visualizations**: Every concept paired with interactive illustrations
- 🧪 **Toy Data Demonstrations**: Showcase concepts using Swiss rolls, ring attractors, and other canonical examples
- 🔗 **Knowledge Integration**: Continuous thread from dot products of vectors to topological properties of manifolds

### 🧠 Target Audience

- Beginners in computational neuroscience
- Researchers seeking mathematical foundations of neural signal processing
- Students interested in geometric structures in the brain
- Anyone curious about dimensionality reduction and manifold learning applications in neuroscience

### 📖 Recommended Learning Approach

1. **Read Sequentially**: The lecture is designed as a progression; later chapters depend on earlier concepts
2. **Hands-On Coding**: Modify code parameters and observe different visualizations
3. **Take Notes**: Pause at each key concept and rephrase it in your own words
4. **Compare Theory & Practice**: Draw parallels between real neural data and toy examples in the lecture

### 📞 Feedback & Contributions

We welcome suggestions, bug reports, and improvements:
- Open an [Issue](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/issues)
- Submit a [Pull Request](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/pulls)

---

## 📄 License | 许可证

This lecture is freely available for use, modification, and sharing.
本讲义可自由使用、修改和分享。

---

## 🎓 Getting Started | 开始学习

**祝学习愉快！ | Happy learning!** 🚀

**从向量到神经流形的旅程，从现在开始！ | Begin your journey from vectors to neural manifolds today!**