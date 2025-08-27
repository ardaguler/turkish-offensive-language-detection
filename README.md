# Turkish Offensive Language Detection (Lexicon + BERTurk)

![Python](https://img.shields.io/badge/python-3.9%2B-blue)  
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-orange)  
![Transformers](https://img.shields.io/badge/HF-Transformers-purple)  
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)  
![Gradio](https://img.shields.io/badge/Gradio-UI-green)  

This repository implements a **two-layer moderation system** for detecting offensive/abusive language in Turkish text.

1. **Lexicon-based masking**: Normalizes obfuscations, replaces offensive terms with `***`, while preserving spacing.  
2. **Contextual classification with BERTurk**: Fine-tunes `dbmdz/bert-base-turkish-cased` to classify text into **FLAG / REVIEW / OK** decisions using a dual-threshold policy.

## Installation
```bash
pip install -r requirements.txt
```

## Usage
Open the Jupyter notebook and run all cells.  
Example input for Gradio demo:
```
sen SALAK mısın amk?
```

## License
Distributed under the MIT License. See `LICENSE` for details.
