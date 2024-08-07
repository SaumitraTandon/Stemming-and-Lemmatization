# Stemming and Lemmatization

## Introduction

This project demonstrates the concepts and implementation of stemming and lemmatization, two fundamental techniques in natural language processing (NLP) for text normalization. These techniques are essential for reducing words to their base or root forms, thereby simplifying text data and enhancing the performance of various NLP tasks.

## Stemming and Lemmatization

### Stemming

Stemming is the process of reducing a word to its base or root form. The resulting stemmed word may not always be a valid word in the language but is sufficient for the purposes of text normalization. Stemming algorithms, such as the Porter Stemmer and Snowball Stemmer, use a set of heuristic rules to remove suffixes from words.

#### Example of Stemming:
- **Running** -> **Run**
- **Studies** -> **Studi**
- **Happiness** -> **Happi**

### Lemmatization

Lemmatization is a more sophisticated process that reduces a word to its lemma, the canonical form that is found in dictionaries. Unlike stemming, lemmatization takes into account the morphological analysis of the words and uses vocabulary and grammatical analysis to determine the correct base form of the word.

#### Example of Lemmatization:
- **Running** -> **Run**
- **Studies** -> **Study**
- **Better** -> **Good**

## Installation

To run the code in this project, you need to have Python installed. The required libraries can be installed using pip:

```bash
pip install -r requirements.txt
```

## Usage

This project includes a Jupyter notebook that demonstrates the stemming and lemmatization processes. To use the notebook, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/stemming-and-lemmatization.git
    ```

2. Navigate to the project directory:

    ```bash
    cd stemming-and-lemmatization
    ```

3. Install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

4. Open the Jupyter notebook:

    ```bash
    jupyter notebook Stemming_and_Lemmatization.ipynb
    ```

5. Follow the instructions in the notebook to see examples of stemming and lemmatization.

## Examples

### Stemming Example

```python
from nltk.stem import PorterStemmer

stemmer = PorterStemmer()
words = ["running", "studies", "happiness"]
stems = [stemmer.stem(word) for word in words]

print(stems)
# Output: ['run', 'studi', 'happi']
```

### Lemmatization Example

```python
from nltk.stem import WordNetLemmatizer

lemmatizer = WordNetLemmatizer()
words = ["running", "studies", "better"]
lemmas = [lemmatizer.lemmatize(word, pos='v') for word in words]

print(lemmas)
# Output: ['run', 'study', 'good']
```

## Contributing

We welcome contributions to this project! If you would like to contribute, please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes with descriptive commit messages.
4. Push your changes to your fork.
5. Open a pull request to the main repository.

## Contact

If you have any questions or suggestions, feel free to open an issue or contact us at hellosaumitra@gmail.com.
