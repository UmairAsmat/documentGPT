```markdown
<div align="center">
  <h1>📄🤖 DocumentGPT: Chat with Your Files!</h1>
  <p>
    <em>Effortlessly interact with your documents using AI.</em>
  </p>
  <img src="https://user-images.githubusercontent.com/your-image-url/banner.png" alt="DocumentGPT Banner" width="600">
</div>

---

## 🌟 Features

- **Upload and Chat:** Seamlessly upload PDF and DOCX files and interact with them in real-time.
- **AI-Powered Responses:** Uses OpenAI's GPT-3.5 Turbo to provide intelligent and context-aware answers to your queries.
- **Smart Text Processing:** Efficiently processes and chunks document content for faster and more relevant responses.
- **Interactive Streamlit Interface:** Enjoy a clean and intuitive UI built with Streamlit, making it easy to use.

## 🛠️ Installation

### Prerequisites

Ensure you have the following installed on your machine:

- Python 3.7 or later
- OpenAI API Key (sign up at [OpenAI](https://platform.openai.com/signup))
- Hugging Face API Token (sign up at [Hugging Face](https://huggingface.co/join))

### Setup Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/document-gpt.git
   cd document-gpt
   ```

2. **Install the Dependencies**

   Install all required Python packages by running:

   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**

   Create a `.streamlit/secrets.toml` file and add your OpenAI API key:

   ```toml
   [secrets]
   OPENAI_API_KEY = "your-openai-api-key"
   ```

   Optionally, you can use a `.env` file to load environment variables for Hugging Face or any other service.

### Run the App

Start the Streamlit app by executing:

```bash
streamlit run app.py
```

This command will launch the app in your default web browser. You can then upload files and start interacting with them!

## 💡 How It Works

1. **File Upload and Parsing:**
   - Upload your documents (PDF, DOCX) via the sidebar. The app extracts text using `PyPDF2` for PDFs and `python-docx` for DOCX files.

2. **Text Chunking:**
   - The extracted text is split into manageable chunks to optimize processing and response accuracy.

3. **Embedding and Vectorization:**
   - Text chunks are embedded using Hugging Face's `all-MiniLM-L6-v2` model. This allows for efficient vector storage and retrieval with `FAISS`.

4. **Conversational AI:**
   - The `ConversationalRetrievalChain` from Langchain is used to create an interactive chatbot experience, retrieving information from vectorized text and generating responses with GPT-3.5 Turbo.

## 📋 Example Usage

After starting the app, simply upload your document and type a question in the input field:

- **Upload a PDF or DOCX file** by clicking on the "Upload your file" button.
- **Click "Process"** to load and process your document.
- **Ask a question** about the uploaded document and receive AI-generated responses instantly.

## 🤝 Contributing

We welcome contributions! Feel free to open issues or submit pull requests for new features or bug fixes. Please make sure to follow the [contribution guidelines](CONTRIBUTING.md).

## 📫 Contact

For any inquiries, please reach out to me.



<div align="center">
  <em>Happy Chatting! 🎉</em>
</div>
```
