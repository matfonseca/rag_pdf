# RAG for PDFs

This project is a basic implementation of a Retrieval-Augmented Generation (RAG) system for PDF documents using LangChain, Chroma, and Ollama. The system loads a PDF, splits the text into manageable chunks, creates embeddings, and then allows for retrieval-based question answering using a language model.

## Project Structure

- **PDF Loading**: Uses `PyPDFLoader` to load the content of a PDF file.
- **Text Splitting**: Utilizes `RecursiveCharacterTextSplitter` to split the document into chunks for processing.
- **Embeddings**: Embeddings are generated using the `SentenceTransformerEmbeddings`.
- **Vector Store**: Chroma is used as the vector store to persist and search embeddings.
- **RAG Implementation**: Combines the embedding-based retrieval with a language model (`OllamaLLM`) to answer questions based on the content of the PDF.

## Getting Started

### Prerequisites

- Python 3.9 or higher
- Poetry for dependency management
- [Ollama](https://ollama.com/) installed on your system

### Installation

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd rag-pdf
