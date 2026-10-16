# Building an LLM From Scratch 🚀

My learning journey through Sebastian Raschka’s *Build a Large Language Model (From Scratch)* — implementing the components, experimenting with code, and documenting what I learn.

For my experiments, I’m exploring **space and astronomy text**, starting with words like *spacetime*, *gravitational waves*, and *black holes*.

## Current Focus: Tokenization

I’m working through Chapter 2: **Working with Text Data**.

My first experiment explores how text becomes token IDs:

```text
Space text → Tokens → Token IDs
```

Questions I’m investigating:

- How do word-level and subword tokenization differ?
- How does BPE split scientific terms?
- Does capitalization or a leading space change the tokens?
- Can encoding and decoding reconstruct the original text?

The initial BPE experiments use GPT-2’s existing tokenizer through `tiktoken`. Implementing and training my own BPE tokenizer is a separate milestone.

## Project Roadmap

- [ ] Explore tokenization with space text
- [ ] Implement a BPE tokenizer from scratch
- [ ] Build token and positional embeddings
- [ ] Implement attention mechanisms
- [ ] Assemble a GPT-style model
- [ ] Explore pretraining and fine-tuning

## Setup

Requirements: Python, Git, and the `uv` package manager.

```powershell
git clone https://github.com/swarnima26796/llm-from-scratch.git
cd llm-from-scratch

uv venv --python 3.12
uv pip install -r requirements.txt
```

In VS Code:

1. Install the Microsoft **Python** and **Jupyter** extensions.
2. Select `.venv` as your Python interpreter.
3. Select the same environment as the kernel when opening notebooks.

## Learning Notes

This repository grows as I work through the book. Early experiments use small text samples to make the intermediate steps easy to inspect.

Tokenizing astronomy text does not train a language model or give it scientific knowledge. It prepares text for the later stages of the pipeline.

## References

- Build a Large Language Model from Scratch - by Sebastian Raschka

Code adapted from the book will be credited alongside my experiments.

---

Documenting the journey on Instagram: **@sassy_builds**
