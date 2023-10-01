# Implements Retrieval Augmented Generation
# Talk through Multiple PDF Documents
Description: A Streamlit web application to facilitate conversational interactions based on the content of uploaded PDF documents.

Key Features:

PDF Upload: Users can upload multiple PDF files simultaneously through the sidebar.
Text Extraction: The content of these PDFs is extracted and processed to be conversation-ready.
Conversational Interface: Users can ask questions related to the content of the uploaded documents. The application responds conversationally, providing relevant information from the documents.
Text Chunking: Extracted text is split into manageable chunks using a character-based text splitter.
Text Embeddings: The application uses embeddings (from OpenAI or HuggingFaceInstruct) to represent text chunks and store them in a FAISS vector store.
Conversational Retrieval Chain: Combines the power of a large language model (LLM) with the retrieval capabilities of the FAISS vector store to provide conversationally relevant responses.
How to use:

Launch the Streamlit application.
Use the sidebar to upload one or multiple PDF documents.
Click on "Process" to extract and process the text content of the PDFs.
Use the main chat interface to ask questions related to the content of your uploaded documents.

Technical Dependencies:

Streamlit
dotenv
PyPDF2
Custom libraries: langchain, template
