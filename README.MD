# **Real-Time Swahili Speech Processing System**

## 📌 Abstract

This project focuses on developing a **real-time Swahili speech analysis system** that integrates **speech-to-text conversion, sentiment analysis, and text summarization**. Many **low-resource languages**, including Swahili, lack robust **automatic speech recognition (ASR) models** due to limited training data.

Using the **Mozilla Common Voice Swahili dataset (2022)**, we implemented a **machine learning pipeline** with pre-trained models:
- **Whisper** (speech-to-text)
- **DistilBERT** (sentiment analysis)
- **T5** (text summarization)

### **Key Findings**
✅ **Speech Recognition:** Achieved a **Word Error Rate (WER) of 3.99**, demonstrating high transcription accuracy.
✅ **Sentiment Analysis:** Reached **60% accuracy**, showing moderate success in Swahili emotion classification.
✅ **Text Summarization:** Faced challenges, with low **ROUGE scores** (ROUGE-1: 0.0917, ROUGE-2: 0.0600, ROUGE-L: 0.0917), indicating difficulties in summarizing Swahili text effectively.

To improve performance, **expanding Swahili training datasets** and **fine-tuning language-specific models** are essential. This research contributes to **bridging language barriers** and supports practical applications in **education, healthcare, and accessibility**.

---

## **🔹 Features**

✅ **Real-Time Speech-to-Text** – Converts Swahili audio into text using **OpenAI’s Whisper model**.
✅ **Sentiment Analysis** – Detects emotions in spoken language with **DistilBERT**.
✅ **Text Summarization** – Generates concise summaries using **T5 Transformer models**.
✅ **Interactive Dashboard** – Uses **Streamlit** for **real-time visualization and analysis**.
✅ **Audio Preprocessing** – Includes **noise reduction, silence trimming, and feature extraction**.
✅ **Performance Metrics** – Evaluates models using **WER, accuracy, F1-score, and ROUGE scores**.
✅ **User Feedback Loop** – Allows users to rate transcriptions and summaries to improve accuracy.

---

## **Getting Started**

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/swahili-speech-processing.git
cd swahili-speech-processing
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Run the Streamlit App**
```bash
streamlit run app.py
```

---

## **📂 Dataset**

The **Mozilla Common Voice 11.0 Swahili dataset** was used for model training and evaluation.
- **Source:** Mozilla Common Voice [Common Voice Datasets](https://commonvoice.mozilla.org/en/datasets)
- **Size:** **14.76 GB audio**, **753 transcribed Swahili sentences**
- **Collection:** Crowdsourced from **East African speakers** with diverse **accents and age groups**

---

## **🤖 Models Used**

| **Task**              | **Model**                                      | **Source** |
|----------------------|-----------------------------------------------|------------|
| **Speech-to-Text**   | Whisper (openai/whisper-medium)              | OpenAI     |
| **Sentiment Analysis** | DistilBERT (distilbert-base-uncased-finetuned-sst-2-english) | Hugging Face |
| **Text Summarization** | T5 (t5-base)                               | Hugging Face |

---

## **🔧 Usage Guide**

1️⃣ **Upload or Record Audio** – Use the Streamlit sidebar to upload or record Swahili speech.
2️⃣ **Real-Time Processing** – The system transcribes the audio, analyzes sentiment, and generates a summary.
3️⃣ **View Results** – The dashboard displays **text output, sentiment polarity, and summary**.
4️⃣ **Provide Feedback** – Users can rate the accuracy of transcriptions and sentiment analysis to refine the model.

---

## **📊 Model Performance**

| **Task**              | **Metric**  | **Score**  |
|----------------------|------------|-----------|
| **Speech-to-Text**   | WER        | **3.99%**  |
| **Sentiment Analysis** | Accuracy  | **60%**    |
| **Text Summarization** | ROUGE-1   | **0.0917** |
|                      | ROUGE-2   | **0.0600** |
|                      | ROUGE-L   | **0.0917** |

---

## **📡 Deployment**

✅ **Web Application:** Hosted using **Streamlit** for real-time speech processing.
✅ **Cloud Integration:** Uses **Google Colab** and **Hugging Face datasets** for efficient model execution.
✅ **Optimized Inference:** Runs on **ONNX Runtime** for **faster CPU-based predictions**.

---

## **🤝 Contributing**

Contributions are welcome! Feel free to:
- **Open an issue** for bug reports or feature requests.
- **Submit a pull request** to enhance functionality or fix issues.

---

## **Citation**

If you use this project, please cite:

```bibtex
@misc{mozilla_common_voice_2022,
  author       = {Mozilla Foundation},
  title        = {Mozilla Common Voice Dataset 11.0},
  year         = {2022},
  url          = {https://commonvoice.mozilla.org/en/datasets},
  howpublished = {Online Dataset},
  note         = {Accessed: January 8, 2025}
}
```

---

** Ready to Try It? Clone the Repo & Start Processing Swahili Speech Today!** 🎙️🤖

