# Leveraging Gen AI for SAT Prep

I’ll start with sharing my motivation for creating this notebook. When I was preparing for SAT mid-2023, I struggled to find extra study material for the new Digital SAT (launched in Spring of 2023), especially for the reading and writing section, which is tougher to crack compared to the math section. I had an idea: why not ask ChatGPT? But to my surprise, the SAT-style questions it generated were lackluster and I knew that I could be the only one, leading me to dive deeper into researching how I can leverage Gen AI for SAT prep.

I ended up figuring out an approach to leverage Llama 3 Instruct models for building my proficiency in word in context type of questions. Through that I was able to build my vocabulary, which is the critical aspect in scoring well in the reading and writing section. I scored 760 out of 800 in my first SAT attempt, which is 99th percentile among all test takers.

I had to use an A100, single GPU, machine from Lambda Labs.

## How to Use the Repository

In your dev environment (Colab, etc.) clone this repository using the following command: git clone https://github.com/PragyanR/GenAI_for_SAT_Prep.git

Open notebook "Llama3_for_SAT_Prep_Prompt_Engineering.ipynb" and run the cells

## Artifacts

This repository has notebooks and artifacts I leveraged to master vacabulary for SAT. I have this code in the following website (URL) for students to master vacabulary. Here are come of the key notesbooks:

#### 1/ Semantic Similarity.ipynb
This notebook showcases how I used semantic similarity to find the best suited word for a given genre to reduce hallucination. Semantic similarity is based on this paper: https://arxiv.org/pdf/2108.06130

#### 2/ Llama3_for_SAT_Prep_Prompt_Engineering.ipynb
This notebook showcases various prompt engineering techniques I used.

#### 3/ Llama3_for_SAT_Prep_Fine_Tuning.ipynb
This notebook showcases how I went about fine-tuning Llama 3 Instruct model.

#### 4/ SAT Word Dataset (sat_vocab.csv)
This dataset has SAT words.

#### 5/ SAT Genre Dataset (sat_genre.csv)
This dataset has 300 odd Genre.

#### 6/ Test cases (semantic_eval_1000_word_genre.csv)
This dataset has word and gener combinations based on semantic similarity.
