# ETMMGA304 – Generative AI Lab Files

Includes four Colab-ready notebooks and the capstone Streamlit app:
- Lab 1: VAE on MNIST
- Lab 2: GAN on Fashion-MNIST
- Lab 3: GPT-2 text generation and fine-tuning
- Lab 4: Stable Diffusion prompt-to-image
- app.py: Study Tip Generator interface

## Run
The manual is designed for Google Colab. Upload one notebook at a time, run cells from top to bottom, and select a GPU runtime for Labs 1, 2 and 4. Lab 3 can run on CPU but fine-tuning is faster on GPU. Internet is needed for first-time downloads.

For local Windows use, create a project-local environment:
```powershell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install torch torchvision matplotlib pandas transformers diffusers accelerate safetensors streamlit
```
Select `.venv` as the VS Code/Jupyter interpreter. Stable Diffusion requires a compatible GPU for practical use.

After Lab 3 exports `lab_outputs/study_tip_gpt2`, run the capstone:
```powershell
streamlit run app.py
```

Complete observation tables using your actual outputs, losses and screenshots. Do not invent measurements or scores.
