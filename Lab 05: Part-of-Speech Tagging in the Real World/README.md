
# Lab 05: Part-of-Speech (POS) Tagging

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Elham Timory  
**Houston Community College**

## Lab Overview

In this lab, I learned how Part-of-Speech (POS) tagging helps computers identify the grammatical roles of words in sentences. I used NLTK and spaCy to compare different tagging methods and understand how context can affect the meaning and grammatical role of a word.

The lab included basic POS tagging exercises and more advanced examples using informal text, customer service transcripts, and unusual sentence structures.

## What I Did

### 1. Basic POS Tagging

I used NLTK and spaCy to identify nouns, verbs, adjectives, adverbs, and other parts of speech.

I compared the results from both libraries and learned that they sometimes assign different tags to the same word.

### 2. Comparing POS Tag Sets

I compared the Penn Treebank and Universal tag sets.

Penn Treebank provides more detailed grammatical information, while Universal tags use simpler categories that are easier to understand.

### 3. Word Ambiguity

I explored words such as *lead* and *bank*, which can have different grammatical roles depending on the sentence.

I learned that surrounding words and sentence structure help POS taggers determine how a word is being used.

### 4. Processing Informal Text

I tested NLTK and spaCy on text containing slang, contractions, emojis, abbreviations, and speech transcripts.

Both libraries processed the examples, but I learned that assigning a tag does not necessarily mean the tag is correct.

### 5. Customer Service Analysis

I analyzed four simulated customer service transcripts involving account access, technical issues, billing, and user guidance.

I used spaCy to identify emotional adjectives, action verbs, and problem-related nouns. I also created visualizations to compare sentiment scores, common words, and urgency indicators.

This exercise helped me understand how NLP could be used to analyze customer problems and support ticket routing.

### 6. POS Tagger Performance Comparison

I compared NLTK and spaCy using five types of text: formal, informal, technical, conversational, and mixed.

I measured processing time and examined potentially problematic tags.

### 7. Edge Cases and Error Analysis

I tested difficult sentences containing repeated words, ambiguous grammar, social media symbols, and technical terms.

These examples helped me understand why POS tagging can be challenging when sentences have unusual structures or unclear meanings.

## Results and Observations

Some interesting findings from this lab were:

- NLTK tagged *brown* as a noun in the example sentence, while spaCy correctly identified it as an adjective.
- In the sentence "I bank with Chase," NLTK tagged *bank* as a noun, even though it was used as a verb.
- Both libraries showed a 100% success rate under the lab's selected problematic-tag test for the informal samples, but this did not prove that all their tags were correct.
- NLTK was generally faster in the performance comparison, although the experiment did not directly measure tagging accuracy.
- Customer service analysis showed how nouns, verbs, and descriptive words could help identify different types of customer problems.

## Tools and Libraries

- Python
- Google Colab
- NLTK
- spaCy
- pandas
- Matplotlib
- Seaborn

## How to Run

1. Open `L05_Timory_Elham_ITAI2373_.ipynb` in Google Colab.
2. Run the installation cells for NLTK, spaCy, and the required libraries.
3. Download the NLTK resources and spaCy English language model.
4. Run the remaining cells in order.
5. Review the POS tagging results, comparisons, visualizations, and reflections.

The notebook includes the sample sentences and simulated customer service transcripts, so no separate dataset is required.

## What I Learned

This lab helped me understand how POS tagging works and why grammar and context are important in Natural Language Processing.

I learned that NLTK and spaCy have different advantages. NLTK is useful for learning and experimenting with detailed tag sets, while spaCy provides readable tags and other tools for larger NLP applications.

I also learned that POS tagging has limitations when dealing with slang, ambiguous words, and complicated sentences. In real-world applications, preprocessing and human review may sometimes be needed to improve the results.

Overall, this lab gave me more practice with Python and helped me understand how POS tagging can support other NLP tasks.
