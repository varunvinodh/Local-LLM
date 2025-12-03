# Local LLM Image Gen Demo

This repository contains a Jupyter Notebook demonstrating how to generate images using **Stable Diffusion** with the Hugging Face `diffusers` library.  

It shows how to load a pre-trained model, run it locally, generate images from text prompts, and save the outputs.

---

## 🚀 Features

- Load a Stable Diffusion model from **Hugging Face** or locally.
- Generate photorealistic images from text prompts.
- Supports CPU and GPU (if available).
- Save generated images to disk.
- Optionally generate multiple images per prompt.

---

## 📦 Requirements

- Python 3.10 or higher
- `torch==2.5.1+cu121`
- `diffusers==0.35.2`
- `huggingface_hub==0.36.0`
- `Pillow==12.0.0`

Install all dependencies using:

```bash
pip install -r requirements.txt
```
---

## ⚙️ Setup

1. **Create a Hugging Face account**: [https://huggingface.co](https://huggingface.co)  
2. **Generate a Personal Access Token (PAT)**: `Settings → Access Tokens → New token`.

---

## 📝 Usage

1. **Open the Jupyter Notebook:**
- jupyter notebook stable_diffusion_demo.ipynb
2. **Run cells in order:**
- Authenticate with Hugging Face from login(token="PasteYourTokerHere")  
- Download and save the required model.
- load the local model.
- Generate images from text prompts.
- Save the generated images.

---

## 📂 Folder Structure
```
Local-LLM-Image-Gen-Demo/
├── stable_diffusion_demo.ipynb   # Main notebook
├── requirements.txt              # Python dependencies
├── README.md                     # Project overview and instructions
├── .gitignore                    # Files/folders to ignore
├── outputs/                      # generated images
└── model/                        # local model files (not committed due to the large size of the model)
```

---

## 📝 Ending Notes

- **CPU vs GPU:** The notebook runs on CPU by default. For faster image generation, you can run on a GPU if available.  
- **Model size:** Stable Diffusion models are large (several GBs). Make sure you have enough disk space if downloading locally.  
- **Hugging Face token:** Keep your token safe. Do not commit it to GitHub. Use `.env` or environment variables instead.  
- **Custom prompts:** Feel free to experiment with different text prompts to generate unique images.  
- **Multiple images:** Use `num_images_per_prompt` to generate more than one image per prompt.  
- **Outputs folder:** All generated images are saved in `outputs/` by default. You can change this path if desired.  

Happy image generating! 🎨
