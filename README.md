# NLP-Research-and-Experiments

objective 1: given a random poem, tell us the prob that this would be selected as pushcart nominee or winner.

objective 2: Learn to retrieve articles relevant to given input (poem). Take lines from the poem, google for articles that are in some way related to the topics mentioned, pick those as your articles that you convert into --> Parts Of Speech --> Knowledge Graph --> Embeddings --> Vector Store

### Data Collection and Preprocessing

1. Scraping Poems:
    - Scraped and stored poems from specified URLs.
    - Saved the poems as pickle and CSV files.

2. Tokenization and POS Tagging:
    - Tokenized and POS-tagged poems using NLTK.
    - Calculated and normalized POS distributions.

### POS Distribution Analysis

3. POS Distribution Computation:
    - Computed frequency distributions and average POS distributions for the poems.
    - Pushcart Probability Assessment 
4. Visualization:
    - Plotted bar charts of POS distributions.

### Similarity Analysis

5. Cosine Similarity Calculation:
    - Converted POS distributions to vectors.
    - Calculated and bucketized cosine similarity scores.

### Golden Cluster Identification

6. Clustering:
    - Applied K-means clustering on POS vectors.
    - Identified the golden cluster with the highest objective ratio.


### Knowledge Graph Creation

7. Knowledge Graphs with NetworkX:
    - Created and visualized knowledge graphs based on syntactic dependencies.


### Article Retrieval and Semantic Search

8. Embedding Generation and Storage:
    - Generated embeddings using Sentence-BERT.
    - Stored embeddings in ChromaDB.

9. Similarity Search and Retrieval:
    - Queried ChromaDB with poem embeddings.
    - Retrieved and ranked the most similar articles.

### Experiments on Topic Extraction and LLM Performance

10. Experiments with Gemini Model:
    - Extracted topics from articles and poems using the Gemini model.
    - Compared topic extraction results using different temperature settings (0.1 and 0.9).

