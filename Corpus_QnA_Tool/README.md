## ❓ Corpus QnA Tool

**Description:**  
Developed a Question Answering system over a large text corpus that identifies the **most relevant paragraphs** for a given query and generates answers using **Large Language Models (LLMs)**. The system combines **information retrieval techniques** with **LLM-based reasoning** to produce context-aware and grounded responses.

---

### 🔎 Paragraph Ranking (Top-K Retrieval)
**Overview:**  
Implemented a ranking algorithm to identify the **top-k most relevant paragraphs** for a given query before passing them to an LLM.

**Approach:**
- Tokenized the query into individual words
- Searched occurrences of each query word in the corpus using a previously built search engine
- Assigned **importance scores to words** based on corpus-specific frequency vs general-language frequency
- Computed paragraph scores as a **weighted sum** of query word occurrences
- Sorted paragraphs by score and selected the **top-k most relevant ones**

**Scoring Formula:**
- Word Importance:  
  `s(w) = (frequency in corpus + 1) / (frequency in general corpus + 1)`
- Paragraph Score:  
  Sum of `frequency(word in paragraph) × s(word)` over all query words

---

### 🤖 LLM-Based Answer Generation
**Overview:**  
Fed the ranked top-k paragraphs as context to an LLM to generate accurate, context-grounded answers.

**Key Features:**
- Context-limited prompt construction to fit LLM constraints
- Prompt engineering for better relevance and clarity
- Ensured answers were derived **only from the provided corpus**
- Printed queries and intermediate context for transparency and debugging

**Models Used:**
- ChatGPT (via API)
- Open-source LLMs via Hugging Face APIs (experimental)

---

### 🧠 Optimizations & Enhancements
- Ignored common stop-words to improve ranking quality
- Efficient paragraph scoring using hash maps
- Modular design allowing easy swapping of ranking strategies or LLMs
- Support for free/open-source LLM alternatives

---

### 🛠 Technologies & Concepts
- C++
- Information Retrieval (TF-like weighted scoring)
- Linked Lists
- Hashing & Frequency Analysis
- Prompt Engineering
- LLM APIs (ChatGPT, Hugging Face)

---

⭐ Designed to bridge **classical information retrieval** with **modern LLM-based question answering** for large corpora.

