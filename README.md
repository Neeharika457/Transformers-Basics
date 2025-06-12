# What are Transformers?
Transformers are a type of neural network architecture designed to handle sequential data, like text. They were introduced in the 2017 paper "Attention is All You Need" and have since powered models like BERT, GPT, T5, and many others.

They work by using attention mechanisms to learn which parts of the input are important — instead of relying on step-by-step memory like RNNs.

## 🧠 Basic Structure
A Transformer has two main parts:

1. 🔐 Encoder — Understands the input
Takes in the input text (e.g., a sentence like "I love pizza")

Converts it into a set of vector representations

Uses self-attention to figure out which words in the sentence are important to each other

The encoder is used in models like BERT (used for classification, question answering, etc.)

🧩 Think of the encoder as a really smart reader — it reads the sentence and creates a deep understanding of the meaning of each word in context.

2. 🗣️ Decoder — Generates output (used in translation, summarization, etc.)
Takes the encoded information from the encoder

Uses it to generate new sequences, like translating a sentence into another language

Also uses self-attention + encoder-decoder attention

The decoder is used in models like GPT

🎯 In models like GPT, the decoder predicts the next word one at a time.

## 🔍 What is Attention?
Attention lets the model focus on relevant words while processing input. For example:

In "The animal didn't cross the road because it was too tired,"
attention helps the model know that "it" refers to "the animal", not "the road".

## 🧱 Key Components
Component	What it does
Self-Attention	Helps each word look at other words in the sentence
Positional Encoding	Adds info about word order (since Transformers don't have sequence memory)
Feedforward Layers	Processes each word vector independently
Layer Norm & Residuals	Help stabilize and improve learning

✅ Summary You Can Use:
Transformers are deep learning models that understand or generate text using attention. The encoder reads and understands the input. The decoder writes or predicts the output. They're fast, powerful, and used in models like BERT and GPT.

