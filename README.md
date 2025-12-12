
# 📘 Local LLM Playground — Colab Experiments (Transformers • ctransformers • Gemini API)

This repository contains a Google Colab notebook designed as a comprehensive playground for experimenting with different Large Language Models (LLMs) using:

- 🤖 HuggingFace Transformers  
- ⚡ ctransformers (GGUF Local Inference)  
- 🔥 Google Gemini API  
- 🧠 Prompting & Chat Templates  
- 🧪 Multiple Model Architectures (TinyLlama, Mistral, Phi, Qwen, etc.)

The notebook serves as a practical environment for learning, testing, comparing, and debugging LLM behavior in a single place.

---

## 🚀 Features

### ✔ Multiple LLM Backends
- HuggingFace Transformers (AutoModelForCausalLM + pipeline)
- ctransformers GGUF inference for running LLMs offline
- Google Gemini API for cloud-based high-quality generation

### ✔ Chatbot Implementations
- Custom Python chat loops  
- Multi-turn conversation handling  
- Consistent response formatting  
- Drift reduction techniques  

### ✔ Prompt Template Experiments
- LLaMA `[INST] ... [/INST]` format  
- Alpaca/Vicuna `### Instruction:` format  
- System/User role formatting  
- Gemini-style prompting  

### ✔ Model Comparison (Qualitative)
- TinyLlama vs Mistral vs Phi vs Qwen behavior  
- Drift, blank output, and hallucination analysis  
- How chat templates affect model performance  
- Local vs API inference differences  

---

## 📂 Repository Contents

```
LLM-PLAYGROUND-COLAB/
│
├── LLM_.ipynb              # Main Colab notebook with all experiments
└── README.md               # Project documentation
```

---

## 🛠️ Requirements

Installable via Colab:

```bash
pip install transformers ctransformers google-generativeai langchain-google-genai huggingface_hub
```

---

## ▶️ How to Use

1. Open the notebook in Google Colab  
2. Install dependencies  
3. Choose a model backend:
   - HuggingFace Transformers  
   - GGUF model via ctransformers  
   - Gemini API  
4. Run chat functions to test responses  
5. Compare behavior between models  

---

## 🔍 What You Will Learn

- How transformers and decoder-only models work  
- How to run LLMs offline with GGUF  
- Why some GGUF models produce blank or drifted answers  
- How to format prompts correctly for each architecture  
- Differences between TinyLlama, Mistral, Phi, and Qwen  
- How to integrate Gemini API into custom chatbots  

---

## ⚠️ Known Limitations

- Some GGUF repos are removed or gated on HuggingFace  
- ctransformers does not support all architectures (e.g., Phi-2, Qwen2.x)  
- Mistral-based GGUF models may load but generate blank output  
- Chat templates must match model training format  
- Colab RAM may be insufficient for >4GB models  

These issues and solutions are documented inside the notebook.

---

## 🤝 Contributions

Feel free to:

- Add new model experiments  
- Add benchmarks or evaluations  
- Improve instructions or templates  
- Add UI (Gradio) or API (FastAPI) extensions  

---

## 📜 License

This project is intended for learning and experimentation.  
Check individual model licenses before production use.

---
