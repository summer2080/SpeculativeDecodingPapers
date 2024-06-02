<div align="center">
  <h2><img src="assets/logo.png" height="28px"/><i>Unlocking Efficiency in Large Language Model Inference:</i><br>A Comprehensive Survey of Speculative Decoding</h2> 
</div>

<div align="center">
<b>Heming Xia</b><sup>1</sup>,
<b>Zhe Yang</b><sup>2</sup>,
<b>Qingxiu Dong</b><sup>2</sup>,
<b>Peiyi Wang</b><sup>2</sup>,
<b>Yongqi Li</b><sup>1</sup>,
<b>Tao Ge</b><sup>3</sup>,
<b>Tianyu Liu</b><sup>4</sup>,
<b>Wenjie Li</b><sup>1</sup>,
<b>Zhifang Sui</b><sup>2</sup>
</div>

<div align="center">
<sup>1</sup>Department of Computing, The Hong Kong Polytechnic University
</div>
<div align="center">
<sup>2</sup>National Key Laboratory for Multimedia Information Processing, Peking University
</div>
<div align="center">
<sup>3</sup>Microsoft Research Asia <sup>4</sup>Alibaba Group
</div>

![timeline](./assets/timeline.png)

This repository contains a regularly updated paper list for **Speculative Decoding**.

