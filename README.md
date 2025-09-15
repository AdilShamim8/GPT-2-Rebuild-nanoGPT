# GPT-2 Rebuild nanoGPT

Welcome to **GPT-2 Rebuild nanoGPT**!  
This repository is a friendly, beginner-accessible, step-by-step reproduction of [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt), inspired by [Andrej Karpathy's YouTube lecture](https://youtu.be/l8pRSuU81PU?feature=shared). The goal is to help you understand and experiment with the core ideas behind transformer-based language models like GPT-2, with simple code, clear documentation, and community support.

---

## Table of Contents

- [Introduction](#introduction)
- [Project Inspiration & Credits](#project-inspiration--credits)
- [Overview of @karpathy/build-nanogpt](#overview-of-karpathybuild-nanogpt)
- [Key Features](#key-features)
- [System Requirements](#system-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Visual Guide](#visual-guide)
- [Troubleshooting](#troubleshooting)
- [Contribution Guidelines](#contribution-guidelines)
- [License](#license)
- [FAQs](#faqs)
- [Additional Resources](#additional-resources)
- [Community](#community)
- [Contact](#contact)

---

## Introduction

**GPT-2 Rebuild nanoGPT** is for anyone who wants to learn how large language models like GPT-2 work—by building one from scratch! This project guides you through each step, with code and explanations closely following [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt) and Karpathy's [YouTube lecture](https://youtu.be/l8pRSuU81PU?feature=shared).

You'll see how transformers process text, how training works, and how to generate your own language model outputs. The code is kept clean and beginner-friendly, so you can follow along even if you're new to deep learning.

---

## Project Inspiration & Credits

- **Original inspiration:** [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt) — an educational, from-scratch reproduction of GPT-2 (nanoGPT) by Andrej Karpathy.
- **Lecture reference:** [Let's reproduce GPT-2 (124M) — YouTube Lecture](https://youtu.be/l8pRSuU81PU?feature=shared)
- **Huge thanks** to Andrej Karpathy and the open research community for making these resources available!

---

## Overview of @karpathy/build-nanogpt

[@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt) is a clean, step-by-step educational repo that builds a small GPT-2-like model from scratch using PyTorch. The repository's commit history is structured so you can follow the evolution of the model line by line. It focuses on learning and transparency, not on production readiness.

Sample outputs from the original project:

```
Hello, I'm a language model, and my goal is to make English as easy and fun as possible for everyone, and to find out the different grammar rules
...
```

After extensive training, the model generates more sophisticated outputs, showcasing the learning process.

---

## Key Features

- **Educational Focus:** Code and explanations are beginner-friendly, emphasizing clarity over complexity.
- **Minimal Dependencies:** Runs with just Python and PyTorch.
- **Step-by-Step Evolution:** Each part of the model is built up gradually, mirroring the approach in [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt).
- **Customizable:** Train on your own text files, tweak model parameters, and experiment freely.
- **Community-Oriented:** Open for questions, discussions, and contributions.

---

## System Requirements

- Python 3.8 or newer
- pip (Python package manager)
- PyTorch (see [installation guide](https://pytorch.org/get-started/locally/))
- Works on Windows, macOS, and Linux
- (Optional) CUDA-enabled GPU for faster training

**Recommended:**  
- At least 4GB RAM  
- (Optional) NVIDIA GPU with 4GB+ VRAM for efficient training

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT.git
   cd GPT-2-Rebuild-nanoGPT
   ```

2. **(Recommended) Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### 1. **Prepare your dataset**
Place your training text (e.g., `input.txt`) in the project directory.

### 2. **Train the model**
```bash
python train.py --data input.txt --epochs 10 --batch_size 64
```

### 3. **Generate text**
After training, sample new text:
```bash
python generate.py --checkpoint model_checkpoint.pt --prompt "Once upon a time"
```

### 4. **Configuration**
- Model and training parameters can be tweaked in `config.py`.

---

## Visual Guide

Below is a simplified diagram of the transformer language model pipeline:

```
[Input Text] → [Tokenizer] → [Embedding Layer] → [Transformer Blocks] → [Output Layer] → [Generated Text]
```

![Transformer Diagram](https://raw.githubusercontent.com/karpathy/build-nanogpt/main/docs/transformer-diagram.png)

---

## Troubleshooting

- **Missing modules:** Run `pip install -r requirements.txt`.
- **CUDA errors:** If you don't have a GPU, set the device to CPU in your config.
- **Out of memory:** Lower batch size or model size in `config.py`.
- **Training is slow:** Use a smaller dataset or a GPU.

---

## Contribution Guidelines

We welcome all contributions!  
To contribute:

1. Fork this repo, then create a new branch:
   ```bash
   git checkout -b your-feature
   ```
2. Make your changes and commit:
   ```bash
   git commit -am 'Describe your change'
   ```
3. Push to your branch and open a Pull Request.

For more, see [CONTRIBUTING.md](CONTRIBUTING.md) (coming soon!).

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## FAQs

**Q: Do I need a GPU?**  
A: No, but a GPU is recommended for faster training. CPU works, just slower.

**Q: Can I use my own dataset?**  
A: Yes! Replace `input.txt` with your own text file.

**Q: I'm new to deep learning, can I follow along?**  
A: Absolutely! The code and documentation are written for beginners.

**Q: Where can I ask questions or get help?**  
A: Use [Discussions](https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT/discussions) or [open an issue](https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT/issues).

---

## Additional Resources

- [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt)
- [YouTube Lecture](https://youtu.be/l8pRSuU81PU?feature=shared)
- [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)
- [GPT-2 Paper (OpenAI)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
- [PyTorch Docs](https://pytorch.org/docs/stable/index.html)

---

## Community

- **Discussions:** [GitHub Discussions](https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT/discussions)
- **Chat:** [Discord (Zero To Hero)](https://discord.gg/3zy8kqD9Cp)
- **Twitter:** [@karpathy](https://twitter.com/karpathy)

---

## Contact

For questions or suggestions, open an [issue](https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT/issues)  
or contact the maintainer: [AdilShamim8](https://github.com/AdilShamim8) | adilshamim8@gmail.com

---

> **Credit:**  
> This project is heavily inspired by [@karpathy/build-nanogpt](https://github.com/karpathy/build-nanogpt) and follows the structure and educational intent of the original.  
> Please see [the original README](https://github.com/karpathy/build-nanogpt/blob/main/README.md) for more context, errata, and production advice.
