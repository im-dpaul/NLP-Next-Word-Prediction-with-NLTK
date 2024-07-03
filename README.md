# Next Word Prediction using NLTK

The goal of this project is to predict the next word in a sentence using the NLTK library and the Reuters corpus. By leveraging bigrams and conditional frequency distributions, the model suggests the most likely word to follow a given input word, enhancing text prediction capabilities.

### Table of Contents:

1. [Importing Libraries & Loading Data](#importing-libraries-and-loading-data)
2. [Creating Bigrams](#creating-bigrams)
3. [Creating Conditional Frequency Distribution](#creating-conditional-frequency-distribution)
4. [Predicting Next Word](#predicting-next-word)
5. [Conclusion](#conclusion)

## Importing Libraries and Loading Data

The project begins by importing essential libraries from `NLTK`, specifically for natural language processing tasks. The `reuters` corpus is used as the dataset, and additional `NLTK` modules for tokenization and bigram creation are also loaded. This setup ensures that the necessary tools for text processing are readily available.

The Reuters corpus is loaded, which provides a comprehensive collection of sentences from news articles. This dataset serves as the foundation for training the model, ensuring that it is exposed to a wide variety of real-world text data. The size and structure of the dataset are also examined to understand the scope of the data being worked with.

## Creating Bigrams

Bigrams, or pairs of consecutive words, are created from the corpus. By analyzing these word pairs, the model gains insight into common word sequences. This step involves tokenizing the text into individual words, converting them to lowercase for uniformity, and forming bigrams to capture the relationship between adjacent words.

## Creating Conditional Frequency Distribution

A conditional frequency distribution (CFD) is constructed from the bigrams. This distribution helps in determining the frequency of occurrence of a word given its preceding word. By querying this CFD, the model can predict the most likely next word for any given input word, based on historical data from the corpus.

## Predicting Next Word

The final step involves using the CFD to predict the next word. A function is implemented that takes an input word, converts it to lowercase, and searches the CFD for the most frequent word that follows the input word. If the input word is found in the CFD, the most common subsequent word is returned; otherwise, a message indicating the absence of the word in the corpus is displayed.

## Conclusion

This project demonstrates how to use NLTK and bigrams to build a simple yet effective next-word prediction model. Such models can significantly enhance user experience in text-based applications by providing intelligent word suggestions.
