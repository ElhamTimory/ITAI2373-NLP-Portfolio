# Lab 02: Basic NLP Preprocessing Techniques

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Elham Timory  
**Houston City College**

## Lab Overview

In this lab, I learned about different text preprocessing techniques used in Natural Language Processing (NLP). The main goal was to understand how to clean and prepare text before using it in machine learning models.

I used Python, NLTK, and spaCy to compare different preprocessing methods and see how they affect different types of text.

## What I Did

### 1. Tokenization
I practiced splitting text into smaller parts called tokens using NLTK and spaCy. I compared how both libraries handle words, punctuation, emojis, and hashtags.

### 2. Stopword Removal
I explored stopword lists in NLTK and spaCy and practiced removing common words that may not be important for some NLP tasks.

### 3. Stemming and Lemmatization
I compared stemming and lemmatization to understand how they reduce words to simpler forms. I learned that stemming cuts words using rules, while lemmatization tries to find their correct dictionary forms.

### 4. Text Cleaning
I practiced basic and advanced text cleaning, including handling punctuation, special characters, URLs, hashtags, and emojis.

### 5. Preprocessing Pipeline
I created a function that combines different preprocessing steps. I tested three configurations: Minimal, Standard, and Aggressive processing.

I also compared the results using five types of text: simple, academic, social media, news, and product reviews.

## Results

One interesting result was that NLTK produced 22 tokens for the social media example, while spaCy produced 23 because they handled the coffee emoji differently.

When testing the preprocessing pipeline on a product review containing 47 original tokens, I got these results:

| Processing Method | Tokens Remaining | Reduction |
|---|---:|---:|
| Minimal | 34 | 27.7% |
| Standard | 18 | 61.7% |
| Aggressive | 21 | 55.3% |

Standard processing removed the most tokens in this example, but removing more words does not always mean better results.

## Tools and Libraries

- Python
- Google Colab
- NLTK
- spaCy
- Regular expressions (`re`)

## How to Run

1. Open `L02_ElhamTimory_ITAI_2373.ipynb` in Google Colab.
2. Run the installation cells to install NLTK, spaCy, and the English language model.
3. Run the remaining cells in order.
4. Review the tokenization, cleaning, and preprocessing results.

The lab uses sample text included in the notebook, so no separate dataset is needed.

## What I Learned

This lab helped me understand that text preprocessing is an important step in NLP. I learned how tokenization, stopword removal, stemming, and lemmatization work and how they can change the original text.

I also learned that different preprocessing methods have different advantages and limitations. The best method depends on the type of text and what we want the NLP system to do.
