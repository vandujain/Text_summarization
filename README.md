# 📝 Text Summarization Project

This project focuses on building an **automated text summarization system** that generates concise and coherent summaries from long text documents, especially news articles. It uses a **transformer-based model** to extract key insights while preserving the original context.

---

## 🎯 Objectives

- Summarize long documents into short, meaningful texts.
- Preserve the context, key points, and tone of the source material.
- Evaluate summary quality based on coherence and accuracy.

---

## 🧠 Technologies Used

- **Python**
- **Hugging Face Transformers**
- **BART-based model**: `sshleifer/distilbart-cnn-12-6`
- **NewsAPI** for live data
- **Requests** for API calls

---

## 📥 Input Data

- Live news articles fetched via a **News API** (e.g., `https://newsapi.org`)
- Only articles with non-empty `content` are considered for summarization

---

## 🔄 Workflow

1. **Fetch Data**:
   - Use the News API to retrieve real-time articles.
2. **Clean and Prepare**:
   - Filter empty articles.
3. **Summarization**:
   - Generate summaries using Hugging Face's `pipeline("summarization")`
4. **Output**:
   - Display or store summaries of top articles.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/text-summarization.git
cd text-summarization
