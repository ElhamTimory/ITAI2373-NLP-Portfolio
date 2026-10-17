# Lab 04: Text Representation

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Elham Timory  
**Houston City College**

## Lab Overview

In this lab, I learned how computers convert text into numerical representations that machine learning models can understand. I explored different methods, including Bag of Words (BoW), TF-IDF, n-grams, and word embeddings.

The main goal was to understand how these methods work, compare their advantages and limitations, and see how they can be used for text classification.

## What I Did

### 1. Text Preprocessing

I practiced cleaning movie reviews by converting text to lowercase, removing punctuation and stopwords, tokenizing sentences, and applying stemming. These steps helped prepare the text for numerical representation.

### 2. Bag of Words (BoW)

I implemented Bag of Words from scratch and compared it with scikit-learn's `CountVectorizer`.

I learned that BoW counts how often words appear in documents, but it does not preserve word order or fully understand context.

### 3. TF-IDF

I implemented TF-IDF calculations and compared my results with scikit-learn's `TfidfVectorizer`.

TF-IDF gives more importance to words that help distinguish documents by considering how frequently words appear and how common they are across the dataset.

### 4. N-grams and Document Similarity

I explored unigrams, bigrams, and trigrams to understand how combining nearby words can preserve some word order.

I also used cosine similarity to compare documents based on their numerical representations.

### 5. Word Embeddings

I explored pretrained word embeddings using Gensim.

I learned that word embeddings represent words using dense vectors and can capture similarities and relationships between words.

### 6. Text Classification

I used the NLTK movie reviews dataset to build text classification models using Bag of Words, TF-IDF, and n-gram features.

I trained Multinomial Naive Bayes classifiers and compared how different text representations affected classification accuracy.

I also analyzed important words that contributed to the model's predictions.

## Classification Results

The original NLTK movie reviews dataset contained 2,000 reviews. For this experiment, I used a subset of 200 reviews, with 140 for training and 60 for testing.

| Representation | Accuracy |
|---|---:|
| Bag of Words | 63.3% |
| N-grams | 60.0% |
| TF-IDF | 58.3% |

Bag of Words achieved the highest accuracy in this experiment. This showed me that more advanced text representation methods do not always produce better results, especially when working with a small dataset.

## Tools and Libraries

- Python
- Google Colab
- NLTK
- scikit-learn
- Gensim
- NumPy
- pandas
- Matplotlib
- Seaborn

## How to Run

1. Open `L04_Elham_Timory_ITAI_2373.ipynb` in Google Colab.
2. Run the installation and import cells.
3. Download the required NLTK resources when prompted.
4. Run the notebook cells in order.
5. Review the preprocessing, text representation, word similarity, and classification results.

The notebook uses sample movie reviews and the NLTK movie reviews dataset. It also uses pretrained word embeddings, which may require an additional download.

## What I Learned

This lab helped me understand why computers need to convert text into numbers before using it in traditional machine learning models.

I learned the differences between sparse representations, such as BoW and TF-IDF, and dense representations, such as word embeddings. I also learned that n-grams can preserve some word order, while embeddings can represent similarities between words.

By comparing different classification methods, I learned that the best text representation depends on the dataset and the task.

I also explored real-world NLP applications and ethical considerations, including bias, privacy, and fairness.
