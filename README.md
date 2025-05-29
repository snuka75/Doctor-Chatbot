# 🩺 Qwen Doctor Chatbot

An intelligent medical chatbot **fine-tuned using the Qwen 1.8B model** on a large set of real-world doctor-patient conversations. This model is **deployed as a live chatbot on Hugging Face Spaces** using Gradio UI.

![Chatbot Screenshot](screenshots/chatbot.png)

---

## 🚀 Project Highlights

✅ Fine-tuned Qwen model with LoRA adapters using 100K+ doctor-patient Q&A pairs  
✅ Achieved **BERTScore F1 of 0.8272** showing strong response quality  
✅ **Deployed chatbot on Hugging Face Space** for real-time interaction  
✅ Built intuitive Gradio interface for easy use  

---

## 📁 Project Structure

```bash
├── app.py                        # Gradio app for chatbot interface
├── finetuningqwenfordoctorchat.py  # Fine-tuning code (LoRA + Transformers)
├── adapter_config.json           # Configuration for LoRA adapter
├── requirements.txt              # Dependencies for app
├── README.md                     # This file              
└── .gitattributes                # HF Spaces config
```

---

## 🤖 Model Details

- **Base Model**: Qwen 1.8B
- **Fine-tuning Method**: LoRA (Parameter Efficient Fine-Tuning)
- **Dataset**: [HealthCareMagic-100k](https://www.kaggle.com/datasets/punyaslokaprusty/chatdoctor)
- **Platform**: Google Colab + RunPod
- **Training Time**: ~3 hours (on T4 GPU)
- **Deployed To**: Hugging Face 🤗 Spaces

---

## 📊 Evaluation Metrics

| Metric             | Value    |
|--------------------|----------|
| Training Loss      | ~1.83    |
| **BERTScore F1**   | **0.8272** |
| Epochs             | 3        |
| Model Size         | 1.8B     |

---

## 🧪 Sample Questions You Can Ask

- *What are the symptoms of a kidney infection?*  
- *Can I take ibuprofen with paracetamol?*  
- *What causes chest pain after eating?*  
- *Is it safe to exercise with a cold?*  

---

## 🌐 Live Demo

Try the chatbot on Hugging Face Space:

👉 [Qwen Doctor Chatbot on Hugging Face](https://huggingface.co/spaces/snuka75/qwen-doctor-chat)

---

## 💻 Running Locally

1. **Clone the repo**:
```bash
git clone https://github.com/YOUR_USERNAME/qwen-doctor-chat.git
cd qwen-doctor-chat
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```
---

## 🧠 Tech Stack

- `Qwen 1.8B` with `LoRA` fine-tuning via `PEFT`
- `Transformers` from Hugging Face
- `Gradio` for live UI
- `Colab` + `RunPod` GPU for training
- `BERTScore` for evaluation

---

## 📷 Screenshots

![Chatbot UI](screenshots/chatbot.png)

---

## 🙏 Acknowledgments

- [Qwen by Alibaba](https://huggingface.co/Qwen)
- [HealthcareMagic Dataset](https://www.kaggle.com/punyaslokaprusty/chatdoctor)
- [PEFT by Hugging Face](https://github.com/huggingface/peft)
- [Gradio UI]([https://89ad3a3fcd195b4bf6.gradio.live])

---

## 🔮 Future Enhancements

- Add more domain-specific medical datasets (MedQA, PubMedQA)
- Support multilingual chat
- Add voice interaction (text-to-speech/speech-to-text)
- Save user query logs for feedback

