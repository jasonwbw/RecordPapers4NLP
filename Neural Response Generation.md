# NRG (Neural Response Generation)

- A Neural Conversational Mode [ICLR15](https://arxiv.org/pdf/1506.05869v1.pdf)  
origin paper
- Neural Responding Machine for Short-Text Conversation [ACL15](https://arxiv.org/pdf/1503.02364.pdf)

## Data
- A Survey of Available Corpora for Building Data-Driven Dialogue Systems
- Improved Deep Learning Baselines for Ubuntu Corpus Dialogs
- LSDSCC: A Large Scale Domain-Specific Conversational Corpus for Response Generation with Diversity Oriented Evaluation Metrics [NAACL18](http://www.aclweb.org/anthology/N18-1188)

## Metric
- How NOT to evaluate your dialogue system: An empirical study of unsupervised evaluation metrics for dialogue response generation
- Towards an automatic turing test: Learning to evaluate dialogue responses.
- RUBER: An Unsupervised Method for Automatic Evaluation of Open-Domain Dialog Systems

## Model

### With knowledge
- Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory [paper](https://arxiv.org/pdf/1704.01074.pdf)
- Topic Aware Neural Response Generation [AAAI16](https://arxiv.org/pdf/1606.08340.pdf)

### Diversity
#### Inference
- A Diversity-Promoting Objective Function for Neural Conversation Models [NAACL16](https://arxiv.org/pdf/1510.03055v2.pdf)
- Generating Long and Diverse Responses with Neural Conversation Models
- A Simple, Fast Diverse Decoding Algorithm for Neural Generation

#### Model
- Sequence to Backward and Forward Sequences: A Content-Introducing Approach to Generative Short-Text Conversation [COLING16](https://arxiv.org/pdf/1607.00970.pdf)
- Learning to Decode for Future Success
- A Prospective-Performance Network to Alleviate Myopia in Beam Search for Response Generation [COLING18](http://www.aclweb.org/anthology/C18-1306)  
1.predict larger beam search by a smaller one which promote the diversity a lot
- Neural Response Generation with Dynamic Vocabularies [AAAI18](https://arxiv.org/pdf/1711.11191.pdf)
- Towards Less Generic Responses in Neural Conversation Models: A Statistical Re-weighting Method [EMNLP18](https://ai.tencent.com/ailab/nlp/papers/emnlp2018_conversation.pdf)  
1.reweight by punish universal replies and short/long replies  
2.use tfidf similar responses to compute the coverage of a response (UR)

#### Latent
- (VHRED) A Hierarchical Latent Variable Encoder-Decoder Model for Generating Dialogues
- A Conditional Variational Framework for Dialog Generation [ACL17](http://www.aclweb.org/anthology/P17-2080)
- (CVAE) Learning Discourse-level Diversity for Neural Dialog Models using Conditional Variational Autoencoders [ACL17](http://www.aclweb.org/anthology/P17-1061) / [code and data](https://github.com/snakeztc/NeuralDialog-CVAE)
- Variational Autoregressive Decoder for Neural Response Generation [EMNLP18](http://www.aclweb.org/anthology/D18-1354)  
1.increase the number of latent z from one to many;  
2.involving SBOW(predict future words in the sequence) auxiliary to training z.
- Improving Variational Encoder-Decoders in Dialogue Generation [AAAI18](https://arxiv.org/pdf/1802.02032.pdf)  
1.add a auto-encoder stagey (DAE) coo-work with CVAE stagey like GAN (to learn a good posterior), feed x->z' and sample z with using z' to stand x in a CVAE model;  
2.use a VAE/ecoder VAE/scheduled sampling to let the model consider more about the latent variable.
- Topic-Guided Variational Autoencoders for Text Generation [arxiv](https://arxiv.org/pdf/1903.07137.pdf)  

### Beam Search Optimization 
- Sequence-to-Sequence Learning as Beam-Search Optimization
- Scheduled Sampling for Sequence Prediction with Recurrent Neural Networks

### RL
- A Deep Reinforcement Learning Chatbot [paper](https://arxiv.org/pdf/1709.02349.pdf)
- Deep Reinforcement Learning for Dialogue Generation [ACL16](https://arxiv.org/pdf/1606.01541.pdf)

### GAN
- Neural Response Generation via GAN with an Approximate Embedding Layer [EMNLP17](http://www.aclweb.org/anthology/D/D17/D17-1066.pdf)  
Approximate (weighted averaged embedding by softmax) Embedding to solve the dispersion.

### Persona
- A Persona-Based Neural Conversation Model [ACL16](https://arxiv.org/pdf/1603.06155.pdf)
- Learning Personas from Dialogue with Attentive Memory Networks [EMNLP18](https://arxiv.org/pdf/1810.08717.pdf)
- Exploring Personalized Neural Conversational Models [ICJAI17](http://www.xiaoyumu.com/s/PDF/IJCAI_2017.pdf)
- Content-Oriented User Modeling for Personalized Response Ranking in Chatbots [TASLP](https://dl.acm.org/citation.cfm?id=3180729)
- Assigning Personality/Profile to a Chatting Machine for Coherent Conversation Generation [IJCAI18](https://www.ijcai.org/proceedings/2018/0595.pdf)  
1.involve profile into NRG (attention)
- Steering Output Style and Topic in Neural Response Generation [EMNLP17](https://www.aclweb.org/anthology/D17-1228)
- Personalizing Dialogue Agents: I have a dog, do you have pets too? [ACL18](http://aclweb.org/anthology/P18-1205) / [code & data](https://github.com/facebookresearch/ParlAI/tree/master/projects/personachat)
