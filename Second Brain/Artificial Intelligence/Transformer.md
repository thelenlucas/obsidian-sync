---
tags: Computer_Science/Machine_Learning
---
# Ghist

A transformer is a [[Machine Learning]] technique that utilizes [[Attention]] on itself to weight the signifigance of each part of it's input. Because models built with this technique can process all of it's input data at once, and receives data sequentially, they are naturally suited for [[Natural Laguage Processing]] applications. This data batching also makes parallelization much easier.

# Self Attention

Nominally, previous models, such as [[Recurrant Neural Network]]s processed information token by token, which allowed tokens to process down the sequence to an arbitrary length, but this procoess hurt training efforts on large datasets using current architectures. *Attention* allows for the pre-encoding of this information, making it much easier to fetch contextual information for the processing of natural language, especially for translation tasks.

This varied into the transformer network when research progressed from adding attention systems to RNN's, by processing all tokens simotaniously, then calculating attention weights inbetween layers.

# Architecture

Input is first passed through a [[Byte Pair Encoder]], which tokenizes the data. Each [[Token]] is then converted into a real-valued [[Vector]] via [[Word Embedding]].

The system uses a [[Encoder-Decoder]] architecture. 