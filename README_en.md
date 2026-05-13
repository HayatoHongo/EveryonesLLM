# **Everyones_nanoGPT Fill-in-the-Blank Notebook Tutorial**

![WebUI.png](assets/WebUI.png)

### [Webアプリで進めてみよう！](https://everyonesai-v2.created.app/)

This is a complete guide for anyone who thinks, "I love ChatGPT!" or "I want to build one myself!"<br>
You type "Hello!", and it replies, "How can I help you today?"<br>
And when you learn that this is actually powered by plain addition, multiplication, and a little stack of nonlinear functions,<br>
you may get so excited that you cannot sleep at night.<br>
Welcome to the world of deep learning. There is no going back now.<br>
I wrote this guide little by little on my way to school, packed into a tiny seat on the Namboku Line every day.<br>
Whenever I receive comments from students saying, "I did it!",<br>
I feel that all those hours in that small seat really meant something.

---

![ColabGPT_demo.gif](assets/ColabGPT_demo.gif)

Now, let us build a GPT model together! 😎  
In this tutorial, you will find friendly explanations and **100+ fill-in-the-blank questions 🫨**.  
If you have ever thought, "I kind of want to build an LLM," this is the kind of tutorial that can seriously level you up.  
With the right background knowledge, you can finish it in 28-42 hours!  
Everything runs on Google Colab.  
This tutorial is based on [Andrej Karpathy's nanoGPT](https://colab.research.google.com/drive/1JMLa53HDuA-i7ZBmqV7ZnA3c_fvtXnx-?usp=sharing) and [jingyaogong's Minimind](https://github.com/jingyaogong/minimind.git).  
I want to say a huge and heartfelt thank you to both of them.

---

## Table of Contents

### Basic Knowledge (Warm-up)

If you have never implemented an MLP or VAE before 😥... do not worry!<br>
This warm-up is a bit of work, but once you finish it, you will be ready to go.<br>
If you have already implemented them before, feel free to start from the main part.

| Chapter | Estimated Time | Notebook |
|---|---|---|
| Chapter 01: MNIST MLP 1        | 2-3 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_DeepLearning_colab_Chapter01_todo_en.ipynb) |
| Chapter 02:  MNIST MLP 2    | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_DeepLearning_colab_Chapter02_todo_en.ipynb) |
| Chapter 03:  cVAE | 2-3 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_DeepLearning_colab_Chapter03_todo_en.ipynb) |


### ColabGPT

| Chapter | Estimated Time | Notebook |
|---|---|---|
| Chapter 00: Start Tutorial      | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter00_todo_en.ipynb) |
| Chapter 01: Dataloader         | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter01_todo_en.ipynb) |
| Chapter 02: TokenEmbedding     | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter02_todo_en.ipynb) |
| Chapter 03: PositionEmbedding  | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter03_todo_en.ipynb) |
| Chapter 04: EmbeddingModule    | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter04_todo_en.ipynb) |
| Chapter 05: LayerNorm          | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter05_todo_en.ipynb) |
| Chapter 06: AttentionHead      | 3-4 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter06_todo_en.ipynb) |
| Chapter 07: MultiHeadAttention | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter07_todo_en.ipynb) |
| Chapter 08: FeedForward        | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter08_todo_en.ipynb) |
| Chapter 09: TransformerBlock   | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter09_todo_en.ipynb) |
| Chapter 10: VocabularyLogits   | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter10_todo_en.ipynb) |
| Chapter 11: nanoGPT| 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter11_todo_en.ipynb) |
| Chapter 12: Trainer            | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter12_todo_en.ipynb) |
| Chapter 13: Tokens per second(CPU)    | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter13_todo_en.ipynb) |          |
| Chapter 14: Tokens per second(T4 GPU)     | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter14_todo_en.ipynb) |          |
| Chapter 15: Train nanoGPT with GPU    | 0.5-1 hour    | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter15_todo_en.ipynb) |          |
| Chapter 16: Make only the model size bigger          | 0.5-1 hour (+ 1 hour model training)  | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter16_todo_en.ipynb) |          |
| Chapter 17:  Make the dataset bigger    | 1-2 hours (+ 1 hour model training) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter17_todo_en.ipynb) |          |
| Chapter 18: tiktoken      | 1-2 hours (+ 1 hour model training)   | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter18_todo_en.ipynb) |          |
| Chapter 19: Long Train    | 1-2 hours (+ **6 hours** model training)  | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter19_todo_en.ipynb) |          |
| Chapter 20: Learning rate            | 0.5-1 hour   | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter20_todo_en.ipynb) |          |
| Chapter 21: Scaling Law       | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter21_todo_en.ipynb) |          |
| Chapter 22: TinyStories(Main) | 1-2 hours   | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter22_main_todo_en.ipynb) |          |
| Chapter 22: TinyStories(Model Training) | 1 hour   | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter22_train_todo_en.ipynb) |          |
| Chapter 23: RPE(OverSimplified) | 2-3 hours   | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter23_todo_en.ipynb) |          |
| Chapter 24: RPE(Simplified)        | 1-2 hours (+ 1 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter24_todo_en.ipynb) |
| Chapter 25: LR schedule      | 1 hour      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter25_todo_en.ipynb) |
| Chapter 26: Checkpoint      | 1 hour      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter26_todo_en.ipynb) |
| Chapter 27: Pretraining        | 0.5 hour (+ **20 hours** model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter27_todo_en.ipynb) |
| Chapter 28: Instruction Tuning        | 0.5 hour (+ 0.5 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/todo/Everyones_nanoGPT_colab_Chapter28_todo_en.ipynb) |



