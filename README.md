---

# NLP Preprocessing Notebook

A repository dedicated to exploring foundational concepts in Natural Language Processing (NLP). This project includes implementations of key algorithms and techniques to help learners and practitioners gain a solid understanding of NLP fundamentals. This Jupyter Notebook showcases various foundational techniques for natural language preprocessing using the Natural Language Toolkit (NLTK) in Python. It is designed as a practical guide for exploring common text preprocessing tasks that are essential for Natural Language Processing (NLP) projects.


# NLP Basics
A repository dedicated to exploring foundational concepts in Natural Language Processing (NLP). This project includes implementations of key algorithms and techniques to help learners and practitioners gain a solid understanding of NLP fundamentals.

Features
CYK Algorithm Implementation: The repository includes a Python implementation of the CYK (Cocke-Younger-Kasami) algorithm, which is used for syntactic parsing of sentences using context-free grammars. The provided implementation demonstrates:
Non-terminal and terminal symbol definitions.
Grammar rules for parsing.
A step-by-step parsing process to determine if a sentence conforms to the defined grammar.
Example usage with a sample sentence: "a very heavy orange book".
Technologies Used
Jupyter Notebooks: The primary format for interactive code demonstrations and analysis.
Python: Employed for implementing NLP algorithms, leveraging its simplicity and robust library ecosystem.
Getting Started
Clone the repository:
bash
git clone https://github.com/vyasdeepti/NLP-Basics.git
Navigate to the repository directory:
bash
cd NLP-Basics
Explore the CYK script to understand the CYK algorithm.
Usage
Run the CYK script to test the parsing algorithm with custom sentences.
Modify the grammar rules or terminal symbols to adapt the algorithm to new contexts.


# NLP Preprocessing Notebook
This Jupyter Notebook showcases various foundational techniques for natural language preprocessing using the Natural Language Toolkit (NLTK) in Python. It is designed as a practical guide for exploring common text preprocessing tasks that are essential for Natural Language Processing (NLP) projects.

## Features and Highlights
1. Stop Words Removal
Demonstrates how to remove stop words (e.g., 'and', 'the') from text using NLTK's stopwords module.
Customizes the stop words list to include additional punctuation marks.
2. Stemming
Implements stemming using the PorterStemmer to reduce words to their root forms (e.g., "playing" -> "play").
Applies stemming to sentences, showcasing its impact on reducing word variations.
3. Lemmatization
Uses the WordNetLemmatizer for lemmatization, which reduces words to their base or dictionary form (e.g., "rocks" -> "rock").
Handles pluralization and irregular forms effectively (e.g., "wolves" -> "wolf").
4. Tokenization
Applies both word and sentence tokenization using NLTK's word_tokenize and sent_tokenize methods.
Splits text into manageable tokens for further processing.
5. Parts-of-Speech Tagging
Tags tokens with their respective parts of speech (e.g., noun, verb) using NLTK's pos_tag function.
Demonstrates tagging in sentences and its role in syntactic analysis.
Getting Started
Prerequisites
Ensure you have Python installed with the following libraries:

NLTK
Install missing libraries using:

bash
pip install nltk
Running the Notebook
Clone this repository:

bash
git clone https://github.com/vyasdeepti/NLP-Basics.git
Navigate to the directory:

bash
cd NLP-Basics
Launch Jupyter Notebook:

bash
jupyter notebook NLP_Preprocessing_2.ipynb
Follow the cells sequentially to explore the preprocessing steps.

Usage
This notebook provides a hands-on introduction to preprocessing tasks in NLP. It can be used as a starting point for projects requiring clean and structured text data.



# Named Entity Recognition (NER) Notebook
This Jupyter Notebook demonstrates the implementation of Named Entity Recognition (NER) using the spaCy library. It provides a comprehensive walkthrough for identifying and visualizing entities in a text, such as persons, organizations, locations, dates, and more.

Features
1. Setup and Installation
Installs necessary Python libraries:
spaCy for NLP tasks.
en_core_web_sm, a spaCy language model.
Includes commands to ensure all dependencies are properly configured.
2. Text Processing with spaCy
Loads and processes textual data using the en_core_web_sm language model.
Demonstrates tokenization to break down text into individual words and components.
3. Named Entity Recognition (NER)
Extracts named entities from the text, including:
PERSON: Names of people.
ORG: Organizations.
DATE: Dates and time expressions.
GPE: Geopolitical entities like cities, countries, or states.
ORDINAL: Ordinal numbers like '1st', '2nd', etc.
Identifies the start and end positions of entities along with their labels.
4. Visualization
Utilizes spaCy's displacy module to render and visualize named entities directly in the notebook.
Highlights entities with different colors for easy identification.
5. Example Text
Processes a sample text about Barack Obama, illustrating NER capabilities on real-world data:
"Barack Hussein Obama II is an American politician who served as the 44th president of the United States from 2009 to 2017."

Getting Started
Prerequisites
Ensure you have Python and Jupyter Notebook installed. Install the required libraries using:

bash
pip install spacy
python -m spacy download en_core_web_sm
Running the Notebook
Clone the repository:

bash
git clone https://github.com/vyasdeepti/NLP-Basics.git
Navigate to the repository directory:

bash
cd NLP-Basics
Launch Jupyter Notebook:

bash
jupyter notebook NamedEntityRecognition.ipynb
Execute the cells sequentially to explore the NER implementation.




Word Frequency Analysis Notebook
This Jupyter Notebook provides a practical implementation of word frequency analysis using the spaCy library. The notebook processes a sample text and identifies the most frequently occurring words, excluding stop words and punctuation.

Features
1. Text Processing
Utilizes spaCy's en_core_web_sm language model to process and tokenize text.
Handles complex text structures, including sentences, punctuation, and stop words.
2. Word Frequency Analysis
Extracts meaningful words from the text after filtering out:
Stop words: Commonly used words (e.g., "and", "the") that don't add significant meaning.
Punctuation.
Counts the occurrences of each word using Python's collections.Counter.
3. Sample Text
Analyzes a predefined text about Gus Proto, a Python developer, covering topics such as:
His interests in Natural Language Processing.
His activities in organizing meetups and talks.
His passion for learning to play the piano.
4. Top Words
Outputs the top 10 most frequent words along with their counts.
Example output:
Code
[('Gus', 4), ('London', 3), ('Natural', 3), ('Language', 3), ('Processing', 3), ('Piano', 3), ('Python', 2), ('developer', 2), ('Fintech', 2), ('learning', 2)]
Getting Started
Prerequisites
Ensure you have Python installed with the following libraries:

spaCy
Install the required libraries using:

bash
pip install spacy
python -m spacy download en_core_web_sm
Running the Notebook
Clone this repository:

bash
git clone https://github.com/vyasdeepti/NLP-Basics.git
Navigate to the directory:

bash
cd NLP-Basics
Launch Jupyter Notebook:

bash
jupyter notebook WordFrequency_.ipynb
Follow the cells sequentially to understand and execute the word frequency analysis.








## Technologies Used

- **Jupyter Notebooks**: The primary format for interactive code demonstrations and analysis.
- **Python**: Employed for implementing NLP algorithms, leveraging its simplicity and robust library ecosystem.


## Usage

This notebook provides a hands-on introduction to preprocessing tasks in NLP. It can be used as a starting point for projects requiring clean and structured text data.

## Contributions

Contributions are welcome! Feel free to fork the repository and submit pull requests to enhance its capabilities.

---


