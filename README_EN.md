# From Vectors to Neural Manifolds: Geometric Principles of Brain Computation

## 📖 About This Lecture

This is a comprehensive teaching guide designed for **neuroscience students without computational backgrounds**, bridging the gap between mathematics and biology through a coherent cognitive framework:

**Vectors → Linear Transformations → Frequency Domain (Fourier/Wavelets) → Sparsity → Neural Manifolds**

### 🎯 Core Logic Chain

- **Representation**: How neural activity translates into points and trajectories in vector space
- **Transformation**: How neural networks process information through matrix operations and basis transformations (Fourier/wavelets)
- **Structure**: How this processing reveals low-dimensional geometric structures in high-dimensional data (neural manifolds/topology)

## 📚 Learning Objectives

Upon completing this lecture, you will be able to:

1. Express population neural activity as $\mathbf{r}(t)\in\mathbb{R}^N$ and reason about "neural state space trajectories"
2. Use dot products and cosine similarity to interpret "neural matching," "template responses," and "decorrelation"
3. Use matrices to explain inter-region projections and inter-layer transformations, and understand determinants (volume scaling) and eigenvalues (dynamic stability)
4. Understand Fourier transforms as "coordinate system transformations": time domain basis → frequency domain basis; grasp the "rotational meaning" of Euler's formula
5. Handle non-stationary neural signals: understand STFT window-length tradeoffs and multi-resolution analysis via wavelets
6. Understand why "sparsity" implies low-dimensional structure and naturally transition to the "manifold hypothesis"
7. Use methods like PCA/Isomap to "unfold crumpled paper" on toy data; understand typical structures like rings/tori/rotational dynamics
8. Learn about Takens time-delay embedding: how to recover the topology of dynamical system manifolds from limited observations (intuitive version)

## 📑 Lecture Outline

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

## 🚀 Quick Start

### 📱 Run Online (Recommended) - One Click

**Click the button below to open and run the lecture directly in your browser:**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/blob/main/20260121%E4%BB%8E%E5%90%91%E9%87%8F%E5%88%B0%E7%A5%9E%E7%BB%8F%E6%B5%81%E5%BD%A2%E8%AE%B2%E4%B9%89.ipynb)

**Or access directly via link:**

https://colab.research.google.com/github/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/blob/main/20260121%E4%BB%8E%E5%90%91%E9%87%8F%E5%88%B0%E7%A5%9E%E7%BB%8F%E6%B5%81%E5%BD%A2%E8%AE%B2%E4%B9%89.ipynb

**Advantages:**
- ✅ No software installation required
- ✅ Free access to GPU/TPU
- ✅ All dependencies pre-installed
- ✅ Save your modifications

### 💻 Run Locally

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

## 📦 Requirements

- **Python** 3.7+
- **numpy** - Numerical computing
- **matplotlib** - Data visualization
- **scipy** - Signal processing
- **pywavelets** - Wavelet transforms
- **scikit-learn** - Machine learning & dimensionality reduction

Most libraries are pre-installed in Colab; necessary installation commands are included in the lecture.

## ✨ Key Features

- 📝 **Progressive Difficulty**: Each section follows the logic: "Current Problem → Solution → Transition to Next Topic"
- 💡 **Intuition First**: Geometric intuition precedes mathematical formalism
- 🎨 **Rich Visualizations**: Every concept paired with interactive illustrations
- 🧪 **Toy Data Demonstrations**: Showcase concepts using Swiss rolls, ring attractors, and other canonical examples
- 🔗 **Knowledge Integration**: Continuous thread from dot products of vectors to topological properties of manifolds

## 🧠 Target Audience

- Beginners in computational neuroscience
- Researchers seeking mathematical foundations of neural signal processing
- Students interested in geometric structures in the brain
- Anyone curious about dimensionality reduction and manifold learning applications in neuroscience

## 📖 Recommended Learning Approach

1. **Read Sequentially**: The lecture is designed as a progression; later chapters depend on earlier concepts
2. **Hands-On Coding**: Modify code parameters and observe different visualizations
3. **Take Notes**: Pause at each key concept and rephrase it in your own words
4. **Compare Theory & Practice**: Draw parallels between real neural data and toy examples in the lecture

## 📞 Feedback & Contributions

We welcome suggestions, bug reports, and improvements:
- Open an [Issue](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/issues)
- Submit a [Pull Request](https://github.com/Vincent-B-Faust/From-Vectors-to-Neural-Manifolds/pulls)

## 📄 License

This lecture is freely available for use, modification, and sharing.

---

**Happy learning!** 🎓

Begin your journey from vectors to neural manifolds today!