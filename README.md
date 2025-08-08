# 🧠 Image Caption Generator: Custom Vs Pre-Trained CNN

This study presents an image captioning model using attention-based encoder-decoder architecture. We compare the performance of a custom CNN and three popular pre-trained CNNs (InceptionV3, ResNet50, and VGG16) for feature extraction. All feature sets are passed to a shared decoder (LSTM) that generates textual descriptions. The results show that pre-trained models, especially InceptionV3, significantly outperform custom CNNs in BLEU scores and generation fluency.

📌 This project is a part of our research paper:  
**“Image Caption Generator: Custom Vs Pre-Trained CNN”**

---

## 🚀 Features

- Custom CNN feature extractor vs. Pre-trained CNNs (InceptionV3, ResNet50, VGG16)
- Attention-based LSTM decoder for sequence generation
- BLEU Score evaluation for caption quality
- Cleanly organized modular codebase
- Training, inference, and attention visualization support
- Research paper included in `research_paper/` folder

---

## 📁 Dataset

We use the **Flickr8k** dataset:

- ~8,000 images with 5 captions each
- Dataset includes:
  - `Flickr8k_Dataset/` (Images)
  - `Flickr8k_text/Flickr8k.token.txt` (Captions)

> 📥 Download link for dataset:  
[Flickr8k Dataset on Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k)

> **Note:** The dataset is imported and preprocessed within the notebook scripts. Captions are cleaned and tokenized; image features are extracted and stored using NumPy arrays.

---

## 🧰 Tech Stack

- Python 3.10+
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib, PIL
- nltk
- tqdm

---

## 📖 How It Works

1. **Feature Extraction:** Images are passed through a custom CNN or a pre-trained CNN to extract dense feature vectors.
2. **Caption Encoding:** Captions are tokenized and padded, then fed into an LSTM-based decoder.
3. **Attention Mechanism:** The decoder uses an attention layer to selectively focus on image features while generating each word.
4. **Caption Generation:** The model generates captions word-by-word using greedy decoding or beam search.
5. **Evaluation:** Generated captions are evaluated using BLEU scores against the reference captions.

---

## 📑 Research Paper

You can access our published research paper here:  
🔗 [“Image Caption Generator: Custom Vs Pre-Trained CNN” – JERA Journal](https://alborearpress.com/jecra/jecraIssue)

---

## 👥 Contributors

This project was originally developed as part of a group academic project.

**Original Contributors:**

- Amil Gauri (Maintainer)  
- Vikas Pandit 
- Jayesh Patil  
- Ajay Chaurasiya

Project restructured, documented, and maintained by **Amil Gauri** for public release.

---

## 📄 License

This project is open-source under the **MIT License**.  
You are free to **use, modify, and distribute** it with proper credit.

See the [LICENSE](LICENSE) file for full details.

---