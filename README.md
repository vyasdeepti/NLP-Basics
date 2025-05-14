 # $${\color{red} NATURAL LANGUAGE PROCESSING 📚📚 }$$
# NATURAL LANGUAGE PROCESSING 📚📚 


Welcome to the **NLP Basics** repository! This repository serves as a comprehensive guide for beginners and enthusiasts to explore the foundational concepts and techniques in **Natural Language Processing (NLP)**. It contains interactive Jupyter Notebooks and Python scripts that demonstrate various NLP workflows, algorithms, and applications.

Natural Language Processing (NLP) is a subfield of Artificial Intelligence (AI) and linguistics that focuses on the interaction between computers and human language. NLP enables machines to understand, interpret, and generate human language in a way that is both meaningful and useful.

**Key Goals of NLP**:
- Language Understanding: 
The ability to comprehend the meaning behind words, sentences, and context.
Examples: Sentiment analysis, text classification, entity recognition.

- Language Generation:
The ability to produce coherent and contextually relevant human-like text.
Examples: Text summarization, chatbots, machine translation.

**Why is NLP Important?**


NLP enables machines to bridge the gap between human communication and computers, making technology more accessible and human-friendly. It powers many modern applications that improve efficiency, automate tasks, and enhance user experiences in various domains like healthcare, finance, education, and entertainment.

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

### **Examples**


1. **Input Text:** *"I love programming in Python!"*
2. **After Text Cleaning:** *"i love programming in python"*
3. **Tokens:** *["i", "love", "programming", "in", "python"]*
4. **Stopwords Removed:** *["love", "programming", "python"]*
5. **Stemming/Lemmatization:** *["lov", "program", "python"]* or *["love", "program", "python"]*


---

### 2. **Named Entity Recognition (NER)**
   - **File**: `NamedEntityRecognition.ipynb`
   - **Description**: Demonstrates how to extract and visualize named entities (e.g., persons, organizations, locations) using the `spaCy` library.
   - **Key Features**:
     - Extraction of entities with labels such as PERSON, ORG, DATE, etc.
     - Visualization of entities using `displacy`.
   - **Use Case**: Identify key entities from unstructured text data.

Input Sentence:
"Barack Obama was born on August 4, 1961, in Honolulu, Hawaii, and served as the 44th President of the United States."

NER Output:
The sentence with recognized entities is as follows:

  Barack Obama → Person
  August 4, 1961 → Date
  Honolulu → Location
  Hawaii → Location
  44th → Ordinal
  United States → Location

---

### 3. **Word Frequency Analysis**
   - **File**: `WordFrequency_.ipynb`
   - **Description**: Analyzes word frequencies in text data using `spaCy`.
   - **Key Features**:
     - Tokenization and filtering of stop words and punctuation.
     - Identification of the top 10 most frequent words.
   - **Use Case**: Understand the most commonly used terms in a text dataset.

Example of Word Frequency Analysis
Input Text:
"I love programming in Python. Python is an amazing programming language that I love."

Steps for Word Frequency Analysis:

Text Cleaning: Convert text to lowercase, remove punctuation, and split into words (tokens).

Example:

["i", "love", "programming", "in", "python", "python", "is", "an", "amazing", "programming", "language", "that", "i", "love"]

Count Word Frequencies: Count the occurrences of each word.

Example:


{
    "i": 2,
    "love": 2,
    "programming": 2,
    "in": 1,
    "python": 2,
    "is": 1,
    "an": 1,
    "amazing": 1,
    "language": 1,
    "that": 1
}

Sort by Frequency : Sort the words by their frequency in descending order.

Example:

[
    ("i", 2),
    ("love", 2),
    ("programming", 2),
    ("python", 2),
    ("in", 1),
    ("is", 1),
    ("an", 1),
    ("amazing", 1),
    ("language", 1),
    ("that", 1)
]





---

### 4. **Bigram Generation**
   - **File**: `convert_in_Biagram.ipynb`
   - **Description**: Generates bigrams (pairs of consecutive words) from a list of sentences.
   - **Key Features**:
     - Efficient implementation using Python's list comprehensions.
     - Example with sentences about flowers and their significance.
   - **Use Case**: Analyze word pair relationships for text modeling tasks.


### Example of Bigram Generation in NLP

**Input Text:**  
*"I love programming in Python"*

---

### Steps to Generate Bigrams:

1. **Tokenization:**  
   - Split the text into individual tokens (words).  
   - Example: *["I", "love", "programming", "in", "Python"]*

2. **Generate Bigrams:**  
   - A bigram is a pair of two consecutive words.  
   - Example: *[("I", "love"), ("love", "programming"), ("programming", "in"), ("in", "Python")]*

---

### Python Code Example:

```python
from nltk import bigrams

# Input text
text = "I love programming in Python"

# Tokenization
tokens = text.split()

# Generate bigrams
bigram_list = list(bigrams(tokens))

print(bigram_list)
```

**Output:**  
```
[('I', 'love'), ('love', 'programming'), ('programming', 'in'), ('in', 'Python')]
```

---

### Visualization (Optional)
You can visualize bigrams as a graph or a frequency distribution:

```python
from collections import Counter
import matplotlib.pyplot as plt

# Count bigram frequencies
bigram_counts = Counter(bigram_list)

# Plot the bigram frequency distribution
bigram_labels, frequencies = zip(*bigram_counts.items())
plt.bar([" ".join(bigram) for bigram in bigram_labels], frequencies)
plt.xticks(rotation=45)
plt.xlabel("Bigrams")
plt.ylabel("Frequency")
plt.title("Bigram Frequency Distribution")
plt.show()
```

