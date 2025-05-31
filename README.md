# 📚 Semantic Book Recommender

This is a semantic search–based book recommendation system that uses natural language processing to recommend books based on user input. Instead of relying on fixed keywords or categories, it understands the **meaning** behind your input using **sentence embeddings**.

### 🔍 How It Works

- Uses `sentence-transformers` (Hugging Face) to generate semantic embeddings from book descriptions.
- To create your own vector database, you’ll need a .env file in the root directory containing either your OpenAI API key or Hugging Face token.
- Stores and searches embeddings using FAISS (Facebook AI Similarity Search).
- A Gradio interface that allows users to enter a query and receive book recommendations.
- Input can be anything — a topic, mood, summary, or even a quote — and you'll get the most semantically relevant books.

---

## 🧰 Tech Stack

- **Python**
- **LangChain**
- **Hugging Face Transformers**
- **FAISS**
- **Gradio**
- **Pandas**
---
## 🔐 Environment Setup (Replit & Gitpod Users)

To run this project on **Replit** or **Gitpod**:

1. Copy the contents of `.env.example` into a new file named `.env` in the root directory.
2. Paste your Hugging Face token or OpenAI API key
---
[![Run on Replit](https://replit.com/badge/github/BusraRafa/Semantic-Book-Recommender)](https://replit.com/new/github/BusraRafa/Semantic-Book-Recommender)
---
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/BusraRafa/Semantic-Book-Recommender)
---
## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/BusraRafa/Semantic-Book-Recommender.git
cd Semantic-Book-Recommender
```
### 2. Create a Virtual Environment (optional but recommended)
```bash
python -m venv myenv
myenv\Scripts\activate.bat
```
### 3. Install Dependencies
A requirements.txt file containing all the project dependencies is provided as part of this repo.
``` bash
pip install -r requirements.txt
```
### 4. Run the Gradio App
```bash
python gradio-dashboard.py
```
Once launched, open the app in your browser at:
👉 http://127.0.0.1:7860

### To create a public shareable link, edit gradio-dashboard.py and modify:
```bash
dashboard.launch(share=True)
