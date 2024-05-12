## Usage Examples

This section provides examples of how to utilize the custom GPT model for specific NLP tasks:

- **Document Processing**:
  ```python
  from langchain.document_loaders import PyPDFLoader
  loader = PyPDFLoader('path_to_your_document.pdf')
  document_text = loader.load()

from langchain_openai import ChatOpenAI
chat_model = ChatOpenAI(api_key='your_openai_api_key')
response = chat_model.query("What is natural language processing?")
print(response)
