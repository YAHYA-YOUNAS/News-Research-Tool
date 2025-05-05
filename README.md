# News Research Tool 

News Research Tool is a user-friendly tool designed for effortless information retrieval. Users can input article URLs and ask questions to receive relevant insights from the stock market and financial domain.

![](bot.jpg)

## Features

- Load URLs or upload text files containing URLs to fetch article content.
- Process article content through LangChain's UnstructuredURL Loader
- Construct an embedding vector using OpenAI's embeddings and leverage FAISS, a powerful similarity search library, to enable swift and effective retrieval of relevant information
- Interact with the LLM's (Chatgpt) by inputting queries and receiving answers along with source URLs.


## Installation

1.Clone this repository to your local machine using:

```bash
  git clone https://github.com/YAHYA-YOUNAS/News-Research-Tool
```
2.Navigate to the project directory:

```bash
  cd News-Research-Tool
```
3. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Set up your GROQ API key by creating a .env file in the project root and adding your API

```bash
  GROQ_API_KEY="your_api_key_here"
```
## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.

- Initiate the data loading and processing by clicking "Process URLs."

- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles
- In video tutorial, we used following news articles
  - https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
  - https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html
  - https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- faiss_store.pkl: A pickle file to store the FAISS index.
- .env: Configuration file for storing your GROQ API key.


# 📰 News Research Tool

News Research Tool is a user-friendly tool designed for effortless information retrieval. Users can input article URLs and ask questions to receive relevant insights from the stock market and financial domain. News Research Tool helps users extract and query information from news articles using advanced natural language processing techniques. It's particularly useful for researchers, investors, and analysts who need to quickly gather insights from multiple financial news sources.

![](bot.jpg)

## ✨ Features

- Load URLs or upload text files containing URLs to fetch article content
- Process article content through LangChain's UnstructuredURL Loader
- Construct an embedding vector using OpenAI's embeddings and leverage FAISS, a powerful similarity search library, to enable swift and effective retrieval of relevant information
- Interact with the LLM's (ChatGPT) by inputting queries and receiving answers along with source URLs

## 🛠️ Tech Stack

- **Python**: Core programming language
- **Streamlit**: Web application framework for creating interactive UI
- **LangChain**: Framework for working with language models and document processing
- **FAISS**: Similarity search library for efficient information retrieval
- **GROQ**: API for language model interactions
- **HuggingFace Embeddings**: For creating vector representations of text

## 🚀 How to Run

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. Clone this repository to your local machine using:
   ```bash
   git clone https://github.com/YAHYA-YOUNAS/News-Research-Tool
   ```

2. Navigate to the project directory:
   ```bash
   cd News-Research-Tool
   ```

3. Install the required dependencies using pip:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up your GROQ API key by creating a .env file in the project root and adding your API:
   ```bash
   GROQ_API_KEY="your_api_key_here"
   ```

### Running the Application

1. Run the Streamlit app by executing:
   ```bash
   streamlit run main.py
   ```

2. The web app will open in your browser.
   - On the sidebar, you can input URLs directly
   - Initiate the data loading and processing by clicking "Process URLs"
   - Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS
   - The embeddings will be stored and indexed using FAISS, enhancing retrieval speed
   - The FAISS index will be saved in a local file path in pickle format for future use
   - You can now ask a question and get the answer based on those news articles

## 💡 Usage Examples

In the video tutorial, we used the following news articles:
- https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
- https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html
- https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

## 📁 Project Structure

- **main.py**: The main Streamlit application script
- **requirements.txt**: A list of required Python packages for the project
- **faiss_store.pkl**: A pickle file to store the FAISS index
- **.env**: Configuration file for storing your GROQ API key

## 👥 Contributing

Contributions are welcome! Here's how you can contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

### Guidelines for Contributions

- Follow the existing code style
- Add comments to your code where necessary
- Write descriptive commit messages
- Update documentation if you change functionality

## 🙏 Acknowledgements
- Based on concepts from [LangChain Crash Course](https://github.com/codebasics/langchain/tree/main/2_news_research_tool_project)
- Thanks to the creators of LangChain, FAISS, and Streamlit for their amazing tools
- All contributors who have helped to improve this project

## 📄 License

This project is licensed under the MIT License.