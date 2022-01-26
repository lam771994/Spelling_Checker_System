# Spelling Checker System

## Objectives

To design and implement a spellcheck system that makes use of a probabilistic model to detect and correct the spelling of the inputs provided by a user. The system was built so that it can detect and correct both non-word and real-word errors by making use of Minimum Edit Distance and N-grams respectively. A Graphical User Interface (GUI) was utilized to receive user input, which is cross-referenced against the system’s corpus to detect errors and suggest alternate options with the highest probabilities of being correct. 

The domain of digital marketing is used to build the corpus. Including domain-specific abbreviations, it contains a total of 202,707 tokens, of which 10,254 are unique tokens or vocabulary that are stored in the form of a variable. 

## Schematic Representation of Spellcheck System Design

![alt text](https://github.com/lam771994/Spelling_Checker_System/blob/main/images/Spell_Checker_System_Flowchart.png)

## Implemented Spelling Checker System

https://user-images.githubusercontent.com/68948128/151116590-e2838c72-f66b-49b1-a1c0-9423d306b0d5.mp4

## Strengths & Limitations of the System

![alt text](https://github.com/lam771994/Spelling_Checker_System/blob/main/images/Strengths_Limitations_NLP.png)

## Recommendations

The application of the techniques listed below could potentially improve the spelling checker system:

1. Parts of Speech (POS) Tagging

- POS Tagging labels each word in a sentence with its appropriate part of speech, depending on the definition of the word and its context
- Parts of speech include nouns, verb, adverbs, adjectives, pronouns, conjunction and their sub-categories.
- Stochastic POS tagging (probabilistic model)- word frequency approach (chooses most frequent tags associated with a word in the corpus) and tag sequence probabilities 
- There would be no probability for the words that do not exist in the corpus – non-word errors (replace edit distance)
- The best tag for a given word is determined by the probability at which it occurs with the n previous tags – real word errors (similar to ngram)
- POS Tagging performance: 97%

2. Information Retrieval (IR)

- IR can be used to improve the system by accessing and retrieving the correct words from the corpus that matches the user’s input with the help of context-based indexing
- There are 2 processes in IR: indexing (tokenization of string, removal of frequent words & stemming) and matching (finding a measure of similarity between 2 text representations)
- Vector space model (probabilistic model): based on Luhn’s similarity criterion
- The more 2 text representations agreed in given elements and distribution, the higher the probability of their representing similar context/information
- This model is ideal for both non-word and real word errors because it allows computing a continuous degree of similarity between queries and corpus

3. Semantics

- Semantic analysis is to identify the relationships between the individual words of the sentence in a particular context
- The relationship between individual words requires the understanding of lexical hierarchy such as synonyms, hyponymy, antonyms, etc.…
- Text classification model: assigns pre-defined categories to text 
- Semantic analysis can be implemented with the help of machine learning algorithms 
- The algorithms can detect and correct real word errors with the classified relationships based on the past results
- Semantic analysis is specifically ideal for correcting real word errors because it understands the context of the words and it is able to accurately disambiguate the proper meaning of words that have more than one definition




