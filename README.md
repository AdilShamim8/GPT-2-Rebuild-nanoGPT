# GPT-2 Rebuild nanoGPT

A step-by-step implementation of nanoGPT inspired by Andrej Karpathy's Neural Networks: Zero To Hero lecture series.

## Introduction

This repository contains my implementation of nanoGPT following Andrej Karpathy's excellent [lecture](https://youtu.be/kCc8FmEb1nY?feature=shared). The goal is to provide a clear, educational walkthrough of building a GPT-2 style language model from scratch, making the concepts accessible to beginners and enthusiasts alike.

By following this repository, you'll gain hands-on experience with:
- Transformer architecture implementation
- Training language models
- Text generation using GPT-2 style models
- PyTorch fundamentals in a practical context

## Project Overview

This project is a direct adaptation of [@karpathy/ng-video-lecture](https://github.com/karpathy/ng-video-lecture), aiming to reproduce the code created during the Neural Networks: Zero To Hero video series. The implementation focuses on clarity and educational value rather than production-ready performance.

## Getting Started

### Prerequisites

- Python 3.6+
- PyTorch 1.0+
- NumPy
- Additional dependencies in `requirements.txt`

### Installation

```bash
# Clone the repository
git clone https://github.com/AdilShamim8/GPT-2-Rebuild-nanoGPT.git
cd GPT-2-Rebuild-nanoGPT

# Install dependencies
pip install -r requirements.txt
```

## Usage

### Training a Model

```bash
python train.py
```

### Generating Text

```bash
python generate.py
```

### Model Parameters

You can customize various aspects of the model by adjusting parameters in the configuration files:
- Model size (number of layers, embedding dimensions)
- Training hyperparameters (learning rate, batch size)
- Text generation settings (temperature, max length)

## Implementation Notes

As noted in the original repository:

> Sadly I did not go too much into model initialization in the video lecture, but it is quite important for good performance. The current code will train and work fine, but its convergence is slower than it could be with better initialization.

This repository includes improved initialization methods to enhance training efficiency while maintaining the educational clarity of the original implementation.

## Project Structure

```
├── data/               # Training data
├── models/             # Model definitions
├── utils/              # Helper functions
├── train.py            # Training script
├── generate.py         # Text generation script
├── config.py           # Configuration settings
└── README.md           # This file
```

## Learning Resources

For a deeper understanding of the concepts implemented here:
- [Neural Networks: Zero To Hero](https://karpathy.ai/zero-to-hero.html) video lecture series
- [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) by Jay Alammar
- [GPT-2 Paper](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) by OpenAI

## Contributing

Contributions to improve the implementation or documentation are welcome! Please feel free to submit a pull request or open an issue.

## Acknowledgments

This project is based on Andrej Karpathy's [ng-video-lecture](https://github.com/karpathy/ng-video-lecture) repository and his Neural Networks: Zero To Hero lecture series. All credit for the original implementation and concepts goes to him.

## License

This project is licensed under the MIT License - see the LICENSE file for details, following the same licensing as the original repository.

---

Created by [AdilShamim8](https://github.com/AdilShamim8) | Last updated: 2025-09-16
