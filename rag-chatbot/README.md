# RAG Chatbot

This project is a Retrieval-Augmented Generation chatbot built with Next.js, LangChain, OpenAI, and MongoDB Atlas Vector Search. Users can upload PDF files, index their contents, and ask questions against the uploaded knowledge base.

## What It Does

- Uploads PDF documents for processing
- Splits and embeds document text
- Stores embeddings in MongoDB Atlas
- Retrieves relevant context for user questions
- Generates answers with OpenAI

## Tech Stack

- Next.js 14
- TypeScript
- LangChain
- MongoDB Atlas
- OpenAI
- Tailwind CSS

## Local Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Create a `.env` file in the project root.

3. Add the required variables:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   MONGODB_URI=your_mongodb_connection_string
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open `http://localhost:3000`.

## Deployment Notes

This app is configured for deployment on Render and uses MongoDB Atlas as the backing data store. Before deployment, make sure:

- the MongoDB Atlas cluster is reachable from your hosting platform
- the required environment variables are configured
- a vector index exists for the embedded document data

## Project Structure

```text
rag-chatbot/
|-- src/app/
|-- src/utils/
|-- public/
|-- assets/
|-- package.json
`-- render.yaml
```

## Environment Variables

- `OPENAI_API_KEY`: OpenAI API key for embeddings and chat completion
- `MONGODB_URI`: MongoDB Atlas connection string

## Portfolio Context

This project demonstrates applied LLM engineering with document ingestion, semantic retrieval, API routes, and deployment-oriented full-stack structure.