## **Demo Output Example**
![nanoGPT_demo_output](assets/v2_Everyones_nanoGPT_demo_output.png)

Chapter28...!

![ColabGPT_demo.gif](assets/ColabGPT_demo.gif)

---

## **Tensor Map (Full Tensor Overview)**
**Try making the tensor map below by yourself!**  
Do not worry, I prepared lots of hints for you.  
[View the full-resolution Tensor Map of the nanoGPT model on Canva](https://www.canva.com/design/DAGskS8QP6k/1zs7IklaMrB_LncHn2I8pA/edit?utm_content=DAGskS8QP6k&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

![Everyones TensorMap](assets/Everyones_nanoGPT_TensorMap_answer.png)

---

## **Prerequisite Knowledge and Skills**

**Things I want you to understand**  
- Matrix multiplication and addition  
- Mean and variance  
- ResNet residual connections  
- How Word2Vector works  

---

## **About the Model**

In this tutorial, we use an ultra-simple "bigram model" where 1 character = 1 token.  
The internal structure is also very simple.  
The training dataset is Shakespeare text. It is very old, so it is copyright-free.

Compared with the real GPT-2, this is extremely basic. But if your goal is to learn from the foundations and aim for the real thing, this is the best place to start.  
On a PC with 16GB of memory, just 2-4 minutes of CPU training is enough to generate text that feels a bit like Shakespeare!  
I think you will be moved!

---

## **About the Development Environment**

To keep setup easy, please try running all the samples on Google Colab.

However, Google Colab does not save checkmarks in checkboxes.  
If you want to track your progress, or if you want to work little by little, say every 30 minutes, I recommend VS Code.  
In that case, fork this repository and clone it to your own PC.


Python 3.12 & PyTorch 2.6.0 is the best setup, but most other versions should also work.  
Usually, the PyTorch you already have installed is fine!  
If something does not work, it is a good idea to create a virtual environment with `requirements.txt`.  
If you use Docker Desktop, the included `Dockerfile` and the Dev Container extension can give you an even more stable environment.

---

## **Answers**

| Chapter                                 | Estimated Time                   | Notebook                                                                                                                                                                                                                           |
| ------------------------------------- | ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chapter 00: Start Tutorial      | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter00_answer_en.ipynb) |
| Chapter 01: Dataloader         | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter01_answer_en.ipynb) |
| Chapter 02: TokenEmbedding     | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter02_answer_en.ipynb) |
| Chapter 03: PositionEmbedding  | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter03_answer_en.ipynb) |
| Chapter 04: EmbeddingModule    | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter04_answer_en.ipynb) |
| Chapter 05: LayerNorm          | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter05_answer_en.ipynb) |
| Chapter 06: AttentionHead      | 3-4 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter06_answer_en.ipynb) |
| Chapter 07: MultiHeadAttention | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter07_answer_en.ipynb) |
| Chapter 08: FeedForward        | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter08_answer_en.ipynb) |
| Chapter 09: TransformerBlock   | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter09_answer_en.ipynb) |
| Chapter 10: VocabularyLogits   | 0.5-1 hour | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter10_answer_en.ipynb) |
| Chapter 11: nanoGPT| 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter11_answer_en.ipynb) |
| Chapter 12: Trainer            | 1-2 hours | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter12_answer_en.ipynb) |
| Chapter 13: Tokens per second(CPU)    | 1-2 hours                    | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter13_answer_en.ipynb)       |
| Chapter 14: Tokens per second(T4 GPU) | 0.5-1 hour                  | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter14_answer_en.ipynb)       |
| Chapter 15: Train nanoGPT with GPU    | 0.5-1 hour                  | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter15_answer_en.ipynb)       |
| Chapter 16: Make only the model size bigger             | 0.5-1 hour (+ 1 hour model training) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter16_answer_en.ipynb)       |
| Chapter 17: Make the dataset bigger              | 1-2 hours (+ 1 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter17_answer_en.ipynb)       |
| Chapter 18: tiktoken                  | 1-2 hours (+ 1 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter18_answer_en.ipynb)       |
| Chapter 19: Long Train                | 1-2 hours (+ **6 hours** model training) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter19_answer_en.ipynb)       |
| Chapter 20: Learning rate                       | 0.5-1 hour                  | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter20_answer_en.ipynb)       |
| Chapter 21: Scaling Law               | 1-2 hours                    | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter21_answer_en.ipynb)       |
| Chapter 22: TinyStories(Main)          | 1-2 hours                    | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter22_main_answer_en.ipynb)  |
| Chapter 22: TinyStories(Model Training)        | 1 hour                      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter22_train_answer_en.ipynb) |
| Chapter 23: RPE(OverSimplified)        | 2-3 hours                     | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter23_answer_en.ipynb) |
| Chapter 24: RPE(Simplified)        | 1-2 hours (+ 1 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter24_answer_en.ipynb) |
| Chapter 25: LR schedule        | 1 hour     | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter25_answer_en.ipynb) |
| Chapter 26: Checkpoint        | 1 hour     | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter26_answer_en.ipynb) |
| Chapter 27: Pretraining        | 0.5 hour (+ **20 hours** model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter27_answer_en.ipynb) |
| Chapter 28: Instruction Tuning        | 0.5 hour (+ 1 hour model training)      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Everyones_nanoGPT_colab_Chapter28_answer_en.ipynb) |


**Added Before Final Cleanup**

| Chapter                                 | Estimated Time                   | Notebook                                                                                                                                                                                                                           |
| ------------------------------------- | ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chapter 25: RoPE        |                      | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/RoPE_Everyones_nanoGPT_colab_Chapter25_answer_en.ipynb) |
| Chapter 26: Pretraining        |       | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Pretraining_Everyones_nanoGPT_colab_Chapter26_answer_en.ipynb) |
| Chapter 27: Instruction Tuning        |       | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/Instruction_Tuning_Everyones_nanoGPT_colab_Chapter27_answer_en.ipynb) |
| Chapter 28: Vision Pretraining        |       | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/ColabGPT/blob/ja/notebooks/answer/multimodal_Everyones_nanoGPT_colab_Chapter28_answer_en.ipynb) |



## **About Project EveryonesAI**

![EveryonesAI Logo](assets/EveryonesAI_logo.png)  
![EveryonesAI Goal](assets/EveryonesAI_goal.png)  
![EveryonesAI Idea](assets/EveryonesAI_idea.png)  
![EveryonesAI Prerequites](assets/EveryonesAI_prerequites.png)  
![EveryonesAI Plan](assets/EveryonesAI_plan.png)