---

### Use Cases of Bigrams:
- Text prediction (e.g., "I love" → "programming").
- Analyzing word pair relationships in a corpus.
- Building language models.


---

### 5. **CYK Algorithm**
   - **File**: `CYK.ipynb`
   - **Description**: Implementation of the Cocke-Younger-Kasami (CYK) algorithm for parsing sentences using context-free grammars.
   - **Key Features**:
     - Parsing of sentences using predefined grammars.
     - Step-by-step demonstration of the CYK algorithm.
   - **Use Case**: Syntax analysis for grammatical sentence verification.

     
### Example of CYK Algorithm (Cocke-Younger-Kasami Algorithm)

The CYK algorithm is used to determine if a given string can be generated by a given context-free grammar in Chomsky Normal Form (CNF). It builds a triangular table to parse the string.

---

### **Problem Example**

#### Context-Free Grammar in CNF:
We need the grammar in Chomsky Normal Form (CNF):
```
S → AB | BC
A → BA | a
B → CC | b
C → AB | a
```

#### Input String:
`"baaba"`

---

### **Steps of the CYK Algorithm**

1. **Prepare the Table:**  
   Create a triangular table where rows represent substrings of increasing lengths, starting from 1.

2. **Initialize the First Row:**  
   The first row corresponds to substrings of length 1. Check which grammar rules produce each character in the string.

3. **Fill the Table for Substrings of Length 2 to n:**  
   For each cell, combine results from shorter substrings (based on grammar rules) to determine possible non-terminals.

4. **Check for S in the Top Cell:**  
   If the start symbol `S` is in the top-right cell of the table, the string can be generated by the grammar.

---

### **CYK Table Example**

#### Input String: `"baaba"`

1. **Step 1: Initialize Table with Length 1 Substrings**
   ```
   |  b  |  a  |  a  |  b  |  a  |
   | {B} | {A,C} | {A,C} | {B} | {A,C} |
   ```

2. **Step 2: Fill Length 2 Substrings**
   - Combine adjacent substrings:
     ```
     | {B}  | {A,C} | {A,C} | {B}  | {A,C} |
     | {S}  | {S,A} | {S,A} | {S}  |       |
     ```

3. **Step 3: Fill Length 3 Substrings**
   - Combine pairs of substrings:
     ```
     | {B}  | {A,C} | {A,C} | {B}  | {A,C} |
     | {S}  | {S,A} | {S,A} | {S}  |       |
     | {S}  | {S,A} | {S}   |       |       |
     ```

4. **Step 4: Fill Length 4 and 5 Substrings**
   - Combine larger substrings:
     ```
     | {B}  | {A,C} | {A,C} | {B}  | {A,C} |
     | {S}  | {S,A} | {S,A} | {S}  |       |
     | {S}  | {S,A} | {S}   |       |       |
     | {S}  | {S}   |       |       |       |
     ```

5. **Final Check:**  
   The top-right cell contains `{S}`, meaning the string `"baaba"` can be generated by the grammar.

---

### Python Implementation (Optional Code):

```python
from collections import defaultdict

# Function to implement CYK Algorithm
def cyk_algorithm(grammar, string):
    # Convert grammar rules to a dictionary
    rules = defaultdict(list)
    for head, body in grammar:
        rules[body].append(head)

    # Length of the input string
    n = len(string)

    # Initialize the CYK table
    table = [[set() for _ in range(n)] for _ in range(n)]

    # Fill the first row of the table
    for i, char in enumerate(string):
        for lhs in rules[char]:
            table[i][i].add(lhs)

    # Fill the rest of the table
    for length in range(2, n + 1):  # Length of the span
        for i in range(n - length + 1):  # Start of the span
            j = i + length - 1  # End of the span
            for k in range(i, j):  # Split point
                for B in table[i][k]:
                    for C in table[k + 1][j]:
                        if B + C in rules:
                            for lhs in rules[B + C]:
                                table[i][j].add(lhs)

    # Check if the start symbol is in the top-right cell
    return 'S' in table[0][n - 1]

# Grammar in CNF: (Head, Body)
grammar = [
    ("S", "AB"), ("S", "BC"),
    ("A", "BA"), ("A", "a"),
    ("B", "CC"), ("B", "b"),
    ("C", "AB"), ("C", "a")
]

# Input string
string = "baaba"

# Run CYK Algorithm
result = cyk_algorithm(grammar, string)
print("String can be generated by the grammar:" if result else "String cannot be generated by the grammar.")
```

**Output:**
```
String can be generated by the grammar.
```

---


---

### 6. **Other Notebooks**
   - **Word Embedding Techniques**
     - Explore word embeddings like Word2Vec, GloVe, and FastText.
   - **Sentiment Analysis**
     - Build sentiment analysis models using machine learning techniques.
   - **Text Summarization**
     - Implement extractive summarization techniques.

---
```bash
+--------------------+
|   Raw Text Input   |
+--------------------+
          |
          v
+--------------------+
| Text Preprocessing |
+--------------------+
          |
          v
+--------------------+
| Feature Extraction |
| (e.g., word vectors|
| or embeddings)     |
+--------------------+
          |
          v
+------------------------------+
| NLP Tasks                   |
| - Text Classification       |
| - Sentiment Analysis        |
| - Named Entity Recognition  |
| - Machine Translation       |
| - Question Answering        |
| - Text Summarization        |
+------------------------------+
          |
          v
+--------------------+
|   Output Results   |
| (Predictions, etc.)|
+--------------------+

This pipeline demonstrates how raw text transitions through preprocessing, feature extraction, and task-specific models to produce meaningful results.
```

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
