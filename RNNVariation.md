# Accelerate
- Learning to Skim Text [paper appeared in ACL17](https://arxiv.org/pdf/1704.06877.pdf)  
Read text by skip some words.  
~ use the RL to learn the best skip stragegy for the target, that   
Action : jump  
Sampling: based on the jump softmax  
Reward: prediction is correct or not  
~ set the maxinum word to skip and jumps times, as well as pre-read content without jump.  
~ speed up about 2.x times for the short text