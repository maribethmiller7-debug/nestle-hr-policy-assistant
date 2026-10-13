# Nestlé HR Policy Assistant

## AI-Powered Retrieval-Augmented Generation (RAG) Application

The Nestlé HR Policy Assistant is an interactive AI application designed to answer natural-language questions using information retrieved from a Nestlé Human Resources policy document.

The project demonstrates how Retrieval-Augmented Generation (RAG) can combine semantic document retrieval with a Large Language Model (LLM) to provide relevant, context-aware answers based on organizational source material.

### Technologies Used

- Python
- OpenAI API
- LangChain
- Chroma Vector Database
- OpenAI Embeddings
- Retrieval-Augmented Generation (RAG)
- Gradio
## The Problem

HR policy documents can contain important information that employees need to access quickly, but manually searching through documents can be time-consuming and inefficient. This project explores how generative AI and semantic search can make organizational knowledge easier to access through natural-language questions.

## The Solution

I developed a Retrieval-Augmented Generation (RAG) application that allows a user to ask questions about the HR policy in natural language.

The application processes the policy document into smaller text chunks, converts those chunks into vector embeddings, and stores them in a Chroma vector database. When a user submits a question, the system retrieves the most relevant policy information and provides that context to a Large Language Model to generate a response.

A Gradio interface provides a simple way for users to interact with the application.
## How It Works

1. **Load the HR Policy Document**  
   The source HR policy document is loaded into the application.

2. **Split the Document into Chunks**  
   The document text is divided into smaller sections so that relevant information can be retrieved efficiently.

3. **Create Vector Embeddings**  
   OpenAI Embeddings are used to convert the text chunks into numerical vector representations that capture semantic meaning.

4. **Store Embeddings in Chroma**  
   The embeddings are stored in a Chroma vector database for semantic search and retrieval.

5. **Retrieve Relevant Context**  
   When a user asks a question, the application searches the vector database and retrieves the most relevant sections of the HR policy.

6. **Generate an Answer with the LLM**  
   The retrieved policy information is provided to the Large Language Model as context so it can generate a response grounded in the source document.

7. **Display the Response in Gradio**  
   The user receives the generated answer through an interactive Gradio interface.
   ## Project Results

The completed application successfully:

- Loaded and processed the Nestlé HR policy document.
- Divided the document into searchable text chunks.
- Generated embeddings for semantic document retrieval.
- Stored and retrieved policy information using Chroma.
- Retrieved relevant policy context based on a user's question.
- Used an LLM to generate answers based on the retrieved information.
- Provided an interactive Gradio interface for asking HR policy questions.

The project demonstrates how Retrieval-Augmented Generation can be used to create an AI-powered knowledge assistant for organizational documents.

## What I Learned

Through this project, I gained hands-on experience with:

- Building an end-to-end RAG workflow.
- Working with Large Language Models through the OpenAI API.
- Creating and using vector embeddings.
- Using a vector database for semantic search and retrieval.
- Connecting document retrieval with LLM-generated responses.
- Designing prompts to guide model responses.
- Integrating multiple AI components into a working application.
- Building an interactive user interface with Gradio.
- Managing API credentials securely using environment variables.

This project strengthened my understanding of how generative AI can be applied to real-world knowledge management and information-retrieval problems.
## Application Demo

The screenshot below demonstrates the Nestlé HR Policy Assistant answering a question using information retrieved from the HR policy document.

![Nestlé HR Policy Assistant Demo](Nestle%20HR%20Policy%20Assistant%20chatbot.png)
