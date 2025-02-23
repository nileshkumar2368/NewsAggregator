# 📰 AI-Powered News Aggregator

An **AI-powered web application** that classifies news headlines into **Legitimate, Clickbait, or Conspiracy** using **Machine Learning & NLP**. This project includes:
- A **FastAPI backend** for classification and CRUD operations.
- A **Gradio UI** for real-time headline analysis.
- A **RandomForest-based NLP model** trained on TF-IDF features.

## 📌 Features
✅ **Headline Classification** – Detects if a headline is Legitimate, Clickbait, or Conspiracy.
✅ **Confidence Score & Probability Breakdown** – Provides category probabilities.
✅ **Suspicious Word Detection** – Highlights words often used in misleading news.
✅ **FastAPI Backend** – RESTful API for model inference.
✅ **CRUD Operations** – Users can manage headlines dynamically.
✅ **Gradio UI** – Simple web interface for testing the classifier.

---

## 📂 Project Structure
```
├── backend/
│   ├── main.py           # FastAPI Backend
│   ├── model.py          # ML Model Training & Loading
│   ├── news_data.json    # Sample News Dataset
│   ├── classifier.joblib # Trained Model
│   ├── vectorizer.joblib # TF-IDF Vectorizer
│   └── requirements.txt  # Dependencies
├── frontend/
│   ├── app.py            # Gradio UI
│   ├── README.md         # Documentation
└── README.md             # Main Project ReadMe
```

---

## 🛠️ Installation
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/news-aggregator.git
cd news-aggregator
```
### 2️⃣ Install Dependencies
```bash
pip install -r backend/requirements.txt
```

---

## 🚀 Running the Project
### Start FastAPI Backend
```bash
cd backend
uvicorn main:app --reload
```
The API will run at: **`http://localhost:8000`**

### Start Gradio Frontend
```bash
cd frontend
python app.py
```

---

## 🔬 API Endpoints
| Method | Endpoint         | Description |
|--------|----------------|-------------|
| `POST` | `/analyze`      | Classifies a news headline |
| `GET`  | `/articles`     | Fetches all stored headlines |
| `POST` | `/add`          | Adds a new headline |
| `PUT`  | `/update/{id}`  | Updates an existing headline |
| `DELETE` | `/delete/{id}` | Removes a headline |

---

## 🎯 Usage
1️⃣ Open the **Gradio UI** in your browser.
2️⃣ Enter a news headline.
3️⃣ Click "Analyze" to see:
   - **Predicted Category** (Legitimate, Clickbait, Conspiracy)
   - **Confidence Score & Probabilities**
   - **Suspicious Words Found**

---

## 🌍 Deployment
To deploy the app on **Hugging Face Spaces, Heroku, or Vercel**, follow their guidelines:
```bash
# Example: Deploy using Docker
docker build -t news-aggregator .
docker run -p 8000:8000 news-aggregator
```


## 📞 Contact
For queries, reach out via nileshkumar2358@gmail.com or open an issue on GitHub. 🚀

