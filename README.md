# 🧠 Building LLM from Scratch

Learn how to build a Large Language Model (LLM) from scratch using Python, PyTorch, and transformer architectures.

<p align="center">
  <a href="https://github.com/your-username/llm-scratch/issues"><img src="https://img.shields.io/github/issues/your-username/llm-scratch"></a> 
  <a href="https://github.com/your-username/llm-scratch/stargazers"><img src="https://img.shields.io/github/stars/your-username/llm-scratch"></a>
  <a href="https://github.com/your-username/llm-scratch/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg">
  </a>
</p>

<p align="center">
  <a href="#-features">Features</a> |
  <a href="#%EF%B8%8F-tech-stack">Tech Stack</a> |
  <a href="#-installation">Installation</a> |
  <a href="#-contributing">Contributing</a> |
  <a href="#%EF%B8%8F-author">Author</a>
</p>

## 🌟 Features

- Train your own LLM from scratch with minimal dependencies.
- Use transformer architectures and attention mechanisms.
- Option to train on OpenWebText corpus or a fallback mini-dataset.
- Compatible with CPU and CUDA-enabled GPUs.
- Supports compression using LZMA for preprocessing.
- Ready-to-use notebook version available via Google Colab.

## 🛠️ Tech Stack

- **Language**: Python 3.10+
- **Deep Learning Framework**: PyTorch
- **Data Processing**: NumPy, pylzma
- **Environment**: Jupyter / Google Colab

## 🚀 Installation

### Requirements 📋

- Python 3.10+
- Pip
- Jupyter Notebook or Google Colab
- (Optional) NVIDIA GPU with CUDA 11.8

### Local Setup 🧑‍💻

1. Clone the repository:

```bash
git clone https://github.com/TechFreak2003/LLM_from_scratch
cd LLM_from_scratch
```

2. Install dependencies:

```bash
pip install pylzma numpy ipykernel jupyter torch --index-url https://download.pytorch.org/whl/cu118
```

> If you don’t have a CUDA-compatible GPU, it will automatically fall back to CPU:
```python
device = 'cuda' if torch.cuda.is_available() else 'cpu'
```

> ⚠️ CPU mode works but will result in slower runtimes.

3. Download Visual Studio (for LZMA support on Windows):

🔗 [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/)

## 📂 Dataset

- Main dataset: [OpenWebText Corpus](https://skylion007.github.io/OpenWebTextCorpus/)
- If unavailable, use a fallback dataset (e.g., Wizard of Oz mini dataset) for training and validation.

## 📓 Google Colab

Try it out on Google Colab (no setup required):

▶️ [Open in Colab](https://colab.research.google.com/drive/1_7TNpEEl8xjHlr9JzKbK5AuDKXwAkHqj?usp=sharing)

## 📚 Key Research Papers

- [Attention is All You Need (Vaswani et al., 2017)](https://arxiv.org/pdf/1706.03762.pdf)
- [A Survey of LLMs (2023)](https://arxiv.org/pdf/2303.18223.pdf)
- [QLoRA: Efficient Finetuning of Quantized LLMs (2023)](https://arxiv.org/pdf/2305.14314.pdf)

## 📁 Project Structure

```
llm-scratch/
├── notebooks/
│   └── build_llm.ipynb         # Colab/Notebook implementation
├── dataset/                    # Data preprocessing and storage
├── model/                      # Transformer and LLM model code
├── utils/                      # Helper functions
├── README.md
└── requirements.txt
```

## 👥 Contributing

Contributions are welcome! Feel free to open issues, suggest improvements, or submit pull requests. Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 👨‍💻 Contributors

| Avatar | Name | GitHub | Role | Contributions |
|--------|------|--------|------|---------------|
| <img src="https://github.com/TechFreak2003.png" width="50px" height="50px" alt="TechFreak2003"/> | Suvrodeep Das | [TechFreak2003](https://github.com/TechFreak2003) | Project Creator & Maintainer | Core implementation, Documentation |

<!-- Future contributors will be added here automatically. -->

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Author

Maintained & Created by [Suvrodeep Das](https://suvrodeepdas.dev)  
Built to help others understand how large language models work at a low level.