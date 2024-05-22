# Research Bot

The News Research Tool is a Streamlit application designed to analyze news articles and answer questions based on user input. It leverages advanced natural language processing (NLP) techniques, including embeddings and retrieval models, to provide accurate and insightful answers to user queries.

## Key Features

- **URL Input**: Users can input URLs of news articles they want to analyze directly into the application.
  
- **Text Processing**: The tool processes the text from the provided URLs, extracting key information and generating embeddings using OpenAI's state-of-the-art models.

- **Embeddings Storage**: The generated embeddings are stored efficiently using FAISS, a library for efficient similarity search and clustering of dense vectors.

- **Question Answering**: Users can ask questions related to the analyzed articles using natural language queries. The tool retrieves relevant answers based on the processed text and stored embeddings.

- **Source Display**: Along with the answers, the tool displays the sources from which the information was retrieved, providing transparency and credibility to the results.

  ![image](https://github.com/AnishaChitturu/FirstBot/assets/74812549/0f0d431b-345f-4c74-9b3d-4d77d0c70bc5)


## Why FAISS, Splitters, and OpenAI Embeddings?

- **FAISS**: FAISS is chosen for its efficiency in storing and retrieving embeddings. It allows for fast similarity searches over large datasets, enabling quick and accurate retrieval of relevant information.

- **Splitters**: The use of splitters, such as RecursiveCharacterTextSplitter, helps break down the text into smaller chunks, facilitating better analysis and embedding generation, especially for longer articles.

- **OpenAI Embeddings**: OpenAI's embeddings provide powerful representations of text, capturing semantic information and contextual relationships. By utilizing these embeddings, the tool can understand and process the nuances of language, leading to more accurate question answering.

## Why not Chatgpt

- Chatgpt can also do it, if we copy and paste the article in the prompt. But there are three major issues we might encounter:
#1 - It is a tedious job to copy and paste articles.
#2 - We need one or more articles, we need to aggregate them.
#3 - Due to the word limit per prompt, we cannot pull from large articles.


## Future Scope

- **UI Enhancement with React**: Consider migrating the user interface to a more dynamic framework like React.js. This would allow for greater flexibility in design and interaction, providing a smoother and more intuitive user experience.

- **Cron Job for Data Ingestion**: Implement a scheduled task using a cron job or similar tool to automatically ingest new data from specified sources at regular intervals. This would ensure that the tool remains up-to-date with the latest news articles without manual intervention.


## Dependencies

- Python 3.7+
- Streamlit
- Dotenv
- LangChain
- FAISS
- OpenAI



