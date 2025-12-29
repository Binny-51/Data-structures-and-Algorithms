## 📄 Document Processing Tool

**Description:**  
Developed a document processing system for **word frequency analysis** and **efficient pattern searching** over large text corpora. The tool emphasizes correctness, scalability, and fast query performance.

---

### 📘 Dictionary Module (Word Count Engine)
**Overview:**  
Implemented a dictionary data structure to store and retrieve **case-insensitive word counts** from documents.

**Key Features:**
- Tokenization of sentences into individual words
- Case-insensitive normalization
- Efficient insertion and lookup of word frequencies
- Ability to dump the dictionary to a file in a standardized format

**Core Concepts Used:**
- AVL Trees / Hash Tables
- String processing
- Memory-efficient data storage

---

### 🔍 Pattern Search Engine
**Overview:**  
Implemented an efficient pattern-matching engine using the **Rabin–Karp algorithm** to locate all occurrences of a pattern within a document.

**Key Features:**
- Case-insensitive pattern matching
- Supports matches starting and ending inside words
- Returns detailed match metadata:
  - Book code
  - Page number
  - Paragraph number
  - Sentence number
  - Starting offset within the sentence
- Handles multiple matches per query efficiently

**Algorithms & Data Structures:**
- Rabin–Karp String Matching Algorithm
- Rolling Hashing
- Linked Lists for storing search results

---

### 🛠 Technologies & Concepts
- C++
- AVL Trees / Hash Tables
- Rabin–Karp Algorithm
- Rolling Hashing
- Linked Lists
- Efficient Memory Management

---

⭐ Built with a focus on **high performance, correctness, and scalability** for large-scale text processing.

