# Transformers from Scratch: BERT & GPT-2 in PyTorch 🤖

Want to truly understand how LLMs work? The best way is to **build them from scratch**. This repository documents my hands-on journey implementing **BERT** and **GPT-2** in PyTorch. ✨

Driven by curiosity, I break down each component step by step——from data preprocessing to model architecture——to reveal the mechanism behind these models. No magic, just elegant engineering. This project is for me——and for anyone seeking a deep, practical understanding of LLMs. 🔍   
</br>

***Note**: Modern LLMs often have billions to trillions of parameters. The BERT_base and GPT-2 small models built in this project are much smaller, but they share the same **core transformer architecture** that underpins today’s large-scale models.* 🔑  
***  

### Repository Structure 📂

The project is organized into three Jupyter notebooks:

`1. Data for BERT.ipynb`  
Processes the data for BERT’s training objectives: 
* **Masked Language Modeling (MLM)**: randomly masks tokens for prediction.
* **Next Sentence Prediction (NSP)**: constructs paired sentences (positive and negative examples).

`2. Reproducing BERT Model from Scratch using PyTorch.ipynb`  
Implements the BERT-base architecture step-by-step:
* **Dataset preparation**:  load processed data into a PyTorch `Dataset`, and wrap it in a `DataLoader`.
* **Model Implementation**: outline the BERT architecture and implement the BERT_base configuration.
* **Training**: train the model for one epoch and report the training and test loss to verify the end-to-end implementation.

`3. Rebuilding GPT-2 Model from Scratch with PyTorch.ipynb`   
Builds the GPT-2 Small model:
* **Dataset preparation**: preprocess the IMDb dataset for language modeling.
* **Model architecture**: outline the GPT-2 architecture and implement the GPT-2 Small configuration.
* **Training and generation**: train the model for 1000 steps, and generate a short piece of text to demonstrate functionality.📝

*** 

### Project Goals 🎯
* Gain a deep understanding of transformer-based models by implementing them from scratch.
* Explore how data is prepared for masked language modeling and next sentence prediction.
* Learn the internals of Transformer blocks that power modern NLP models.

***

### References 📚
* Vaswani, Ashish, et al. "[Attention is all you need.](https://arxiv.org/abs/1706.03762)" Advances in neural information processing systems 30 (2017). 
* Devlin, Jacob, et al. "[Bert: Pre-training of deep bidirectional transformers for language understanding.](https://arxiv.org/abs/1810.04805)" Proceedings of the 2019 conference of the North American chapter of the association for computational linguistics: human language technologies, volume 1 (long and short papers). 2019. 
* Radford, Alec, et al. "[Improving language understanding by generative pre-training.](https://www.mikecaptain.com/resources/pdf/GPT-1.pdf)" (2018): 3.
* Radford, Alec, et al. "[Language models are unsupervised multitask learners.](https://storage.prod.researchhub.com/uploads/papers/2020/06/01/language-models.pdf)" OpenAI blog 1.8 (2019): 9.
* Adrian Tam. [Linear Layers and Activation Functions in Transformer Models.](https://machinelearningmastery.com/linear-layers-and-activation-functions-in-transformer-models/) 2025

*** 

### License ⚖️ 
This project is licensed under the MIT License.
