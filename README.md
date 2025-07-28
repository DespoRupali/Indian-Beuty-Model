# Fooocus + Indian Beuty Model Setup

This README guides you through setting up the [Fooocus](https://github.com/lllyasviel/Fooocus) AI-powered image generation tool with the **Indian Beuty** model from Civitai.

---

## 📦 Requirements

- Python environment (e.g., Google Colab, Jupyter Notebook, or local setup)
- Internet access to clone the repository and download the model
- A system with high VRAM is recommended (Colab Pro or equivalent)

---

## 🧭 Setup Steps Overview

1. Install the `pygit2` library required by Fooocus.
2. Clone the official Fooocus GitHub repository.
3. Navigate into the Fooocus directory.
4. Download the **Indian Beuty** model file into the `models/checkpoints/` folder.
5. Launch Fooocus with options enabled for high VRAM usage and sharing.

---

## 🧵 Model Information

- **Model Name:** Indian Beuty  
- **File Type:** `.safetensors`  
- **Download Link:** [Civitai – Indian Beuty](https://civitai.com/models/299307/indian-beuty)  
- **Description:** Designed to generate Indian-themed photorealistic female portraits and styles.

---

## 💻 Commands to Run

```bash
# Step 1: Install required packages
!pip install pygit2==1.15.1

# Step 2: Clone Fooocus repo
%cd /content
!git clone https://github.com/lllyasviel/Fooocus.git
%cd /content/Fooocus

# Step 3: Download the "Indian Beuty" model
!wget -O /content/Fooocus/models/checkpoints/Indian\ Beuty.safetensors https://civitai.com/models/299307/indian-beuty

# Step 4: Launch Fooocus
!python entry_with_update.py --share --always-high-vram
