🧠Word2Vec on Game and series Lore

Training Separate Embedding Models for Dark Souls and Game of Thrones



&nbsp;📌Overview

This repository contains two independent Word2Vec experiments trained on:

Dark Souls lore dataset

Game of Thrones text dataset

The goal is to analyze how corpus size affects embedding quality and semantic similarity results.





📂 Repository Structure

├── dark\_souls\_word2vec.ipynb

├── game\_of\_thrones\_word2vec.ipynb  

├── dark\_souls\_dataset.txt  AS dataset

├── game\_of\_thrones\_dataset.txt  AS archive 

└── README.md





🧪 Experiments

1️⃣ Dark Souls Word2Vec



Dataset size: ~461 lines

Trained using Gensim Word2Vec

Observed issue: similarity results biased toward frequent stopwords



2️⃣ Game of Thrones Word2Vec



Dataset size: ~145,020 lines

Same training configuration

Produces meaningful noun-based similarity outputs





🔍 Key Observation



Word2Vec performance is highly dependent on corpus size.

Dataset	Size	Embedding Quality

Dark Souls	Small (~461 lines)	Weak semantic learning

Game of Thrones	Large (~145k lines)	Strong contextual embeddings



Smaller corpora tend to:



Overfit to high-frequency words

Return stopwords in similarity queries

Lack semantic depth



⚙️ Tech Stack



Python

Jupyter Notebook

Gensim (Word2Vec)

NumPy,Pandas

