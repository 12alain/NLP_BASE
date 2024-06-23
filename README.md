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



