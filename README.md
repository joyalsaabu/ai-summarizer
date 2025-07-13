AI-Powered Text Summarizer using Gemini LLM & LangChain

This project is a lightweight, yet powerful AI-based Text Summarizer designed to extract and condense information from `.pdf` and `.txt` documents using Gemini 2.5 Flash (Google LLM) through LangChain.

Objective

To create an AI utility tool that allows users to upload lengthy documents and receive a short, meaningful summary—saving time and improving understanding for students, researchers, and professionals.

Problem Statement

Reading long documents takes time, especially when we only need key insights. This tool uses generative AI to:
- Extract text from uploaded `.pdf` or `.txt` files
- Process the content via Gemini LLM
- Return a concise, high-quality summary

Features

- Accepts PDF and text files
- Extracts clean text using PyMuPDF and file reading
- Sends content to Gemini 2.5 Flash LLM via LangChain
- Displays a concise summary of the full document
- Can be extended into a web app

 Approach / How It Works

 Step 1: Upload File
User uploads a `.pdf` or `.txt` file via Google Colab interface.

 Step 2: Extract Text
- If PDF → uses PyMuPDF to extract text page by page
- If TXT → reads file directly

 Step 3: Prompt the LLM
- A prompt is created using LangChain's `PromptTemplate`
- Gemini model (`gemini-2.5-flash`) is initialized with `ChatGoogleGenerativeAI`

 Step 4: LLM Summarization
- The full extracted text is sent as a prompt to Gemini
- Gemini generates a well-structured, coherent summary

 Step 5: Output
- The response is printed as final output in the notebook

 File Structure

 text-summarizer/
│
├── text summarizer.ipynb 
├── README.md 

Note
do  not publicily display your api key so not displaying api key in the code



