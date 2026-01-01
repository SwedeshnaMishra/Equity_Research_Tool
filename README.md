# Equity_Research_Tool — Talk to Financial News

## 💬 An End-to-End LLM Project using OpenAI, LangChain & FAISS

**Equity Research Tool** is a user-friendly news research application designed for effortless information retrieval from financial and stock market articles.  
Users can load news article URLs, ask questions in natural language, and receive accurate, context-aware answers along with source references.

---

## 🚀 Project Overview

This tool allows users to:
- Input multiple financial news article URLs.
- Process and index article content using embeddings.
- Ask questions related to the stock market, companies, or financial trends.
- Receive precise answers backed by the original article sources.

The system intelligently:
- Fetches article content from provided URLs.
- Converts text into embedding vectors using OpenAI embeddings.
- Stores and indexes embeddings using FAISS for fast similarity search.
- Uses an LLM (ChatGPT) to generate answers based on the most relevant content.

---

## ✨ Project Highlights

- 📰 Domain-focused on **stock market & financial news**
- 🔍 Fast and efficient information retrieval using **FAISS**
- 🤖 LLM-powered Q&A with **source URL references**
- 🧠 Persistent vector store for reuse (pickle-based FAISS index)

---

## 🧠 Tech Stack

- OpenAI Embeddings & ChatGPT
- LangChain Framework
- FAISS (Vector Similarity Search)
- Streamlit (Interactive Web UI)
- Python
- UnstructuredURL Loader

---

## 🛠️ Installation Guide

### 1️⃣ Clone the repository
```git clone https://github.com/SwedeshnaMishra/Equity_Research_Tool.git```

### 2️⃣ Navigate to the project directory
```cd Retail_QandA_Tool```

### 3️⃣ Install dependencies
```pip install -r requirements.txt```

### 4️⃣ Set up OpenAI API Key
- Create a .env file in the project root and add:
``` `GOOGLE_API_KEY` ="your_api_key_here"```

## ▶️ Usage / Examples

### Run the Streamlit app
```streamlit run main.py```
Then open the local URL (usually `http://localhost:8501`) in your browser.

### How to use the app:
- Enter one or more news article URLs in the sidebar.
- Click “Process URLs” to load and process the data.
- The system will:
  - Fetch article content
  - Split text into chunks
  - Generate embedding vectors
  - Index them using FAISS
- The FAISS index is saved locally in pickle format for future use.
- Ask questions related to the loaded articles and get answers with source links.

---

## 🧪 Sample Articles Used

The following financial news articles were used:

- [Tata Motors, Mahindra gain certificates for production-linked payouts](https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html)
- [Tata Motors launches Punch iCNG, price starts at ₹7.1 lakh](https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html)
- [Buy Tata Motors: Target of ₹743 – KR Choksey](https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html)

---

## 🧩 Project Structure

```
Equity_Research_Tool/
│
├── main.py                    # Main Streamlit application
├── requirements.txt           # Python dependencies
├── faiss_store_openai.pkl     # Stored FAISS vector index
├── .env                       # Environment variables (OpenAI API key)
└── README.md                  # Project documentation
```

---

## 💡 Example Output

**User Query:**  
> What is the outlook on Tata Motors based on the provided news articles?

**System Response:**  
> Tata Motors shows a positive outlook driven by strong analyst recommendations, recent product launches, and favorable market sentiment.  
>  
> **Sources:**  
> - https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html  
> - https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

---

## 📚 Future Enhancements

- Support for PDF and DOCX financial reports
- Automatic news fetching using stock tickers (e.g., NSE/BSE symbols)
- Chat history and multi-session support
- Advanced filtering by company, sector, or date
- Cloud-based vector store integration (Pinecone / Weaviate)
- Improved answer explainability with highlighted source snippets

---

## For Contributing
If you want to contribute to this project, please follow these steps:
- `Fork` the repository.
- Create a new branch `(git checkout -b feature/your-feature-name)`.
- Make your changes and commit them `(git commit -m 'Add some feature')`.
- Push to the branch `(git push origin feature/your-feature-name)`.
- Open a pull request.

---

## Project Maintainer
**Github:** [Swedeshna Mishra](https://github.com/SwedeshnaMishra)
