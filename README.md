# Adaptive LLM Framework for Multi-Source Text Summarization

## 📌 Description
This project presents an **Adaptive Large Language Model (LLM) Framework** designed to generate high-quality summaries from multiple data sources such as YouTube videos, PDF documents, and textual content.

The system uses **Natural Language Processing (NLP)** techniques and **open-source Large Language Models (LLMs)** to automatically analyze input content, classify it as either **code-oriented or theory-based**, and dynamically select the most suitable model for summarization.

It also integrates **Automatic Speech Recognition (ASR)** to process videos without transcripts, making the system capable of handling both structured and unstructured data efficiently.

---

## 🚀 Features
- Multi-source input (Text, PDF, YouTube)
- Automatic Speech Recognition (ASR) for videos without transcripts
- Content classification (Coding vs Theory)
- Adaptive model selection
- Transformer-based summarization
- Fast and automated processing
- User-friendly API interface

---

## ⚙️ Installation Steps

### 1. Clone the repository
```bash
git clone https://github.com/your-username/adaptive-llm-summarization.git
cd adaptive-llm-summarization



2. Install dependencies
pip install -r requirements.txt
▶️ How to Run the Code
python app.py

The server will start at:

http://127.0.0.1:5000/
📡 API Usage
Endpoint:
POST /summarize
Sample Request:
{
  "text": "Python is a programming language used for web development, AI, and data science."
}
Sample Response:
{
  "content_type": "Theory Content",
  "summary": "Python is a widely used programming language for applications like AI and web development."
}
🧠 Algorithm Explanation
1. Content Detection (Rule-Based)

The system uses a custom function detect_content_type() to classify input text.

Coding Content Detection:

Programming keywords (if, for, while, etc.)
Assignment patterns (x = 10)
Indentation structure
Symbols like ":" and "()"

Theory Content Detection:

Longer sentences
Natural language structure
Descriptive content
2. Adaptive Model Selection
Coding Content → Code-based model
Theory Content → General NLP model
3. Summarization
Uses transformer-based models (BART or similar)
Generates concise summaries
Maintains context and meaning
📊 Sample Input & Output
Input:
for i in range(5):
    print(i)
Output:
Content Type: Coding Content  
Summary: The code prints numbers from 0 to 4 using a loop.
📚 Technologies Used
Python
Flask
Hugging Face Transformers
NLP (NLTK, spaCy)
PyTorch
Whisper ASR
PyPDF2
📖 Citation Note (IMPORTANT)

This project is developed as part of the research work:

"Adaptive Large Language Model Framework for Multi-Source Text Summarization Using Open-Source Models"

If you use this code or build upon this work, please cite the corresponding research paper.

🔗 Repository & DOI
GitHub: https://github.com/Madhu-Priya-Sai/Final-Year-Project
DOI: https://doi.org/10.5281/zenodo.19230012
🙌 Acknowledgment

This project was developed as part of a Bachelor of Technology (B.Tech) final year project in Information Technology.
