\# Local LLM Image Gen Demo



This repository contains a Jupyter Notebook demonstrating how to generate images using \*\*Stable Diffusion\*\* with the Hugging Face `diffusers` library.  

It shows how to load a pre-trained model, run it locally, generate images from text prompts, and save the outputs.



---



\## 🚀 Features



\- Load a Stable Diffusion model from \*\*Hugging Face\*\* or locally.

\- Generate photorealistic images from text prompts.

\- Supports CPU and GPU (if available).

\- Save generated images to disk.

\- Optionally generate multiple images per prompt.



---



\## 📦 Requirements



\- Python 3.10 or higher

\- `torch==2.5.1+cu121`

\- `diffusers==0.35.2`

\- `huggingface\_hub==0.36.0`

\- `Pillow==12.0.0`



Install all dependencies using:



```bash

pip install -r requirements.txt



