Here’s a well-structured **README.md** file for your chatbot project:  

---

# **💬 AI Chatbot with Semantic Search**  

This is a simple AI chatbot that uses **Sentence-BERT (SBERT)** to perform **semantic search** and answer user queries based on a predefined FAQ dataset. The chatbot runs in a command-line interface (CLI) and finds the most relevant response based on the user's input.  

---

## **🚀 Features**  
- Uses **SBERT (all-MiniLM-L6-v2)** for sentence embedding.  
- Computes **semantic similarity** to find the best-matching response.  
- Supports **natural language queries** instead of keyword-based search.  
- Lightweight and runs **entirely on the CPU**.  

---

## **📦 Installation**  

### **1. Clone the Repository**  
```sh
git clone https://github.com/benasphy/semantic_search.git
cd semantic_search
```

### **2. Create a Virtual Environment (Optional but Recommended)**  
```sh
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows
```

### **3. Install Dependencies**  
```sh
pip install sentence-transformers torch
```

---

## **💡 Usage**  
Run the chatbot by executing:  
```sh
python semantic_search.py
```

### **Example Conversation:**  
```
💬 AI Chatbot with Semantic Search (Type 'exit' to quit)
You: Who is the CEO of OpenAI?
🤖 Bot: Sam Altman is the CEO of OpenAI.

You: What has he invested in?
🤖 Bot: Sam Altman has invested in Reddit, Stripe, and Asana.

You: exit
👋 Goodbye!
```

---

## **🛠 How It Works**  
1. **SBERT Model**: Loads `all-MiniLM-L6-v2` from `sentence-transformers`.  
2. **Precomputed Embeddings**: Generates embeddings for predefined FAQ questions.  
3. **Semantic Search**:  
   - Converts user input into an embedding.  
   - Computes **cosine similarity** with stored embeddings.  
   - Returns the **most relevant** response.  
4. **Command-line Chatbot**: Keeps running until the user types `"exit"`.  

---

## **📜 License**  
This project is open-source under the **MIT License**.  

---