[![Arxiv](https://img.shields.io/badge/Arxiv-2401.07851-orange.svg)](https://arxiv.org/abs/2401.07851) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](./LICENSE) ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/hemingkx/SpeculativeDecodingPapers/main?logo=github&color=blue)

## Content

- [Keywords Convention](#keywords-convention)
- [Papers](#papers)
  - [Survey](#survey)
  - [Speculative Decoding for Seq2Seq](#speculative-decoding-for-seq2seq)
  - [Speculative Decoding for LLMs](#speculative-decoding-for-llms)
  - [Multimodal Speculative Decoding](#multimodal-speculative-decoding)
  - [Long-Context Speculative Decoding](#long-context-speculative-decoding)
  - [Alignment](#alignment)
  - [Benchmarks](#benchmarks)
  - [Applications](#applications)
  - [Analysis](#analysis)
- [Blogs](#blog--project)
- [Contribution](#contribution)
  - [Contributors](#contributors)
  - [Contributing to this paper list](#contributing-to-this-paper-list)
- [Citation](#citation)

## Keywords Convention

![](https://img.shields.io/badge/SpecDec-blue) Abbreviation

![](https://img.shields.io/badge/ACL2022-orange) Conference

![](https://img.shields.io/badge/Drafter:_small_LM-green) Drafting Methods in Speculative Decoding

![](https://img.shields.io/badge/Batching-lightgray) Main Features

## Papers

### Survey

- **Unlocking Efficiency in Large Language Model Inference: A Comprehensive Survey of Speculative Decoding**  
  *Heming Xia, Zhe Yang, Qingxiu Dong, Peiyi Wang, Yongqi Li, Tao Ge, Tianyu Liu, Wenjie Li, Zhifang Sui.* [[pdf](https://arxiv.org/pdf/2401.07851.pdf)], [[code](https://github.com/hemingkx/SpeculativeDecodingPapers)], 2024.01. ![](https://img.shields.io/badge/ACL2024--findings-orange) ![](https://img.shields.io/badge/Survey_on_Speculative_Decoding-lightgray)
- **Beyond the Speculative Game: A Survey of Speculative Execution in Large Language Models**  
  *Chen Zhang, Zhuorui Liu, Dawei Song.* [[pdf](https://arxiv.org/pdf/2404.14897.pdf)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange)

### Speculative Decoding for Seq2Seq

- **Blockwise Parallel Decoding for Deep Autoregressive Models**  
  *Mitchell Stern, Noam Shazeer, Jakob Uszkoreit*. [[pdf](https://arxiv.org/pdf/1811.03115.pdf)], 2018.11. ![](https://img.shields.io/badge/NIPS2018-orange) ![](https://img.shields.io/badge/Self--Draft:_specialized_FFN_heads-green) ![](https://img.shields.io/badge/Blockwise_Decoding-blue)

- **Speculative Decoding: Exploiting Speculative Execution for Accelerating Seq2seq Generation**  
  *Heming Xia, Tao Ge, Peiyi Wang, Si-Qing Chen, Furu Wei, Zhifang Sui*. [[pdf](https://aclanthology.org/2023.findings-emnlp.257.pdf)], [[code](https://github.com/hemingkx/SpecDec)], 2022.03. ![](https://img.shields.io/badge/EMNLP2023--findings-orange) ![](https://img.shields.io/badge/Drafter:_specialized_Non--Auto_LM-green) ![](https://img.shields.io/badge/SpecDec-blue)

- **Speculative Decoding with Big Little Decoder**  
  *Sehoon Kim, Karttikeya Mangalam, Suhong Moon, John Canny, Jitendra Malik, Michael W. Mahoney, Amir Gholami, Kurt Keutzer*. [[pdf](https://openreview.net/pdf?id=EfMyf9MC3t)], [[code](https://github.com/kssteven418/BigLittleDecoder)], 2023.02. ![](https://img.shields.io/badge/NIPS2023-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/BiLD-blue)

- **Accelerating Transformer Inference for Translation via Parallel Decoding**  
  *Andrea Santilli, Silvio Severino, Emilian Postolache, Valentino Maiorca, Michele Mancusi, Riccardo Marin, Emanuele Rodolà*. [[pdf](https://aclanthology.org/2023.acl-long.689.pdf)], 2023.05. ![](https://img.shields.io/badge/ACL2023-orange) ![](https://img.shields.io/badge/Self--Draft:_mask--predict-green)
  
- **SPEED: Speculative Pipelined Execution for Efficient Decoding**  
  *Coleman Hooper, Sehoon Kim, Hiva Mohammadzadeh, Hasan Genc, Kurt Keutzer, Amir Gholami, Sophia Shao*. [[pdf](https://arxiv.org/pdf/2310.12072.pdf)], 2023.10. ![](https://img.shields.io/badge/ENLSP_at_NIPS2023-orange) ![](https://img.shields.io/badge/Self--Draft:_early--exiting-green) ![](https://img.shields.io/badge/SPEED-blue)
  
- **Fast and Robust Early-Exiting Framework for Autoregressive Language Models with Synchronized Parallel Decoding**  
  *Sangmin Bae, Jongwoo Ko, Hwanjun Song, Se-Young Yun*. [[pdf](https://aclanthology.org/2023.emnlp-main.362.pdf)], [[code](https://github.com/raymin0223/fast_robust_early_exit)], 2023.10. ![](https://img.shields.io/badge/EMNLP2023-orange) ![](https://img.shields.io/badge/Self--Draft:_early--exiting-green) ![](https://img.shields.io/badge/FREE-blue)

### Speculative Decoding for LLMs

- **Fast Inference from Transformers via Speculative Decoding**  
  *Yaniv Leviathan, Matan Kalman, Yossi Matias*. [[pdf](https://arxiv.org/pdf/2211.17192.pdf)], 2022.11. ![](https://img.shields.io/badge/ICML2023--Oral-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green)
- **Accelerating Large Language Model Decoding with Speculative Sampling**  
  *Charlie Chen, Sebastian Borgeaud, Geoffrey Irving, Jean-Baptiste Lespiau, Laurent Sifre, John Jumper*. [[pdf](http://arxiv.org/abs/2302.01318)], 2023.02. ![](https://img.shields.io/badge/Technical_Report-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/SpS-blue)
- **Inference with Reference: Lossless Acceleration of Large Language Models**  
  *Nan Yang, Tao Ge, Liang Wang, Binxing Jiao, Daxin Jiang, Linjun Yang, Rangan Majumder, Furu Wei.* [[pdf](https://arxiv.org/pdf/2304.04487.pdf)], 2023.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Draft:_the_reference-green) ![](https://img.shields.io/badge/LLMA-blue)
- **SpecInfer: Accelerating Generative LLM Serving with Speculative Inference and Token Tree Verification**  
  *Xupeng Miao, Gabriele Oliaro, Zhihao Zhang, Xinhao Cheng, Zeyu Wang, Rae Ying Yee Wong, Alan Zhu, Lijie Yang, Xiaoxiang Shi, Chunan Shi, Zhuoming Chen, Daiyaan Arfeen, Reyna Abhyankar, Zhihao Jia.* [[pdf](https://arxiv.org/pdf/2305.09781.pdf)], [[code](https://github.com/flexflow/FlexFlow/)], 2023.05. ![](https://img.shields.io/badge/ASPLOS2024-orange) ![](https://img.shields.io/badge/Drafter:_boost--tuned_small_LMs-green) ![](https://img.shields.io/badge/SpecInfer-blue)
- **Predictive Pipelined Decoding: A Compute-Latency Trade-off for Exact LLM Decoding**  
  *Seongjun Yang, Gibbeum Lee, Jaewoong Cho, Dimitris Papailiopoulos, Kangwook Lee*. [[pdf](https://arxiv.org/pdf/2307.05908.pdf)], 2023.08. ![](https://img.shields.io/badge/ES--FOMO_at_ICML2023-orange) ![](https://img.shields.io/badge/Self--Draft:_early--exiting-green) ![](https://img.shields.io/badge/PPD-blue)
- **Accelerating LLM Inference with Staged Speculative Decoding**  
  *Benjamin Spector, Chris Re*. [[pdf](https://arxiv.org/pdf/2308.04623.pdf)], 2023.08. ![](https://img.shields.io/badge/ES--FOMO_at_ICML2023-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green)
- **SpecTr: Fast Speculative Decoding via Optimal Transport**   
  *Ziteng Sun, Ananda Theertha Suresh, Jae Hun Ro, Ahmad Beirami, Himanshu Jain, Felix Yu, Michael Riley, Sanjiv Kumar*. [[pdf](https://openreview.net/pdf?id=d0mGsaheuT)], 2023.08. ![](https://img.shields.io/badge/ES--FOMO_at_ICML2023-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/SpecTr-blue)
- **Draft & Verify: Lossless Large Language Model Acceleration via Self-Speculative Decoding**  
  *Jun Zhang, Jue Wang, Huan Li, Lidan Shou, Ke Chen, Gang Chen, Sharad Mehrotra*. [[pdf](https://arxiv.org/pdf/2309.08168.pdf)], [[code](https://github.com/dilab-zju/self-speculative-decoding)], 2023.09. ![](https://img.shields.io/badge/ACL2024-orange) ![](https://img.shields.io/badge/Self--Draft:_layer--skipping-green) ![](https://img.shields.io/badge/Self--Speculative-blue)
- **Online Speculative Decoding**  
  *Xiaoxuan Liu, Lanxiang Hu, Peter Bailis, Ion Stoica, Zhijie Deng, Alvin Cheung, Hao Zhang*. [[pdf](https://arxiv.org/pdf/2310.07177.pdf)], 2023.10. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Online_Distillation_Strategy-lightgray)
- **DistillSpec: Improving Speculative Decoding via Knowledge Distillation**  
  *Yongchao Zhou, Kaifeng Lyu, Ankit Singh Rawat, Aditya Krishna Menon, Afshin Rostamizadeh, Sanjiv Kumar, Jean-François Kagy, Rishabh Agarwal.* [[pdf](https://arxiv.org/pdf/2310.08461.pdf)], 2023.10. ![](https://img.shields.io/badge/ICLR2024-orange) ![](https://img.shields.io/badge/Drafter:_distilled_small_LM-green) ![](https://img.shields.io/badge/DistillSpec-blue) ![](https://img.shields.io/badge/Distillation_Strategy-lightgray)
- **REST: Retrieval-Based Speculative Decoding**  
  *Zhenyu He, Zexuan Zhong, Tianle Cai, Jason D Lee, Di He.* [[pdf](https://arxiv.org/pdf/2311.08252.pdf)], [[code](https://github.com/FasterDecoding/REST)], 2023.11. ![](https://img.shields.io/badge/NAACL2024-orange) ![](https://img.shields.io/badge/Draft:_retrieved_Docs-green) ![](https://img.shields.io/badge/REST-blue)
- **Speculative Contrastive Decoding**  
  *Hongyi Yuan, Keming Lu, Fei Huang, Zheng Yuan, Chang Zhou.* [[pdf](https://arxiv.org/pdf/2311.08981.pdf)], 2023.11. ![](https://img.shields.io/badge/ACL2024-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/SCD-blue)
- **PaSS: Parallel Speculative Sampling**  
  *Giovanni Monea, Armand Joulin, Edouard Grave.* [[pdf](https://arxiv.org/pdf/2311.13581.pdf)], 2023.11. ![](https://img.shields.io/badge/ENLSP_at_NIPS2023-orange) ![](https://img.shields.io/badge/Self--Draft:_prompt--tuning-green) ![](https://img.shields.io/badge/PaSS-blue)
- **Cascade Speculative Drafting for Even Faster LLM Inference**  
  *Ziyi Chen, Xiaocong Yang, Jiacheng Lin, Chenkai Sun, Jie Huang, Kevin Chen-Chuan Chang.* [[pdf](https://arxiv.org/pdf/2312.11462.pdf)], [[code](https://github.com/lfsszd/CS-Drafting)], 2023.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_cascaded_LMs-green)
- **SLiM: Speculative Decoding with Hypothesis Reduction**  
  *Hongxia Jin, Chi-Heng Lin, Shikhar Tuli, James Seale Smith, Yen-Chang Hsu, Yilin Shen*. [[pdf](https://openreview.net/pdf?id=aPOFpNWwzl)], 2023.12. ![](https://img.shields.io/badge/NAACL2024--findings-orange) ![](https://img.shields.io/badge/Hypothesis_Reduction-lightgray) ![](https://img.shields.io/badge/SLiM-blue)
- **Graph-Structured Speculative Decoding**  
  *Zhuocheng Gong, Jiahao Liu, Ziyue Wang, Pengfei Wu, Jingang Wang, Xunliang Cai, Dongyan Zhao, Rui Yan*. [[pdf](https://openreview.net/pdf?id=KSq0Gwyl_sL)], 2023.12. ![](https://img.shields.io/badge/ACL2024-orange) ![](https://img.shields.io/badge/Token_Graph:_directed_acyclic_graph-lightgray) ![](https://img.shields.io/badge/GSD-blue)
- **Multi-Candidate Speculative Decoding**  
  *Sen Yang, Shujian Huang, Xinyu Dai, Jiajun Chen.* [[pdf](https://arxiv.org/pdf/2401.06706.pdf)], [[code](https://github.com/NJUNLP/MCSD)], 2024.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green)
- **Medusa: Simple LLM Inference Acceleration Framework with Multiple Decoding Heads**  
  *Tianle Cai, Yuhong Li, Zhengyang Geng, Hongwu Peng, Jason D. Lee, Deming Chen, Tri Dao.* [[pdf](https://arxiv.org/pdf/2401.10774.pdf)], [[code](https://github.com/FasterDecoding/Medusa)], 2024.01. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Self--Draft:_specialized_FFN_heads-green) ![](https://img.shields.io/badge/Medusa-blue)
- **BiTA: Bi-Directional Tuning for Lossless Acceleration in Large Language Models**  
  *Feng Lin, Hanling Yi, Hongbin Li, Yifan Yang, Xiaotian Yu, Guangming Lu, Rong Xiao*. [[pdf](https://arxiv.org/pdf/2401.12522.pdf)], [[code](https://github.com/linfeng93/BiTA)], 2024.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_prompt--tuning-green) ![](https://img.shields.io/badge/BiTA-blue)
- **EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty**  
  *Yuhui Li, Fangyun Wei, Chao Zhang, Hongyang Zhang*. [[pdf](https://arxiv.org/pdf/2401.15077.pdf)], [[code](https://github.com/SafeAILab/EAGLE)], 2024.01. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Self--Draft:_auto--regression_heads-green) ![](https://img.shields.io/badge/EAGLE-blue)
- **GliDe with a CaPE: A Low-Hassle Method to Accelerate Speculative Decoding**  
  *Cunxiao Du, Jing Jiang, Xu Yuanchen, Jiawei Wu, Sicheng Yu, Yongqi Li, Shenggui Li, Kai Xu, Liqiang Nie, Zhaopeng Tu, Yang You*. [[pdf](https://arxiv.org/pdf/2402.02082.pdf)], [[code](https://github.com/NonvolatileMemory/GliDe_with_a_CaPE_ICML_24)], 2024.02. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/GLIDE-blue)
- **Break the Sequential Dependency of LLM Inference Using Lookahead Decoding**  
  *Yichao Fu, Peter Bailis, Ion Stoica, Hao Zhang*. [[pdf](https://arxiv.org/pdf/2402.02057.pdf)], [[code](https://github.com/hao-ai-lab/LookaheadDecoding)], 2024.02. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Self--Draft:_mask--predict-green) ![](https://img.shields.io/badge/Lookahead-blue)
- **Hydra: Sequentially-Dependent Draft Heads for Medusa Decoding**  
  *Zachary Ankner, Rishab Parthasarathy, Aniruddha Nrusimha, Christopher Rinard, Jonathan Ragan-Kelley, William Brandon*. [[pdf](https://arxiv.org/pdf/2402.05109.pdf)], [[code](https://github.com/zankner/hydra)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_specialized_FFN_heads-green) ![](https://img.shields.io/badge/Hydra-blue)
- **Speculative Streaming: Fast LLM Inference without Auxiliary Models**  
  *Nikhil Bhendawade, Irina Belousova, Qichen Fu, Henry Mason, Mohammad Rastegari, Mahyar Najibi*. [[pdf](https://arxiv.org/pdf/2402.11131.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_multi--stream_attention-green) 
- **Generation Meets Verification: Accelerating Large Language Model Inference with Smart Parallel Auto-Correct Decoding**  
  *Hanling Yi, Feng Lin, Hongbin Li, Peiyang Ning, Xiaotian Yu, Rong Xiao*. [[pdf](https://arxiv.org/pdf/2402.11809.pdf)], 2024.02. ![](https://img.shields.io/badge/ACL2024--findings-orange) ![](https://img.shields.io/badge/Self--Draft:_semi--autoregressive_finetuning-green) ![](https://img.shields.io/badge/SPACE-blue)
- **Sequoia: Scalable, Robust, and Hardware-aware Speculative Decoding**  
  *Zhuoming Chen, Avner May, Ruslan Svirschevski, Yuhsun Huang, Max Ryabinin, Zhihao Jia, Beidi Chen*. [[pdf](https://arxiv.org/pdf/2402.12374.pdf)], [[code](https://github.com/Infini-AI-Lab/Sequoia)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Tree_Optimization-lightgray) ![](https://img.shields.io/badge/Sequoia-blue)
- **ProPD: Dynamic Token Tree Pruning and Generation for LLM Parallel Decoding**  
  *Shuzhang Zhong, Zebin Yang, Meng Li, Ruihao Gong, Runsheng Wang, Ru Huang*. [[pdf](https://arxiv.org/pdf/2402.13485.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Tree_Pruning_&_Generation-lightgray) ![](https://img.shields.io/badge/ProPD-blue)
- **Ouroboros: Speculative Decoding with Large Model Enhanced Drafting**  
  *Weilin Zhao, Yuxiang Huang, Xu Han, Chaojun Xiao, Zhiyuan Liu, Maosong Sun*. [[pdf](https://arxiv.org/pdf/2402.13720.pdf)], [[code](https://github.com/thunlp/Ouroboros)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Phrase_Candidate_Pool-lightgray) ![](https://img.shields.io/badge/Ouroboros-blue)
- **Recursive Speculative Decoding: Accelerating LLM Inference via Sampling Without Replacement**  
  *Wonseok Jeon, Mukul Gagrani, Raghavv Goel, Junyoung Park, Mingu Lee, Christopher Lott*. [[pdf](https://arxiv.org/pdf/2402.14160.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Diverse_Token_Tree-lightgray) ![](https://img.shields.io/badge/RSD-blue)
- **Chimera: A Lossless Decoding Method for Accelerating Large Language Models Inference by Fusing all Tokens**  
  *Ziqian Zeng, Jiahong Yu, Qianshi Pang, Zihao Wang, Huiping Zhuang, Cen Chen*. [[pdf](https://arxiv.org/pdf/2402.15758.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_lightweight_draft_model-green) ![](https://img.shields.io/badge/Chimera-blue)
- **Speculative Decoding via Early-exiting for Faster LLM Inference with Thompson Sampling Control Mechanism**  
  *Anonymous ACL submission*. [[pdf](https://openreview.net/pdf?id=B3qT4gVHwqY)], 2024.02. ![](https://img.shields.io/badge/ACL2024_submission-orange) ![](https://img.shields.io/badge/EESD-blue) 
- **Specuna: A Speculative Vicuna with Shallow Layer Reuse**  
  *Anonymous ACL submission*. [[pdf](https://openreview.net/pdf?id=D1iAiSaLOy)], 2024.02. ![](https://img.shields.io/badge/ACL2024_submission-orange) ![](https://img.shields.io/badge/Specuna-blue)
- **Parallel Decoding via Hidden Transfer for Lossless Large Language Model Acceleration**  
  *Anonymous ACL submission*. [[pdf](https://openreview.net/pdf?id=eExwTP0Fwv)], 2024.02. ![](https://img.shields.io/badge/ACL2024_submission-orange) ![](https://img.shields.io/badge/Hidden_Transfer-blue)
- **Minions: Accelerating Large Language Model Inference with Adaptive and Collective Speculative Decoding**  
  *Siqi Wang, Hailong Yang, Xuezhu Wang, Tongxuan Liu, Pengbo Wang, Xuning Liang, Kejie Ma, Tianyu Feng, Xin You, Yongjun Bao, Yi Liu, Zhongzhi Luan, Depei Qian*. [[pdf](https://arxiv.org/pdf/2402.15678.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Minions-blue)
- **CLLMs: Consistency Large Language Models**  
  *Siqi Kou, Lanxiang Hu, Zhezhi He, Zhijie Deng, Hao Zhang*. [[pdf](https://arxiv.org/pdf/2403.00835.pdf)], [[code](https://github.com/hao-ai-lab/Consistency_LLM)], [[blog](https://hao-ai-lab.github.io/blogs/cllm/)], 2024.03. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/Self--Draft:_training_with_jacobi_trajectories-green) ![](https://img.shields.io/badge/CLLM-blue)
- **Recurrent Drafter for Fast Speculative Decoding in Large Language Models**  
  *Aonan Zhang, Chong Wang, Yi Wang, Xuanyu Zhang, Yunfei Cheng*. [[pdf](https://arxiv.org/pdf/2403.09919.pdf)], 2024.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_recurrent_drafter-green) ![](https://img.shields.io/badge/ReDrafter-blue)
- **Optimal Block-Level Draft Verification for Accelerating Speculative Decoding**  
  *Ziteng Sun, Jae Hun Ro, Ahmad Beirami, Ananda Theertha Suresh*. [[pdf](https://arxiv.org/pdf/2403.10444.pdf)], 2024.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Block--Level_Draft_Verification-lightgray)
- **SDSAT: Accelerating LLM Inference through Speculative Decoding with Semantic Adaptive Tokens**  
  *Chengbo Liu, Yong Zhu*. [[pdf](https://arxiv.org/pdf/2403.18647.pdf)], 2024.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_semantic_adaptive_tokens-green) ![](https://img.shields.io/badge/SDSAT-blue)
- **Lossless Acceleration of Large Language Model via Adaptive N-gram Parallel Decoding**  
  *Jie Ou, Yueming Chen, Wenhong Tian*. [[pdf](https://arxiv.org/pdf/2404.08698.pdf)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_N--gram_model-green) ![](https://img.shields.io/badge/ANPD-blue)
- **Towards Fast Inference: Exploring and Improving Blockwise Parallel Drafts**  
  *Taehyeon Kim, Ananda Theertha Suresh, Kishore Papineni, Michael Riley, Sanjiv Kumar, Adrian Benton*. [[pdf](https://arxiv.org/pdf/2404.09221.pdf)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_specialized_FFN_heads-green)
- **Parallel Decoding via Hidden Transfer for Lossless Large Language Model Acceleration**  
  *Pengfei Wu, Jiahao Liu, Zhuocheng Gong, Qifan Wang, Jinpeng Li, Jingang Wang, Xunliang Cai, Dongyan Zhao*. [[pdf](https://arxiv.org/pdf/2404.12022.pdf)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_hidden_transfer-green)
- **BASS: Batched Attention-optimized Speculative Sampling**  
  *Haifeng Qian, Sujan Kumar Gonugondla, Sungsoo Ha, Mingyue Shang, Sanjay Krishna Gouda, Ramesh Nallapati, Sudipta Sengupta, Xiaofei Ma, Anoop Deoras*. [[pdf](https://arxiv.org/pdf/2404.15778.pdf)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/Batched_Speculative_Sampling-lightgray) ![](https://img.shields.io/badge/BASS-blue)
- **Layer Skip: Enabling Early Exit Inference and Self-Speculative Decoding**  
  *Mostafa Elhoushi, Akshat Shrivastava, Diana Liskovich, Basil Hosmer, Bram Wasti, Liangzhen Lai, Anas Mahmoud, Bilge Acun, Saurabh Agarwal, Ahmed Roman, Ahmed A Aly, Beidi Chen, Carole-Jean Wu*. [[pdf](https://arxiv.org/pdf/2404.16710)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_early--exiting-green) ![](https://img.shields.io/badge/Training_using_Layer_Dropout_&_Early_Exit_Loss-lightgray) ![](https://img.shields.io/badge/LayerSkip-blue)
- **Kangaroo: Lossless Self-Speculative Decoding via Double Early Exiting**  
  *Fangcheng Liu, Yehui Tang, Zhenhua Liu, Yunsheng Ni, Kai Han, Yunhe Wang*. [[pdf](https://arxiv.org/pdf/2404.18911)], [[code](https://github.com/Equationliu/Kangaroo)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_early--exiting_with_adapter-green) ![](https://img.shields.io/badge/Kangaroo-blue)
- **Accelerating Production LLMs with Combined Token/Embedding Speculators**  
  *Davis Wertheimer, Joshua Rosenkranz, Thomas Parnell, Sahil Suneja, Pavithra Ranganathan, Raghu Ganti, Mudhakar Srivatsa*. [[pdf](https://arxiv.org/pdf/2404.19124)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Speculator_Design_&_Training-lightgray)
- **Better & Faster Large Language Models via Multi-token Prediction**  
  *Fabian Gloeckle, Badr Youbi Idrissi, Baptiste Rozière, David Lopez-Paz, Gabriel Synnaeve*. [[pdf](https://arxiv.org/pdf/2404.19737)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_specialized_FFN_heads-green)
- **Clover: Regressive Lightweight Speculative Decoding with Sequential Knowledge**  
  *Bin Xiao, Chunan Shi, Xiaonan Nie, Fan Yang, Xiangwei Deng, Lei Su, Weipeng Chen, Bin Cui*. [[pdf](https://arxiv.org/pdf/2405.00263)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_auto--regressive_attention_block-green) ![](https://img.shields.io/badge/Clover-blue)
- **Accelerating Speculative Decoding using Dynamic Speculation Length**  
  *Jonathan Mamou, Oren Pereg, Daniel Korat, Moshe Berchansky, Nadav Timor, Moshe Wasserblat, Roy Schwartz*. [[pdf](https://arxiv.org/pdf/2405.04304)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DISCO-blue)
- **EMS-SD: Efficient Multi-sample Speculative Decoding for Accelerating Large Language Models**  
  *Yunsheng Ni, Chuanjian Liu, Yehui Tang, Kai Han, Yunhe Wang*. [[pdf](https://arxiv.org/pdf/2405.07542)], [[code](https://github.com/niyunsheng/EMS-SD)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Batched_Speculative_Decoding-lightgray) ![](https://img.shields.io/badge/EMS--SD-blue)
- **Nearest Neighbor Speculative Decoding for LLM Generation and Attribution**  
  *Minghan Li, Xilun Chen, Ari Holtzman, Beidi Chen, Jimmy Lin, Wen-tau Yih, Xi Victoria Lin*. [[pdf](https://arxiv.org/pdf/2405.19325)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Draft:_retrieved_Docs-green) ![](https://img.shields.io/badge/NEST-blue)
- **Hardware-Aware Parallel Prompt Decoding for Memory-Efficient Acceleration of LLM Inference**  
  *Hao (Mark)Chen, Wayne Luk, Ka Fai Cedric Yiu, Rui Li, Konstantin Mishchenko, Stylianos I. Venieris, Hongxiang Fan*. [[pdf](https://arxiv.org/pdf/2405.18628)], [[code](https://github.com/hmarkc/parallel-prompt-decoding)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_prompt--tuning-green) ![](https://img.shields.io/badge/PPD-blue)
- **Faster Cascades via Speculative Decoding**  
  *Harikrishna Narasimhan, Wittawat Jitkrittum, Ankit Singh Rawat, Seungyeon Kim, Neha Gupta, Aditya Krishna Menon, Sanjiv Kumar*. [[pdf](https://arxiv.org/pdf/2405.19261)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/SpecCascade-blue)
- **S3D: A Simple and Cost-Effective Self-Speculative Decoding Scheme for Low-Memory GPUs**  
  *Wei Zhong, Manasa Bharadwaj*. [[pdf](https://arxiv.org/pdf/2405.20314)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Draft:_layer--skipping_&_mask--predict-green) ![](https://img.shields.io/badge/S3D-blue)
- **SpecDec++: Boosting Speculative Decoding via Adaptive Candidate Lengths**  
  *Kaixuan Huang, Xudong Guo, Mengdi Wang*. [[pdf](https://arxiv.org/pdf/2405.19715)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Adaptive_Candidate_Lengths-lightgray) ![](https://img.shields.io/badge/SpecDec++-blue)

- **[ACL 2024] Self-Speculative Decoding**
  *Jun Zhang, Jue Wang, Huan Li, Lidan Shou, Ke Chen, Gang Chen, Sharad Mehrotra* [[pdf](https://arxiv.org/pdf/2309.08168)],[[code](https://github.com/dilab-zju/self-speculative-decoding)], 2024,05

### Multimodal Speculative Decoding

- **On Speculative Decoding for Multimodal Large Language Models**  
  *Mukul Gagrani, Raghavv Goel, Wonseok Jeon, Junyoung Park, Mingu Lee, Christopher Lott*. [[pdf](https://arxiv.org/pdf/2404.08856.pdf)], 2024.04. ![](https://img.shields.io/badge/ELVM_at_CVPR2024-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green)

### Long-Context Speculative Decoding

- **TriForce: Lossless Acceleration of Long Sequence Generation with Hierarchical Speculative Decoding**  
  *Hanshi Sun, Zhuoming Chen, Xinyu Yang, Yuandong Tian, Beidi Chen*. [[pdf](https://arxiv.org/pdf/2404.11912.pdf)], [[code](https://github.com/Infini-AI-Lab/TriForce)],2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_retrieval--based_drafting_&_hierarchical_speculation-green) ![](https://img.shields.io/badge/TriForce-blue)

### Alignment

- **Direct Alignment of Draft Model for Speculative Decoding with Chat-Fine-Tuned LLMs**  
  *Raghavv Goel, Mukul Gagrani, Wonseok Jeon, Junyoung Park, Mingu Lee, Christopher Lott.* [[pdf](https://arxiv.org/pdf/2403.00858.pdf)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter_Alignment-lightgray)

### Benchmarks

- **Spec-Bench: A Comprehensive Benchmark for Speculative Decoding**  
  *Heming Xia, Zhe Yang, Qingxiu Dong, Peiyi Wang, Yongqi Li, Tao Ge, Tianyu Liu, Wenjie Li, Zhifang Sui.* [[pdf](https://arxiv.org/pdf/2401.07851.pdf)], [[code](https://github.com/hemingkx/Spec-Bench)], [[blog](https://sites.google.com/view/spec-bench)], 2024.02. ![](https://img.shields.io/badge/ACL2024--findings-orange) ![](https://img.shields.io/badge/Spec--Bench-blue)

### Applications

- **Instantaneous Grammatical Error Correction with Shallow Aggressive Decoding**  
  *Xin Sun, Tao Ge, Furu Wei, Houfeng Wang*. [[pdf](https://aclanthology.org/2021.acl-long.462.pdf)], [[code](https://github.com/AutoTemp/Shallow-Aggressive-Decoding)], 2021.07. ![](https://img.shields.io/badge/ACL2021-orange) ![](https://img.shields.io/badge/Draft:_original_input-green) ![](https://img.shields.io/badge/SAD-blue)
- **LLMCad: Fast and Scalable On-device Large Language Model Inference**  
  *Daliang Xu, Wangsong Yin, Xin Jin, Ying Zhang, Shiyun Wei, Mengwei Xu, Xuanzhe Liu.* [[pdf](https://arxiv.org/pdf/2309.04255.pdf)], 2023.09. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LLMCad-blue)
- **Accelerating Retrieval-Augmented Language Model Serving with Speculation**  
  *Zhihao Zhang, Alan Zhu, Lijie Yang, Yihua Xu, Lanting Li, Phitchaya Mangpo Phothilimthana, Zhihao Jia.* [[pdf](https://arxiv.org/pdf/2401.14021.pdf)], 2023.10. ![](https://img.shields.io/badge/ICML2024-orange) ![](https://img.shields.io/badge/RaLMSpec-blue)
- **Lookahead: An Inference Acceleration Framework for Large Language Model with Lossless Generation Accuracy**  
  *Yao Zhao, Zhitian Xie, Chenyi Zhuang, Jinjie Gu.* [[pdf](https://arxiv.org/pdf/2312.12728.pdf)], [[code](https://github.com/alipay/PainlessInferenceAcceleration)], 2023.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Draft:_retrieved_Docs-green)
- **A Simple Framework to Accelerate Multilingual Language Model for Monolingual Text Generation**  
  *Jimin Hong, Gibbeum Lee, Jaewoong Cho.* [[pdf](https://arxiv.org/pdf/2401.10660.pdf)], 2024.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_specialized_FFN_heads-green) ![](https://img.shields.io/badge/MuMo-blue)![](https://img.shields.io/badge/Korean_&_Japanese-lightgray)
- **Accelerating Greedy Coordinate Gradient via Probe Sampling**  
  *Yiran Zhao, Wenyue Zheng, Tianle Cai, Xuan Long Do, Kenji Kawaguchi, Anirudh Goyal, Michael Shieh.* [[pdf](https://arxiv.org/pdf/2403.01251.pdf)], 2024.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter:_smaller_LM-green) ![](https://img.shields.io/badge/Greedy_Coordinate_Gradient-lightgray)

### Analysis

- **The Synergy of Speculative Decoding and Batching in Serving Large Language Models**  
  *Qidong Su, Christina Giannoula, Gennady Pekhimenko.* [[pdf](https://arxiv.org/pdf/2310.18813.pdf)], 2023.10. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Optimal_Speculation_Length_in_Batching-lightgray)
  
- **Decoding Speculative Decoding**  
  *Minghao Yan, Saurabh Agarwal, Shivaram Venkataraman.* [[pdf](https://arxiv.org/pdf/2402.01528.pdf)], [[code](https://github.com/uw-mad-dash/decoding-speculative-decoding)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Drafter_Selection_to_Maximize_Throughput-lightgray)
  
- **How Speculative Can Speculative Decoding Be?**  
  *Zhuorui Liu, Chen Zhang, Dawei Song.* [[pdf](https://aclanthology.org/2024.lrec-main.725.pdf)], [[code](https://github.com/ZhuoruiLiu12/SpecGame)], 2024.05. ![](https://img.shields.io/badge/COLING2024-orange) ![](https://img.shields.io/badge/Drafter_Scale_&_Draft_Length-lightgray)

## Blog & Project

**Assisted Generation: a new direction toward low-latency text generation.** Huggingface. 2023.05. [[Blog](https://huggingface.co/blog/assisted-generation)] [[Code](https://github.com/huggingface/transformers/blob/849367ccf741d8c58aa88ccfe1d52d8636eaf2b7/src/transformers/generation/utils.py#L4064)]

**Medusa: Simple Framework for Accelerating LLM Generation with Multiple Decoding Heads.** Princeton, UIUC. 2023.09. [[Blog](https://sites.google.com/view/medusa-llm)] [[Code](https://github.com/FasterDecoding/Medusa)]

**Break the Sequential Dependency of LLM Inference Using Lookahead Decoding.** LMSys. 2023.11. [[Blog](https://lmsys.org/blog/2023-11-21-lookahead-decoding/)] [[Code](https://github.com/hao-ai-lab/LookaheadDecoding)]

**Accelerating Generative AI with PyTorch II: GPT, Fast.** Pytorch. 2023.11. [[Blog](https://pytorch.org/blog/accelerating-generative-ai-2/)] [[Code](https://github.com/pytorch-labs/gpt-fast/blob/main/generate.py#L76)]

**Prompt Lookup Decoding.** Apoorv Saxena. 2023.11. [[Code](https://github.com/apoorvumang/prompt-lookup-decoding)] [[Colab](https://colab.research.google.com/drive/1ovjH1sg3lXWdm5Rx5EEukB9H_PFJVpJ4?usp=sharing)]

**REST: Retrieval-Based Speculative Decoding.** Peking University, Princeton University. 2023.11. [[Blog](https://sites.google.com/view/rest-llm/)] [[Code](https://github.com/FasterDecoding/REST)]

**EAGLE: Lossless Acceleration of LLM Decoding by Feature Extrapolation.** Vector Institute, University of Waterloo, Peking University. 2023.12. [[Blog](https://sites.google.com/view/eagle-llm)] [[Code](https://github.com/SafeAILab/EAGLE)]

**SEQUOIA: Serving exact Llama2-70B on an RTX4090 with half-second per token latency.** Carnegie Mellon University, Together AI, Yandex, Meta AI. 2024.02. [[Blog](https://infini-ai-lab.github.io/Sequoia-Page/)] [[Code](https://github.com/Infini-AI-Lab/Sequoia)]

## Contributors

<a href="https://github.com/hemingkx/SpeculativeDecodingPapers/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=hemingkx/SpeculativeDecodingPapers" />
</a>

## Contributing to this paper list

-  There are cases where we miss important works in this field, please feel free to contribute and promote your awesome work or other related works here! Thanks for the efforts in advance.

## Citation

If you find the resources in this repository useful, please cite our paper:

```
@misc{xia2024unlocking,
      title={Unlocking Efficiency in Large Language Model Inference: A Comprehensive Survey of Speculative Decoding}, 
      author={Heming Xia and Zhe Yang and Qingxiu Dong and Peiyi Wang and Yongqi Li and Tao Ge and Tianyu Liu and Wenjie Li and Zhifang Sui},
      year={2024},
      eprint={2401.07851},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

