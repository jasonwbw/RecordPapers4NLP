# Refs

## Dataset
- [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) / most popular, EMNLP best resource paper
- [MARCO](http://www.msmarco.org/)
- [NewsQA](https://datasets.maluuba.com/NewsQA)
- [Quasar](https://github.com/bdhingra/quasar)
- [RACE](http://www.cs.cmu.edu/~glai1/data/race/)
- [CNN/Daily Mail](https://github.com/deepmind/rc-data/)
- [DuReader](https://arxiv.org/pdf/1711.05073.pdf) / multi document for CQA
- [SQuAD: Adversarial Examples](https://arxiv.org/pdf/1707.07328.pdf)

## Leadboards
- [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/)
- [MARCO](http://www.msmarco.org/leaders.aspx)
- [DuReader](http://ai.baidu.com/broad/leaderboard?dataset=dureader)

## Reference

### E2E Models for SQuAD
- [SAN](https://arxiv.org/pdf/1712.03556.pdf)  
1.join hidden states of previous reasoning steps
- [FUSIONNET](https://arxiv.org/pdf/1711.07341.pdf) / [code](https://github.com/momohuang/FusionNet-NLI)  
a fusion version of other networks
- [ELMo](https://openreview.net/pdf?id=S1p31z-Ab)  
pretrained word embedding by LM, which is somewhat similar with Tricks [Learned in Translation ...]
- [R-Net](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/05/r-net.pdf) / [reproduce code](https://github.com/HKUST-KnowComp/R-Net)  
1.self att;  
2.soft att
- [Reinforced Mnemonic Reader](https://arxiv.org/abs/1705.02798)  
1.RL for F1;  
2.feature rich;  
3.memory answer pointer  
- [MEMEN](https://arxiv.org/abs/1707.09098)
- [ReasoNet](https://arxiv.org/abs/1609.05284)
- [SEDT](https://arxiv.org/abs/1703.00572)
- [BiDAF](https://arxiv.org/abs/1611.01603) / [code](https://github.com/allenai/bi-att-flow)  
1.(widely used) coopreation for question and contexts
- [BiDAF + self attention](https://arxiv.org/pdf/1710.10723.pdf)  
1.self attention with simplified BiDAF; 2.new data; 3.vairous comparision about diff functions
- [jNet](https://arxiv.org/abs/1703.04617)
- [Multi-Perspective Matching](https://arxiv.org/abs/1612.04211)
- [Dynamic Coattention Networks](https://arxiv.org/abs/1611.01604)
- [Document Reader](https://arxiv.org/abs/1704.00051)
- [FastQAExt](https://arxiv.org/abs/1703.04816)
- [RaSoR](https://arxiv.org/abs/1611.01436)
- [Fine-Grained Gating](https://arxiv.org/abs/1611.01724)
- [Dynamic Chunk Reader](https://arxiv.org/abs/1610.09996)
- [Conductor-net](https://arxiv.org/pdf/1710.10504.pdf)
- [RaSoR + TR + LM](https://arxiv.org/pdf/1710.10504.pdf)  
(have report results on adversarial SQuAD)
- [Smartnet](https://arxiv.org/pdf/1710.02772.pdf)

### Non-E2E Models
- [Globally Normalized Reader](http://aclweb.org/anthology/D17-1111) / [code](https://github.com/baidu-research/GloballyNormalizedReader)  
1.Three stage model include sentence selection, start prediction, end prediction  
2.Data augmentation (as the model runs faster, the authors replace the NEs to generate more data)


### Models for others dataset
- [Towards Human-level Machine Reading Comprehension: Reasoning and Inference with Multiple Strategies](https://arxiv.org/pdf/1711.04964.pdf)  
datasets: RACE  
multi step reasoning by update a Memory

### Tricks
- [A Comparative Study of Word Embeddings for Reading Comprehension](https://arxiv.org/pdf/1703.00993.pdf)
- [Learned in Translation: Contextualized Word Vectors](https://einstein.ai/static/images/layouts/research/cove/McCann2017LearnedIT.pdf)
- [R3 : Reinforced Reader-Ranker for Open-Domain Question Answering](https://arxiv.org/pdf/1709.00023.pdf)

### Generation
- [Learning to Ask: Neural Question Generation for Reading Comprehension](http://aclweb.org/anthology/P/P17/P17-1123.pdf)
- [S-Net](https://arxiv.org/pdf/1706.04815.pdf)

### Slot-filling
- [Zero-Shot Relation Extraction via Reading Comprehension](https://arxiv.org/pdf/1706.04115.pdf)
