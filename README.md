Chatbot
This project is a Streamlit web based application for querying information from PDF files using natural language questions. Let me break down the main components and flow:

Importing Libraries: The necessary libraries are imported, including Streamlit for creating the web interface, PyPDF2 for working with PDF files, various components from the langchain library for natural language processing tasks, and dotenv for loading environment variables.

Loading Environment Variables: The Google API key is loaded from the environment variables.

Function Definitions:

get_pdf_text(pdf_docs): This function extracts text from PDF documents.
get_text_chunks(text): Splits the text into smaller chunks.
get_vector_store(text_chunks): Generates embeddings for the text chunks and creates a vector store using FAISS.
get_conversational_chain(): Sets up a conversational question-answering model.
user_input(user_question): Takes a user's question, searches for relevant documents, and generates a response using the conversational chain.
Main Function:

Sets up the Streamlit page configuration and header.
Provides a text input box for users to ask questions.
When a question is submitted, it processes the uploaded PDF files, extracts text, generates text chunks, creates a vector store, and then processes the user's question to provide a response.
Streamlit Interface:

Users can upload PDF files and ask questions about the content.
Once files are uploaded and the "Submit & Process" button is clicked, the system processes the PDF files and makes them available for querying.
Users can then input questions, and the system responds with relevant information from the PDF documents.
Overall, this project combines PDF processing, natural language understanding, and conversational AI to create a user-friendly interface for querying information from PDF files.

git clone https://github.com/shabanaalina14/chat_with_multiple/tree/main

Contact For any questions or suggestions, please feel free to reach.

Gmail: shabanaalina14@gmail.com

GitHub Profile: https://github.com/shabanaalina14

Happy Coding!
