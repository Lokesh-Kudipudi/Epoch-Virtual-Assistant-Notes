# Retrieval Augmented Generation

[Home](/main.md)

## Source 1 - [Link](https://www.youtube.com/watch?v=T-D1OfcDW1M)

Generation refers to LLMs that generate text
The data on which LLMs are trained can be outdated real Quick, Imagine we retrieve data from a particular source

User :- Which Planets have the most number of Moon? \
LLM :- Its Jupiter (based on trained Data)

### RAG - Model

User :- Which Planets have the most number of Moon? \
Retrieves the relavant content \
Retrieves Data that is relevant to the User Query \
LLMs :- Answers based on the Data Retrieved which is more accurate \
If the Retriever cannot give the relevant data then LLM should say that I cannot answer the Query \
So We do depend on a General LLM like chatGPT over here we just provide some relevant information for the LLM to answer from

## Source 2 - [Link](https://www.youtube.com/playlist?list=PLfaIDFEXuae2LXbO1_PKyVJiQ23ZztA0x)

LLMs haven’t learnt from much data that is private to most of us \
Connecting LLMs to External data is a central need \
Question → Retrieve Relavent Data from the DB → Prompt the LLMs
Documents are indexed and stored in our DB
