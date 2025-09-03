# 🖼️ Image Captioning with CNN + Transformer  

This project implements an **Image Captioning model** using **deep learning**. It combines:  
- A **CNN encoder** (EfficientNet) to extract image features  
- A **Transformer encoder-decoder** to generate captions in natural language  

---

## 📊 Dataset  

The model uses the **Flickr8k dataset**, which contains 8,000 images with five captions each.  
Download inside the repo with:  
wget -q https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip
wget -q https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_text.zip
unzip -qq Flickr8k_Dataset.zip
unzip -qq Flickr8k_text.zip

⚙️ Installation

# Clone the repository
git clone https://github.com/your-username/image-captioning.git
cd image-captioning

# Install dependencies
pip install -r requirements.txt

🚀 Training

Run the training script:
python image_captioning.py
Training uses:
EfficientNetB0 as CNN encoder (pretrained on ImageNet)
Transformer with positional embeddings
Early stopping and learning rate scheduler

🎯 Inference
After training, the script can generate captions for random validation images.
Example output:

<img width="968" height="801" alt="image" src="https://github.com/user-attachments/assets/28eb44b5-468c-483e-9ba7-910618ee6ad5" />


📂 Project Structure

├── image_captioning.py   # Main script (training + inference)
├── data/                 # Flickr8k dataset (after download)
├── requirements.txt      # Python dependencies
└── README.md             # Documentation

📌 Features

CNN for visual feature extraction
Transformer encoder-decoder for caption generation
Data augmentation and preprocessing pipeline
BLEU score evaluation
Easily extendable to other datasets

📜 License
MIT License
