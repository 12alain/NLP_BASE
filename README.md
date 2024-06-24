# [Natural Language Processing (NLP)](#natural-language-processing-nlp)

## 1. [Text Preprocessing](#text-preprocessing)
### [1.1. Tokenization](#11-tokenization)
### [1.2. Noise Removal](#12-noise-removal)

## 2. [Text Normalization](#text-normalization)
### [2.1. Introduction](#21-introduction)
### [2.2. Stemming](#22-stemming)
### [2.3. Lemmatization](#23-lemmatization)

## 3. [Word Embedding](#word-embedding)
### [3.1. Frequency-based Word Embedding](#31-frequency-based-word-embedding)
### [3.2. Precision-based Word Embedding](#32-precision-based-word-embedding)
### [3.5. Contextual Embeddings (BERT, GPT)](#35-contextual-embeddings-bert-gpt)

## [Conclusion](#conclusion)

# Natural Language Processing (NLP)

Natural Language Processing (NLP), in its simplest form, is the ability for a computer/system to truly understand human language and process it in the same way humans do.

## 1. Text Preprocessing

The entire process of cleaning and normalizing text, making it free of noise and ready to be analyzed, is called text preprocessing.

### 1.1. Noise Removal

Anything in text that is not relevant in the context of the data and the final result can be specified as noise. Examples include:

- Stop-words (commonly used words in a language such as is, am, the, of, in; in French: le, la, te, me, à, etc.)
- URLs or links
- Social media entities (mentions, hashtags)
- Punctuation
- Emojis
- Numeric values

### 1.2. Tokenization

Tokenization is a way of breaking down text into smaller units called tokens. Tokens can be words, characters, or subwords. Thus, tokenization can be classified into three types: word tokenization, character tokenization, and subword (n-grams) tokenization.

- Character tokenization
```
word: "Intelligent"

tokens: ["I","n","t","e","l","l","i","g","e","n","t"]

```
- Word tokenization
```
sentence: "I am alone"
tokens: ["I", "am", "alone"]
```
- Tokenization into subwords (n-grams)

```
sentence: "I am onlone "
tokens: ["am alone"]
```

## 2. [Text Normalization](#text-normalization)

Text normalization is the process of transforming text into
a canonical (standard) form.

We have two main methods of text normalization:
**Stemming** : is a rules-based process that involves
remove suffixes (“ing”, “ly”, “es”, “s”, etc.) from a word.
- Porter Stemmer
- Snowball Stemmer
- Lancaster Stemmer 

**Lemmatization**: is for its part, is an organized procedure, step
step by step, allowing you to obtain the root of the word.
- WordNetLemmatizer

## 3. [Word Embedding](#word-embedding)

The different types of Word Embeddings can be classified into two main categories.

**Frequency-based Word Embeddings**
- Count Vector
- BOW
- TF-IDF (Term Frequency-Inverse Document Frequency)
**Prediction-based Word Embeddings**
- CBOW (Continuous Bag of words)
- Skip-Gram (Word2Vec)
- GloVe (Global Vectors for Word Representation)

### [3.5. Contextual Embeddings (BERT, GPT)](#35-contextual-embeddings-bert-gpt)

Contextual embeddings such as BERT and GPT represent a significant advancement in natural language processing by capturing the meaning of words based on their context.

**BERT (Bidirectional Encoder Representations from Transformers)**

BERT utilizes a bidirectional Transformer model pre-trained on large textual corpora. It generates embeddings that capture semantic nuances by considering words both to the left and right of each word in a sentence.

**GPT (Generative Pre-trained Transformer)**

Similar to BERT but typically used for text generation, GPT is a pre-trained Transformer model that produces contextual embeddings by predicting the next word in a sequence of words.
