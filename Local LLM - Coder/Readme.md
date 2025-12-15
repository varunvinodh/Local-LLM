# Local LLM Code Gen Demo

This repository contains a Jupyter Notebook demonstrating how to **download, quantize, and run a local large language model (LLM) for Python code generation** using Hugging Face Transformers and a 4-bit quantized Stable-Code-3B model.

The project showcases how to run a **code-focused LLM entirely locally** (no API calls after download), making it suitable for offline development, experimentation, and learning.

---

## 🚀 Features

- Download and save a Hugging Face code generation model locally
- Load the model using **4-bit quantization (NF4)** for reduced VRAM usage
- Automatic GPU device mapping
- Generate Python code from natural language prompts
- Fully local inference after initial setup
- Jupyter Notebook–based workflow for easy experimentation

---

## 📦 Requirements

### Hardware
- NVIDIA GPU (recommended)
- Compute capability **7.0+** (Turing or newer) for 4-bit quantization

### Software
- Python **3.9+**
- CUDA-enabled PyTorch installation

### Python Libraries
```txt
transformers
accelerate
bitsandbytes
torch
huggingface_hub
```
---

## ⚙️ Setup

1. **Create a Hugging Face account**: [https://huggingface.co](https://huggingface.co)  
2. **Generate a Personal Access Token (PAT)**: `Settings → Access Tokens → New token`.
3. **Install dependencies**: pip install -r requirements.txt
4. **Authenticate with Hugging Face (first run only)**: 
```from huggingface_hub import login
login()```
5. **Run the notebook**: jupyter notebook LocalCoderLLMDemo.ipynb

---


## 📝 Usage

1. LocalCoderLLMDemo.ipynb

2. Run the cells to:

- Download and save the Stable-Code-3B model locally
- Reload it using 4-bit quantization
- Provide a natural language prompt
- Generate Python code locally on your machine

**Example Prompt**: "Write a Python function that checks if a number is prime."

---

## 📂 Folder Structure
```

Local-CoderLLM-Demo/
├── LocalCoderLLMDemo.ipynb   # Main notebook
├── requirements.txt         # Python dependencies
├── README.md                # Project overview and instructions
├── .gitignore               # Files/folders to ignore
└── model/                   # Local model files (not committed due to size)
```


---

## 📝 Ending Notes:

- The model/ directory is intentionally excluded from version control due to its large size.
- After the initial download, no internet connection is required to run inference.
- This project is intended for educational and experimental purposes.
- You can easily swap in other Hugging Face causal language models for testing.

Happy coding! 🚀



