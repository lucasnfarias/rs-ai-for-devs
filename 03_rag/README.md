# Concept
Try to first retrieve small chunks (child chunks - more precision) from Vector DB and then send a larger chunk (parent chunk - more context - stored in Memory) so that the LLM can give a more refined and complete answer.

**Chunk Size:** determines the context length of individual text pieces (vectors) for embedding, impacting granularity (small=specific, large=broad) and LLM context loading.

**Top-K (number of retrieved chunks):** balances context relevance and noise; small K risks missing info, large K adds irrelevant data, but often with larger chunks, a smaller K works better.

Finding the right balance involves trade-offs, often requiring experimentation to optimize for accuracy, relevance, and processing speed.


![Parent Document RAG](.github/parent-document-rag-diagram.png)
