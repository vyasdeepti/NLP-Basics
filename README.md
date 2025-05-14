# NATURAL LANGUAGE PROCESSING 📚📚

Welcome to the **NLP Basics** repository! This repository serves as a comprehensive guide for beginners and enthusiasts to explore the foundational concepts and techniques in **Natural Language Processing (NLP)**. It contains interactive Jupyter Notebooks and Python scripts that demonstrate various NLP workflows, algorithms, and applications.

---

## Repository Overview

### 🗂 Repository Composition:
- **Languages Used:**
  - **Jupyter Notebook/Google Colaboratory** : Interactive notebooks to explore and execute NLP concepts.
  - **Python** : Python scripts for implementing core NLP functionalities.

- **Intended Audience:**
  - Beginners aiming to learn NLP concepts.
  - Students and researchers working on NLP projects.
  - Practitioners looking for foundational NLP examples.

---

## 📚 Contents of the Repository

### 1. **NLP Preprocessing**
   - **Files**: `NLP_Preprocessing_1.ipynb`, `NLP_Preprocessing_2.ipynb`
   - **Description**: These files cover essential text preprocessing steps required for NLP pipelines.
   - **Key Topics**:
     - Stop Word Removal
     - Tokenization
     - Stemming and Lemmatization
     - Parts of Speech (POS) Tagging
   - **Use Case**: Prepare raw text data for downstream NLP tasks.

---

### 2. **Named Entity Recognition (NER)**
   - **File**: `NamedEntityRecognition.ipynb`
   - **Description**: Demonstrates how to extract and visualize named entities (e.g., persons, organizations, locations) using the `spaCy` library.
   - **Key Features**:
     - Extraction of entities with labels such as PERSON, ORG, DATE, etc.
     - Visualization of entities using `displacy`.
   - **Use Case**: Identify key entities from unstructured text data.

---

### 3. **Word Frequency Analysis**
   - **File**: `WordFrequency_.ipynb`
   - **Description**: Analyzes word frequencies in text data using `spaCy`.
   - **Key Features**:
     - Tokenization and filtering of stop words and punctuation.
     - Identification of the top 10 most frequent words.
   - **Use Case**: Understand the most commonly used terms in a text dataset.

---

### 4. **Bigram Generation**
   - **File**: `convert_in_Biagram.ipynb`
   - **Description**: Generates bigrams (pairs of consecutive words) from a list of sentences.
   - **Key Features**:
     - Efficient implementation using Python's list comprehensions.
     - Example with sentences about flowers and their significance.
   - **Use Case**: Analyze word pair relationships for text modeling tasks.

---

### 5. **CYK Algorithm**
   - **File**: `CYK.ipynb`
   - **Description**: Implementation of the Cocke-Younger-Kasami (CYK) algorithm for parsing sentences using context-free grammars.
   - **Key Features**:
     - Parsing of sentences using predefined grammars.
     - Step-by-step demonstration of the CYK algorithm.
   - **Use Case**: Syntax analysis for grammatical sentence verification.

---

### 6. **Other Notebooks**
   - **Word Embedding Techniques**
     - Explore word embeddings like Word2Vec, GloVe, and FastText.
   - **Sentiment Analysis**
     - Build sentiment analysis models using machine learning techniques.
   - **Text Summarization**
     - Implement extractive summarization techniques.

---

## 🛠️ Getting Started

### Prerequisites
To run the notebooks and scripts, ensure you have the following installed:
- **Python** (version 3.7 or higher)
- **Jupyter Notebook**
- Required Python libraries:
  ```bash
  pip install spacy nltk
  python -m spacy download en_core_web_sm
  ```

### Running the Repository
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/vyasdeepti/NLP-Basics.git
   ```
2. **Navigate to the Directory**:
   ```bash
   cd NLP-Basics
   ```
3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
4. **Explore the Notebooks**:
   Open any `.ipynb` file to explore and execute the code.

---

## Contribution Guidelines

We welcome contributions to enhance this repository! If you would like to contribute:
1. **Fork the Repository**:
   - Click the "Fork" button on the top-right corner of this repository.
2. **Create a Feature Branch**:
   ```bash
   git checkout -b feature-name
   ```
3. **Commit Your Changes**:
   ```bash
   git commit -am "Add new feature or fix"
   ```
4. **Push to Your Branch**:
   ```bash
   git push origin feature-name
   ```
5. **Submit a Pull Request**:
   - Create a pull request detailing the changes you’ve made.

---

## License

This repository is licensed under the **MIT License**. 

Thanks for exploring this repository! If you find it useful, consider giving it a ⭐ to show your support!
