# Attention
- What does Attention in Neural Machine Translation Pay Attention to? [paper](https://arxiv.org/pdf/1710.03348.pdf)  
Some interesting findings, and more details in the paper:  
~ only 54% attention to alignment points, which NUM 73%, NOUN 68%, VERB just 49%, and PRT(Particle, such as ’s, off, up) just 36%.  
~ Attention acc on alignments are high for NOUN, and very low for the VERB, but their target losses are about the same.


# Tricks
- REGULARIZING NEURAL NETWORKS BY PENALIZING CONFIDENT OUTPUT DISTRIBUTIONS [paper](https://arxiv.org/pdf/1701.06548.pdf)  
1.Label smoothing;  
2.Confidence penalty  


# Overfitting
- R-Drop: Regularized Dropout for Neural Networks [paper](https://arxiv.org/pdf/2106.14448.pdf)
add KL divergence between the results from two times of dropout
