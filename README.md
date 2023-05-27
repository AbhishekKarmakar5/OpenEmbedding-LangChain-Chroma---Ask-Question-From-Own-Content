# OpenEmbedding-LangChain-Chroma : Ask-Question-From-Own-Content

# Chroma and LangChain Demo
This repository contains code and resources for demonstrating the power of Chroma and LangChain for asking questions about your own data. 
The demo showcases how to pull data from the English Wikipedia using their API. The project also demonstrates how to vectorize data in chunks and get embeddings using OpenAI embeddings model.

We then use [LangChain](https://github.com/hwchase17/langchain) to ask questions based on our data which is vectorized using OpenAI embeddings model. 
I used [Chroma](https://github.com/chroma-core/chroma) a database for storing and querying vectorized data.

## Getting Started
To get started with the demo, you will need to have Python (I use Python 3.8) installed on your machine. You will also need to install the required Python packages by running the following command:
`pip install -r requirements.txt`

 **You can change the `_ALGORITHMS` constant to whatever you want to query other topics on Wikipedia.**

From there on you can simply run `wikipedia.py` which generates the text file which will be vectorized and stored in the database.
You need to use the name of the created textfile in the `ask_wikipedia.py` file.

Now you can run `ask_wikipedia.py`.

**Simply change the `print(genie.ask("Can you tell me the formula for Linear Regression?"))` in the `ask_wikipedia.py` file to whatever question you want to ask.**

# OpenAI Whisper API ChromaDB and LangChain Demo
This repository contains code and resources for demonstrating the power of OpenAI's Whisper API in combination with ChromaDB and LangChain for asking questions about your audio data. 
The demo showcases how to transcribe audio data into natural language with the Whisper API. The project also demonstrates how to vectorize data in chunks and get embeddings using OpenAI embeddings model.

We then use [LangChain](https://github.com/hwchase17/langchain) to ask questions based on our data which is vectorized using OpenAI embeddings model. 
I used [Chroma](https://github.com/chroma-core/chroma) a database for storing and querying vectorized data.

## Getting Started
To get started with the demo, you will need to have Python (I use Python 3.8) installed on your machine. You will also need to install the required Python packages by running the following command:
`pip install -r requirements.txt`

All the `(m4a, mp3, mp4, mpeg, mpga, wav, webm)` files need to be in the `/files` folder.

 **Run the `whisper.py` file to generate a .txt file out of your audio data**

Now you can run `ask_the_audio.py`.

**Simply change the `print(genie.ask("Can you tell me the formula for Linear Regression?"))` in the `ask_the_audio.py` file to whatever question you want to ask.**
