# Text-Generator-using-Transformers
# Overview
In this example, we will use KerasNLP to build a scaled down generative model using a Transformer Decoder. A generative model allows you to generate sophisticated text from a prompt. In this lab, we will be building a model that only uses the decoder from the Transformer stack. At each stage, for a given word the attention layers can only access the words positioned before it in the sentence. These models are often called auto-regressive models. Some examples of decoder-only models are Transformer XL, GPT-2, CTRL, etc.

We will train the model on the simplebooks-92 corpus,which is a dataset made from several novels. This dataset was created from 1,573 Gutenberg books. It is a good dataset for this example since it has a small vocabulary and high word frequency, which is beneficial when training a generative model with few parameters.

This notebook demonstrates how to use KerasNLP tokenization, layers and metrics to simplify the training process, and then show how to generate output text using the KerasNLP sampling utilities.

# Learning Objectives

-Learn how to train a prepare a dataset for generative models using wordpiece tokenizer

-Learn how to use Keras NLP to build a generative model

-Learn different inference techniques to output text from a prompt
