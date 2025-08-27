# Turkish Offensive Language Detection (Lexicon + BERTurk)

![Python](https://img.shields.io/badge/python-3.9%2B-blue)  
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-orange)  
![Transformers](https://img.shields.io/badge/HF-Transformers-purple)  
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)  
![Gradio](https://img.shields.io/badge/Gradio-UI-green)  

This project detects offensive/abusive language in Turkish text using a **two-layer system**:

1. **Lexicon-based masking** – normalizes obfuscations and masks offensive words.  
2. **Contextual classification (BERTurk)** – fine-tuned `dbmdz/bert-base-turkish-cased` model for detecting abusive context.

---

## 🚀 Features
- Turkish-specific text normalization.  
- Lexicon-based profanity masking.  
- Baseline: TF-IDF + Logistic Regression.  
- Advanced: Fine-tuned BERTurk model.  
- Simple Gradio demo for testing.  

---

## 📚 Dataset
- [TROFF v1.0 (Turkish Offensive Language Dataset)](https://coltekin.github.io/offensive-turkish/troff-v1.0.tsv.gz)  
- [Turkish Swear Word Lexicons](https://github.com/ooguz/turkce-kufur-karaliste), [d35k/Turkish-Swear-Words](https://github.com/d35k/Turkish-Swear-Words)

---

## 📦 Installation
```bash
pip install -r requirements.txt
```

---


### Example
```
Input:   sen gerçekten çok salakça konuşuyorsun
Output:  FLAG | score=0.87
```

---

