# Word2Vec - Odd One Out

## Overview
This project utilizes the **Word2Vec model** to determine the **odd one out** from a set of words based on semantic similarities. By leveraging word embeddings, the model can identify the least related word in a given group.

## Features
- Train or load a **pre-trained Word2Vec model**
- Compute word similarities and differences
- Identify the **odd one out** from a list of words
- Interactive testing with custom word sets

## Installation
### Prerequisites
Ensure you have the following installed:
- Python (>= 3.7)
- Gensim
- Numpy
- Pandas
- Jupyter Notebook (for running the provided notebook)

### Install dependencies
```bash
pip install gensim numpy pandas jupyter
```

## Usage
### Running the Notebook
1. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Load and execute the `assignment_word2vec.ipynb` file.

### Example Usage
```python
from gensim.models import Word2Vec

# Load pre-trained model
model = Word2Vec.load("word2vec.model")

# Find the odd one out
words = ["apple", "banana", "car", "mango"]
odd_one = model.wv.doesnt_match(words)
print("Odd one out:", odd_one)
```

## Dataset
This model can be trained using a text corpus like:
- Google News Dataset (pre-trained model available)
- Wikipedia dumps
- Custom text data

## Contribution
Feel free to fork the repository and contribute with improvements. Pull requests are welcome!

## License
This project is open-source and available under the **MIT License**.

