

# Aarogyam - AI-Powered Healthcare Chatbots  

Aarogyam is an AI-driven **healthcare platform** that integrates **10 specialized chatbots** to provide **personalized health insights**, including **AI Diet Plan, Symptom Checker, Mental Health Support, and more**. It leverages **NLP, LLMs, and Neo4j** for intelligent health recommendations.

---

## 🚀 Features  
- 🔹 **10 Specialized Healthcare Chatbots**  
- 🔹 **AI Diet Plan for personalized nutrition**  
- 🔹 **Symptom Checker for preliminary health assessment**  
- 🔹 **Mental Health Support and Wellness Guide**  
- 🔹 **Interactive NLP-based responses using OpenAI API**  
- 🔹 **Neo4j Database for structured medical knowledge storage**  

---

## 🛠 Tech Stack  
- **Backend:** Python, Flask, OpenAI API, Neo4j  
- **Frontend:** React  
- **Database:** Neo4j  
- **ML/NLP:** Hugging Face Transformers, OpenAI API  

---

## 🔧 Installation  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/YourUsername/Aarogyam.git
cd Aarogyam
```

### 2️⃣ Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Set Up Neo4j Database  
#### **Install & Start Neo4j**  
- **Download Neo4j:** [Click Here](https://neo4j.com/download/)  
- **Start Neo4j Desktop or Community Edition**  

#### **Initialize the Database**  
```python
from neo4j import GraphDatabase

uri = "bolt://localhost:7687"
username = "neo4j"
password = "your_password"

driver = GraphDatabase.driver(uri, auth=(username, password))

def initialize_db(tx):
    tx.run("CREATE CONSTRAINT ON (n:Health) ASSERT n.id IS UNIQUE")

with driver.session() as session:
    session.write_transaction(initialize_db)

driver.close()
```

### 4️⃣ Run the Application  
```bash
python app.py
```

### 5️⃣ Open in Browser  
Go to: **[http://127.0.0.1:5000](http://127.0.0.1:5000)**  

---

## 📂 Project Structure  
```
├── backend/
│   ├── app.py           # Flask backend  
│   ├── chatbot.py       # Chatbot logic  
│   ├── neo4j_handler.py # Neo4j database handler  
│   ├── requirements.txt # Python dependencies  
│  
├── frontend/
│   ├── public/  
│   ├── src/  
│   ├── App.js           # React main app  
│   ├── components/      # Chatbot UI components  
│  
└── README.md
```

---

## 🔮 Future Enhancements  
- ✅ Integration of **real-time health monitoring**  
- ✅ **Voice-based AI chatbots** for accessibility  
- ✅ Expansion to include **doctor consultations**  

---

## 📬 Contact  
📧 **Email:** katha.kirtan2@gmail.com
🔗 **LinkedIn:** https://www.linkedin.com/in/kirtanubhavsar/

---

🚀 **Aarogyam - AI for Smarter Healthcare!**  
```


Just **replace "YourUsername"** with your actual GitHub username, and it's good to go! 🚀
