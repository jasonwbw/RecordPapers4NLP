# Implementations

### Leadboard according to the papers and offincal implementations
Model | EM | F1 | code | paper |
:----:|:--:|:--:|:----:|:-----:|
Globally Normalized Reader | 66.6 | 75.0 | [Tensorflow](https://github.com/baidu-research/GloballyNormalizedReader) | [EMNLP17](https://www.aclweb.org/anthology/D17-1111) |
BiDAF | 68.0 | 77.3 | [Tensorflow](https://github.com/allenai/bi-att-flow) | [ICLR17](https://arxiv.org/abs/1611.01603) |
SEDT | 68.5 | 78.0 | | [EMNLP17](https://arxiv.org/pdf/1703.00572.pdf) |
ReasoNet | 69.1 | 78.9 | [CNTK](https://github.com/Microsoft/CNTK/tree/penhe/reasonet_tutorial/Examples/LanguageUnderstanding/ReasoNet) | [SIGKDD17](https://arxiv.org/pdf/1609.05284.pdf) |
RNET1 | 71.1 | 79.5 | | [ACL17](http://www.aclweb.org/anthology/P17-1018) |
Smartnet | 71.4 | 80.2 | | [arxiv-17](https://arxiv.org/pdf/1710.02772.pdf) |
RNET2 | 72.3 | 80.6 | | [MS share](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/05/r-net.pdf) |
BiDAF + selfatt | 72.1 | 81.1 | [Tensorflow](github.com/allenai/document-qa) | [arxiv-17](https://arxiv.org/pdf/1710.10723.pdf) |
MneReader | 71.8 | 81.2 | | [arxiv-17](https://arxiv.org/abs/1705.02798) |
PhaseCond | 72.1 | 81.4 | | [arxiv-17](https://arxiv.org/pdf/1710.10504.pdf) |
Document Reader | 73.6 | 82.7 | [Pytorch](https://github.com/facebookresearch/DrQA) | [ACL17](https://arxiv.org/pdf/1704.00051.pdf) |
MEMEN     | 75.4 | 82.7 | | [arxiv-17](https://arxiv.org/pdf/1707.09098.pdf) |
QANet     | 73.6 | 82.7 | | [ICLR18](https://openreview.net/pdf?id=B14TlG-RW)
FusionNet | 76.0 | 83.9 | [Pytorch](https://github.com/momohuang/FusionNet-NLI) | [ICLR18](https://arxiv.org/pdf/1711.07341.pdf) |
RaSoR + TR + LM | 77.6 | 84.2 | | [arxiv-17](https://arxiv.org/pdf/1712.03609.pdf) |

### None original Implementations (may without offical code)
Repository | RNET | MneReader | QANet | Document Reader | FusionNet |
-----------|:----:|:---------:|:-----:|:---------------:|:---------:|
ML Results in paper | 72.3/80.6 | 71.8/81.2 | 73.6/82.7 | 69.5/78.8 / 
[Pytorch](https://github.com/minsangkim142/QANet) | X | X | 70.0/79.4 | X | X | X |
[Pytorch](https://github.com/HKUST-KnowComp/MnemonicReader) | 70.2/79.2 | 72.3/81.4 | X | X | 69.4/78.6 | X |
[TF](https://github.com/HKUST-KnowComp/R-Net) | 71.1/79.5 | X | X | X | X | X |

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

### E2E Models for SQuAD and summrized contributions
- [SAN](https://arxiv.org/pdf/1712.03556.pdf)  
1.join hidden states of previous reasoning steps
- [FUSIONNET](https://arxiv.org/pdf/1711.07341.pdf)  
1.a fusion version of other networks
- [ELMo](https://openreview.net/pdf?id=S1p31z-Ab)  
1.pretrained word embedding by LM, which is somewhat similar with Tricks [Learned in Translation ...]
- [R-Net](https://www.microsoft.com/en-us/research/wp-content/uploads/2017/05/r-net.pdf)  
1.self att;  
2.soft att
- [Reinforced Mnemonic Reader](https://arxiv.org/abs/1705.02798)  
1.RL for F1;  
2.feature rich;  
3.memory answer pointer  
- [MEMEN](https://arxiv.org/abs/1707.09098)
- [ReasoNet](https://arxiv.org/abs/1609.05284)
- [SEDT](https://arxiv.org/abs/1703.00572)
- [BiDAF](https://arxiv.org/abs/1611.01603)  
1.(widely used) coopreation for question and contexts
- [BiDAF + self attention](https://arxiv.org/pdf/1710.10723.pdf)  
1.self attention with simplified BiDAF;  
2.new data;  
3.vairous comparision about diff functions
- [jNet](https://arxiv.org/abs/1703.04617)
- [Multi-Perspective Matching](https://arxiv.org/abs/1612.04211)
- [Dynamic Coattention Networks](https://arxiv.org/abs/1611.01604)
- [Document Reader](https://arxiv.org/abs/1704.00051)
- [FastQAExt](https://arxiv.org/abs/1703.04816)
- [RaSoR](https://arxiv.org/abs/1611.01436)
- [Fine-Grained Gating](https://arxiv.org/abs/1611.01724)
- [Dynamic Chunk Reader](https://arxiv.org/abs/1610.09996)
- [Conductor-net](https://arxiv.org/pdf/1710.10504.pdf)
- [RaSoR + TR + LM](https://arxiv.org/pdf/1712.03609.pdf)  
(have report results on adversarial SQuAD)
- [Smartnet](https://arxiv.org/pdf/1710.02772.pdf)
- [Globally Normalized Reader](https://www.aclweb.org/anthology/D17-1111)
1.A three step model non E2E (sentence selection, begin pred, end pred)

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
