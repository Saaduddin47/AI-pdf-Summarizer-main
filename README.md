# 📄 PDF Summarizer App

A simple and powerful web app that allows users to upload PDF documents and receive concise summaries in seconds using **LangChain**, **OpenAI**, and **Streamlit**.

---

## 🚀 Features

- 📁 Upload any PDF file
- 🧠 Automatically extract and process text
- 🤖 Summarize content using OpenAI's GPT-3.5-turbo model
- 🖥️ Clean, interactive UI built with Streamlit
- ⚡ Fast and accurate results powered by vector search (FAISS + HuggingFace)

---

## 🛠️ Tech Stack

- **Frontend**: [Streamlit](https://streamlit.io/)
- **Backend**: Python, [LangChain](https://www.langchain.com/)
- **LLM**: OpenAI `gpt-3.5-turbo-16k`
- **Text Embeddings**: HuggingFace Transformers
- **Vector Store**: FAISS
- **PDF Reading**: PyPDF

---
Install Required Packages

pip install -r requirements.txt
Set your OpenAI API key

You can either:

Set it in your environment:

export OPEN_AI_KEY=your_openai_api_key  # Linux/macOS
set OPEN_AI_KEY=your_openai_api_key     # Windows
Or hardcode it (not recommended for production):

os.environ["OPEN_AI_KEY"] = "your_openai_api_key"
-------------------------
🚀 How to Run
streamlit run app.py
This will start the web app locally. Open your browser and go to http://localhost:8501.
-------------------------
📂 Project Structure

pdf-summarizer/
├── app.py               # Main Streamlit UI file
├── utils.py             # Core logic: PDF reading, processing, summarizing
├── requirements.txt     # All dependencies
├── README.md            # You are here
-----------------------
🔒 Environment Variables
Make sure to configure the following:

OPEN_AI_KEY: Your OpenAI API key for accessing GPT-3.5 or GPT-4 models.

You can use a .env file with python-dotenv if preferred.
------------------------
🧪 Example Use Case
Upload your research paper, legal contract, or lengthy report.

Let the app break it into chunks, extract key content, and return a clear, short summary.

🐛 Known Issues
PDF files with scanned images or poor formatting may result in incomplete text extraction.

Summarization may miss context if the PDF is too short or lacks cohesive content.

🤝 Contributing
Contributions are welcome! Please open issues or submit pull requests for improvements or feature ideas.

📜 License
This project is licensed under the MIT License.

📬 Contact
Made by Syed Saaduddin Azhaan
📧 Email: saaduddinsyed10@gmail.com

