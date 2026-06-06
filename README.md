---
title: Book Recommender
emoji: 📚
colorFrom: blue
colorTo: purple
sdk: gradio
sdk_version: 5.49.1
app_file: app.py
pinned: false
---

## 📚 Book Recommender System

An intelligent **book recommendation system** built with **Python** and **Large Language Models (LLMs)**.
This project uses **semantic embeddings** to understand book descriptions and recommend similar titles based on meaning, not just keywords.
The interactive **Gradio dashboard** allows users to input a book title or description and instantly receive personalized book recommendations.

---

## 🚀 Features

* 🧠 **LLM-Powered Understanding:** Generates high-quality semantic embeddings for book descriptions.
* 🔍 **Content-Based Recommendations:** Finds books with similar narratives, genres, and styles.
* 🧩 **Gradio Interface:** Simple, elegant dashboard for interactive exploration.
* 📊 **Scalable and Modular:** Can integrate new datasets or AI models with minimal changes.
* 💡 **Data-Driven Discovery:** Helps readers uncover hidden gems beyond popular titles.

---

## 🧰 Tech Stack

* **Python 3.10+**
* **pandas**, **numpy** – for data processing
* **OpenAI API** – for text embeddings
* **LangChain + ChromaDB** – for vector similarity search
* **Transformers (HuggingFace)** – for emotion and category classification
* **Gradio** – to build the user interface

---

## 📁 Dataset

This project uses the **[7k Books with Metadata](https://www.kaggle.com/datasets)** dataset, which includes:

* Titles
* Authors
* Descriptions
* Genres
* ISBN and publication details

---

## ⚙️ Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/Abdifatah2023/BookRecommender.git
cd BookRecommender

# 2. Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Create a .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_api_key_here" > .env

# 5. Run the Gradio app
python app.py
```

---

## 🧠 How It Works

1. **Preprocessing** – Cleans and normalizes book descriptions.
2. **Embedding Generation** – Converts text to dense vectors using OpenAI embeddings.
3. **Vector Search** – Uses ChromaDB to find semantically similar books.
4. **Emotion Filtering** – Ranks results by emotional tone (joy, fear, sadness, etc.).
5. **Recommendation Output** – Displays top results in the Gradio dashboard.

---

## 🖥️ Gradio Dashboard

Once launched, you'll see an interface where you can:

* Enter a **book description**
* Choose a **category** (Fiction, Nonfiction, Children's Fiction)
* Choose an **emotional tone** (Happy, Surprising, Angry, Suspenseful, Sad)

---

## 🔒 Security Notes

Make sure `.env` is **ignored** in your repository:

```gitignore
# .gitignore
.env
```

Set your `OPENAI_API_KEY` as a Space secret in the Hugging Face dashboard — never commit it.
