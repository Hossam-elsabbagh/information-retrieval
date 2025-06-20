# 🔍 Information Retrieval System using PyTerrier & Flask

A full-featured **Information Retrieval** project built in Python with **PyTerrier**, supporting document indexing, preprocessing, ranking with **BM25**, **TF-IDF**, **query expansion using RM3**, and a web interface with **Flask** & **ngrok**.

## 📁 Dataset

The project uses the **CISI dataset**, which includes:  
- `CISI.ALL` – full documents  
- `CISI.QRY` – queries  
- `CISI.REL` – relevance judgments  
These files are extracted and parsed into structured `DataFrames`.

## 🧠 Features

- ✅ Preprocessing: Cleaning, stopwords removal, stemming  
- 🧾 Document & Query Indexing using PyTerrier  
- 📊 Retrieval using:  
  - **TF-IDF**  
  - **BM25**  
  - **RM3** (Query Expansion)  
- 🤖 Query expansion using top documents and terms  
- 🌐 Web interface built with **Flask** and hosted using **ngrok**  
- 🔁 Interactive search and result display  
- 🤖 BERT tokenization for text understanding

## 🛠️ Requirements

- Python 3.6+  
- Install dependencies:

```bash
pip install python-terrier nltk flask flask_ngrok pyngrok
```

- For PRF (query expansion):

```bash
git clone https://github.com/terrierteam/terrier-prf/
apt-get install maven
cd terrier-prf
mvn install
```

## ▶️ How to Run on Google Colab

1. Upload the notebook `IR_Project.ipynb` to Colab  
2. Upload `cisi.zip` and extract it  
3. Run all cells **in order**  
4. At the Flask section:  
   - Add your ngrok authtoken  
   - Copy the generated public URL

## 🌍 Web Interface

- Built with `Flask` + `HTML` + `JavaScript`  
- Lightweight UI for searching queries  
- Results shown with relevance scores

## 🧪 Sample Query Flow

1. Query input: `"book"`  
2. Preprocessing (clean → remove stopwords → stem)  
3. Match with documents  
4. Rank with **BM25**, optionally expand using **RM3**  
5. Output top documents and scores

## 📂 Project Structure

```
IR_Project/
├── IR_Project.ipynb        # Main Jupyter notebook
├── cisi.zip                # Dataset ZIP file
├── cisi_dataset/           # Extracted files
└── README.md               # This file
```

## 🧑‍💻 Author

**Hossam Elsabbagh**  
🎓 Zewail City of Science & Technology  
💡 Computer Science and AI Student  
📍 Egypt

> Made with 💙 for learning and research.
