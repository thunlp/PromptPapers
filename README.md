# PromptPapers


![](https://img.shields.io/github/last-commit/thunlp/PromptPapers?color=green) ![](https://img.shields.io/badge/PaperNumber-65-brightgreen) ![](https://img.shields.io/badge/PRs-Welcome-red) 

We have released an open-source prompt-learning toolkit, check out **[OpenPrompt](https://github.com/thunlp/OpenPrompt)!**

We strongly encourage the researchers that want to promote their fantastic work to the community to make **pull request** to update their paper's information! (See [contributing details](#contribution))

Effective adaptation of pre-trained models could be probed from different perspectives. Prompt-learning more focuses on the organization of training procedure and the unification of different tasks, while delta tuning (parameter efficient methods) provides another direction from the specific optimization of pre-trained models. Check [DeltaPapers](https://github.com/thunlp/DeltaPapers)!

<!-- omit in toc -->
## Contents

Must-read papers on prompt-based tuning for pre-trained language models. The paper list is mainly mantained by [Ning Ding](https://github.com/ningding97) and [Shengding Hu](https://github.com/shengdinghu). Watch this repository for the latest updates!

- [PromptPapers](#promptpapers)
  - [Introduction](#introduction)
    - [Keywords Convention](#keywords-convention)
  - [Papers](#papers)
    - [Overview](#overview)
    - [Pilot Work](#pilot-work)
    - [Basics](#basics)
    - [Analysis](#analysis)
    - [Improvements](#improvements)
    - [Specializations](#specializations)
  - [Contribution](#contribution)
    - [Other contributors](#other-contributors)
    - [Contributing to this paper list](#contributing-to-this-paper-list)




## Introduction

This is a paper list about **prompt-based tuning** for large-scale pre-trained language models. Different from traditional fine-tuning that uses an explicit classifier, prompt-based tuning directly uses the pre-trained models to conduct the pre-training tasks for classification or regression. 

### Keywords Convention

![](https://img.shields.io/badge/T5-blue) The abbreviation of the work.

![](https://img.shields.io/badge/Continuous_Template-red) The key features in terms of prompt learning used in the work.

![](https://img.shields.io/badge/Generation-brown) The mainly explored task of the work.

![](https://img.shields.io/badge/Analysis-green) The mainly explored property of prompt learning methods in the work.


## Papers



### Overview
This section contains the papers that overview the general trends in recent natural language processing with big (pretrained) models. 

1. **OpenPrompt: An Open-source Framework for Prompt-learning.** Preprint.
   
   *Ning Ding, Shengding Hu, Weilin Zhao, Yulin Chen, Zhiyuan Liu, Hai-Tao Zheng, Maoson Sun*  [[pdf](https://arxiv.org/pdf/2111.01998.pdf)] [[project](https://github.com/thunlp/OpenPrompt)], 2021.11

2. **Pre-Trained Models: Past, Present and Future.** Preprint.

   *Xu Han, Zhengyan Zhang, Ning Ding, Yuxian Gu, Xiao Liu, Yuqi Huo, Jiezhong Qiu, Yuan Yao, Ao Zhang, Liang Zhang, Wentao Han, Minlie Huang, Qin Jin, Yanyan Lan, Yang Liu, Zhiyuan Liu, Zhiwu Lu, Xipeng Qiu, Ruihua Song, Jie Tang, Ji-Rong Wen, Jinhui Yuan, Wayne Xin Zhao, Jun Zhu.* [[pdf](https://arxiv.org/abs/2106.07139)], 2021.6

3. **Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing.**  Preprint.

   *Liu, Pengfei, Weizhe Yuan, Jinlan Fu, Zhengbao Jiang, Hiroaki Hayashi, and Graham Neubig.*  [[pdf](https://arxiv.org/abs/2107.13586)] [[project](http://pretrain.nlpedia.ai)], 2021.7

4. **Paradigm Shift in Natural Language Processing.** Machine Intelligence Research.
   
   *Tianxiang Sun, Xiangyang Liu, Xipeng Qiu, Xuanjing Huang* [[pdf](https://arxiv.org/abs/2109.12575)] [[project](https://txsun1997.github.io/nlp-paradigm-shift/)], 2021.9



### Pilot Work
This section contains the pilot works that might contributes to the prevalence of prompt learning paradigm.
1. **Parameter-Efficient Transfer Learning for NLP.** ICML 2019. ![](https://img.shields.io/badge/Adapter-blue) 

   *Neil Houlsby, Andrei Giurgiu, Stanislaw Jastrzebski, Bruna Morrone, Quentin de Laroussilhe, Andrea Gesmundo, Mona Attariyan, Sylvain Gelly*.  [[pdf](http://proceedings.mlr.press/v97/houlsby19a/houlsby19a.pdf)], [[project](https://github.com/google-research/adapter-bert)],  2019.6

2.  **Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer.** JMLR.  ![](https://img.shields.io/badge/T5-blue) ![](https://img.shields.io/badge/Seq2Seq-red)
   *Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu.* [[pdf](https://arxiv.org/abs/1910.10683)], [[project](https://github.com/google-research/text-to-text-transfer-transformer)].  2019.10. 



3. **Language Models as Knowledge Bases?** EMNLP 2019. ![](https://img.shields.io/badge/LAMA-blue)  ![](https://img.shields.io/badge/Probing-brown) ![](https://img.shields.io/badge/Discrete_Template-red) 

   *Fabio Petroni, Tim Rocktaschel, Patrick Lewis, Anton Bakhtin, Yuxiang Wu, Alexander H. Miller, Sebastian Riedel.*  [[pdf](https://arxiv.org/abs/1909.01066)], [[project](https://github.com/facebookresearch/LAMA)] , 2019.9 

4.  **How Can We Know What Language Models Know?** TACL 2020. ![](https://img.shields.io/badge/Probing-brown) ![](https://img.shields.io/badge/Discrete_Template-red) 
   
    *Zhengbao Jiang, Frank F. Xu, Jun Araki, Graham Neubig*.  [[pdf](https://arxiv.org/abs/1911.12543)], [[project](https://github.com/jzbjyb/LPAQA)], 2019.11


5. **Language Models are Few-shot Learners.** NeurIPS 2020. ![](https://img.shields.io/badge/GPT3-blue) ![](https://img.shields.io/badge/Discrete_Template-red) 

   *Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, Sandhini Agarwal, Ariel Herbert-Voss, Gretchen Krueger, Tom Henighan, Rewon Child, Aditya Ramesh, Daniel M. Ziegler, Jeffrey Wu, Clemens Winter, Christopher Hesse, Mark Chen, Eric Sigler, Mateusz Litwin, Scott Gray, Benjamin Chess, Jack Clark, Christopher Berner, Sam McCandlish, Alec Radford, Ilya Sutskever, Dario Amodei.*   [[pdf](https://arxiv.org/abs/2005.14165)], [[website](https://openai.com/blog/gpt-3-apps/)], 2020.5

6. **AdaPrompt: Adaptive Model Training for Prompt-based NLP** ![](https://img.shields.io/badge/PET_Extension-blue)

   *Yulong Chen, Yang Liu, Li Dong, Shuohang Wang, Chenguang Zhu, Michael Zeng, Yue Zhang*  [[pdf](https://arxiv.org/abs/2202.04824)], 2022.02

### Basics
This section contains the exploration on the basic aspects of prompt tuning, such as
template, verbalizer, training paradigms, etc.

1. **Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference.** EACL 2021. ![](https://img.shields.io/badge/PET-blue) ![](https://img.shields.io/badge/Discrete_Template-red) 
   
    *Timo Schick, Hinrich Schütze.*  [[pdf](https://arxiv.org/abs/2001.07676)], [[project](https://github.com/timoschick/pet)], 2020.1


2. **It’s Not Just Size That Matters: Small Language Models Are Also Few-Shot Learners.** NAACL 2021. ![](https://img.shields.io/badge/PET_Extension-blue) ![](https://img.shields.io/badge/Discrete_Template-red) 

   *Timo Schick, Hinrich Schütze.* [[pdf](https://arxiv.org/abs/2009.07118)], [[project](https://github.com/timoschick/pet)], 2020.9

3. **Autoprompt: Eliciting knowledge from language models with automatically generated prompts.** Preprint. ![](https://img.shields.io/badge/AutoPrompt-blue) ![](https://img.shields.io/badge/Discrete_Template-red)

   *Taylor Shin, Yasaman Razeghi, Robert L. Logan IV, Eric Wallace, Sameer Singh.*  [[pdf](https://arxiv.org/abs/2010.15980)], [[website](https://ucinlp.github.io/autoprompt/)], 2020.10

4. **Automatically Identifying Words That Can Serve as Labels for Few-Shot Text Classification.** COLING 2020. ![](https://img.shields.io/badge/PETAL-blue) ![](https://img.shields.io/badge/Verbalizer-red)

    *Timo Schick, Helmut Schmid, Hinrich Schütze.* [[pdf](https://arxiv.org/abs/2010.13641)], [[project](https://github.com/timoschick/pet)], 2020.12

5. **Making Pre-trained Language Models Better Few-shot Learners.** ACL 2021. ![](https://img.shields.io/badge/LMBFF-blue) ![](https://img.shields.io/badge/Discrete_Template-red)

   *Tianyu Gao, Adam Fisch, Danqi Chen.*  [[pdf](https://arxiv.org/abs/2012.15723)], [[project](https://github.com/princeton-nlp/LM-BFF)], 2020.12


6.  **Prefix-tuning: Optimizing continuous prompts for generation**. ACL 2021. ![](https://img.shields.io/badge/Prefix_Tuning-blue) ![](https://img.shields.io/badge/Continuous_Template-red) ![](https://img.shields.io/badge/Generation-brown)

      *Xiang Lisa Li, Percy Liang.* [[pdf](https://arxiv.org/abs/2101.00190)], [[project](https://github.com/XiangLi1999/PrefixTuning)], 2021.1


7. **Prompt Programming for Large Language Models: Beyond the Few-Shot Paradigm.**  Preprint. ![](https://img.shields.io/badge/Discrete_Template-red)
   
      *Laria Reynolds, Kyle McDonell.*  [[pdf](https://arxiv.org/abs/2102.07350)], 2021.2



8.   **Improving and Simplifying Pattern Exploiting Training.** Preprint. ![](https://img.shields.io/badge/ADAPET-blue) ![](https://img.shields.io/badge/Discrete_Template-red)

       *Derek Tam, Rakesh R Menon, Mohit Bansal, Shashank Srivastava, Colin Raffel.* [[pdf]](https://arxiv.org/abs/2103.11955), 2021.3

9.    **GPT understands, too.** Preprint. ![](https://img.shields.io/badge/P_tuning-blue) ![](https://img.shields.io/badge/Mix_Template-red) ![](https://img.shields.io/badge/Probing-brown)

       *Xiao Liu, Yanan Zheng, Zhengxiao Du, Ming Ding, Yujie Qian, Zhilin Yang, Jie Tang*.  [[pdf](https://arxiv.org/abs/2103.10385)], [[project](https://github.com/THUDM/P-tuning)], 2021.3

10.    **The Power of Scale for Parameter-Efﬁcient Prompt Tuning.** Preprint. ![](https://img.shields.io/badge/Soft_Prompt-blue) ![](https://img.shields.io/badge/Continuous_Template-red) 

       *Brian Lester, Rami Al-Rfou, Noah Constant*. [[pdf](https://arxiv.org/abs/2104.08691)], [[project](https://github.com/kipgparker/soft-prompt-tuning)], 2021.4

11.    **Learning How to Ask: Querying LMs with Mixtures of Soft Prompts.** NAACL 2021. ![](https://img.shields.io/badge/Ensemble-blue) ![](https://img.shields.io/badge/Continuous_Template-red) 

       *Guanghui Qin, Jason Eisner.* [[pdf](https://arxiv.org/abs/2104.06599)][[project](https://github.com/hiaoxui/soft-prompts)], 2021.4



12.    **Factual Probing Is [MASK]: Learning vs. Learning to Recall.** NAACL 2021. ![](https://img.shields.io/badge/OptiPrompt-blue) ![](https://img.shields.io/badge/Continuous_Template-red)  ![](https://img.shields.io/badge/Probing-brown)

       *Zexuan Zhong, Dan Friedman, Danqi Chen.*  [[pdf](https://arxiv.org/abs/2104.05240)], [[project](https://github.com/princeton-nlp/OptiPrompt)], 2021.4



13.    **Cutting Down on Prompts and Parameters: Simple Few-Shot Learning with Language Models.** Preprint. ![](https://img.shields.io/badge/null_prompts-blue)

        *Robert L. Logan IV, Ivana Balažević, Eric Wallace, Fabio Petroni, Sameer Singh, Sebastian Riedel*.   [[pdf](https://arxiv.org/abs/2106.13353)], 2021.6


14.  **WARP: Word-level Adversarial ReProgramming.**  ACL 2021. ![](https://img.shields.io/badge/WARP-blue) ![](https://img.shields.io/badge/Continuous_Template-red)

      *Karen Hambardzumyan, Hrant Khachatrian, Jonathan May.*  [[pdf](https://arxiv.org/abs/2101.00121)], [[project](https://github.com/YerevaNN/WARP)], 2021.6

15. **PTR: Prompt Tuning with Rules for Text Classification.** Preprint.  ![](https://img.shields.io/badge/PTR-blue) ![](https://img.shields.io/badge/Discrete_Template-red)
    
    *Xu Han, Weilin Zhao, Ning Ding, Zhiyuan Liu, Maosong Sun.*  [[pdf](https://arxiv.org/abs/2105.11259)], 2021.5


16. **NSP-BERT: A Prompt-based Zero-Shot Learner Through an Original Pre-training Task —— Next Sentence Prediction**  ![](https://img.shields.io/badge/NSPBERT-blue) ![](https://img.shields.io/badge/Discrete_Template-red)
    
    *Yi Sun\*, Yu Zheng\*, Chao Hao, Hangping Qiu*, [[pdf](https://arxiv.org/abs/2109.03564)], [[project](https://github.com/sunyilgdx/NSP-BERT)], 2021.9


17. **Finetuned language models are zero-shot learners.** ![](https://img.shields.io/badge/Instruction_Tuning-blue) ![](https://img.shields.io/badge/FLAN-blue) ![](https://img.shields.io/badge/Pretrain_Prompt-red)
    
    *ason Wei, Maarten Bosma, Vincent Y. Zhao, Kelvin Guu, Adams Wei Yu, Brian Lester, Nan Du, Andrew M. Dai, Quoc V. Le.* [[pdf](https://arxiv.org/abs/2109.01652)], 2021.9

18. **PPT: Pre-trained Prompt Tuning for Few-shot Learning** ![](https://img.shields.io/badge/PPT-blue) ![](https://img.shields.io/badge/Pretrain_Prompt-red)
    
    *Yuxian Gu\*, Xu Han\*, Zhiyuan Liu, Minlie Huang.* [[pdf](https://arxiv.org/abs/2109.04332)], 2021.9

19. **Differentiable Prompt Makes Pre-trained Language Models Better Few-shot Learners.** ICLR 2022. ![](https://img.shields.io/badge/DART-blue) ![](https://img.shields.io/badge/Continuous_Template-red)

    *Ningyu Zhang, Luoqiu Li, Xiang Chen, Shumin Deng, Zhen Bi, Chuanqi Tan, Fei Huang, Huajun Chen.* [[pdf](https://arxiv.org/abs/2108.13161)], [[project](https://github.com/zjunlp/DART)], 2021.10

20. **Multitask Prompted Training Enables Zero-Shot Task Generalization.** ![](https://img.shields.io/badge/T0-blue) ![](https://img.shields.io/badge/multitask-green)

    *Victor Sanh, Albert Webson, Colin Raffel, Stephen H. Bach, Lintang Sutawika, Zaid Alyafeai, Antoine Chaffin, Arnaud Stiegler, Teven Le Scao, Arun Raja, Manan Dey, M Saiful Bari, Canwen Xu, Urmish Thakker, Shanya Sharma Sharma, Eliza Szczechla, Taewoon Kim, Gunjan Chhablani, Nihal Nayak, Debajyoti Datta, Jonathan Chang, Mike Tian-Jian Jiang, Han Wang, Matteo Manica, Sheng Shen, Zheng Xin Yong, Harshit Pandey, Rachel Bawden, Thomas Wang, Trishala Neeraj, Jos Rozen, Abheesht Sharma, Andrea Santilli, Thibault Fevry, Jason Alan Fries, Ryan Teehan, Stella Biderman, Leo Gao, Tali Bers, Thomas Wolf, Alexander M. Rush.* [[pdf](https://arxiv.org/abs/2110.08207)], 2021.10
    
21. **P-Tuning v2: Prompt Tuning Can Be Comparable to Finetuning Universally Across Scales and Tasks.** ACL 2022. ![](https://img.shields.io/badge/P_Tuning_v2-blue) ![](https://img.shields.io/badge/Continuous_Template-red)
    
    *Xiao Liu, Kaixuan Ji, Yicheng Fu, Zhengxiao Du, Zhilin Yang, Jie Tang* [[pdf](https://arxiv.org/abs/2110.07602)], [[project](https://github.com/THUDM/P-tuning-v2)], 2021.10

22. **Black-Box Tuning for Language-Model-as-a-Service.** ICML 2022. ![](https://img.shields.io/badge/Black--Box_Tuning-blue) ![](https://img.shields.io/badge/Derivative--free_optimization-red)
    
    *Tianxiang Sun, Yunfan Shao, Hong Qian, Xuanjing Huang, Xipeng Qiu* [[pdf](https://arxiv.org/abs/2201.03514)], [[project](https://github.com/txsun1997/Black-Box-Tuning)], 2022.1
    
23. **Black-box Prompt Learning for Pre-trained Language Models.** Preprint. ![](https://img.shields.io/badge/-Black--Box%20Prompt%20Learning%20-blue) ![](https://img.shields.io/badge/Derivative--free_optimization-red)
    
    *Shizhe Diao, Xuechun Li, Yong Lin, Zhichao Huang, Tong Zhang* [[pdf](https://arxiv.org/abs/2201.08531)], 2022.1   

24. **Binding Language Models in Symbolic Languages.** Preprint. ![](https://img.shields.io/badge/Binder-blue) ![](https://img.shields.io/badge/Discrete_Template-red) ![](https://img.shields.io/badge/Neural_Symbolic-green)
    
    *Zhoujun Cheng\*, Tianbao Xie\*, Peng Shi, Chengzu Li, Rahul Nadkarni, Yushi Hu, Caiming Xiong, Dragomir Radev, Mari Ostendorf, Luke Zettlemoyer, Noah A. Smith, Tao Yu* [[pdf](https://arxiv.org/abs/2210.02875)], [[project](https://github.com/HKUNLP/Binder)], [[website](https://lm-code-binder.github.io/)], 2022.10
    
25. **A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT.** ![](https://img.shields.io/badge/chatGPT-blue) ![](https://img.shields.io/badge/Prompt_Pattern-red)
    *Jules White, Quchen Fu, Sam Hays, Michael Sandborn, Carlos Olea, Henry Gilbert, Ashraf Elnashar, Jesse Spencer-Smith, Douglas C. Schmidt* [[pdf](https://arxiv.org/abs/2302.11382)], 2023.2

### Analysis
This section contains the analysis of prompt learning methods, including but not limited to why does prompt learning work, various properties of prompt learning methods, limilation of prompt learning methods.
1. **What Makes Good In-Context Examples for GPT-3?**. Preprint. ![](https://img.shields.io/badge/Analysis-green)

    *Jiachang Liu, Dinghan Shen, Yizhe Zhang, Bill Dolan, Lawrence Carin, Weizhu Chen*. [[pdf](https://arxiv.org/abs/2101.06804)] 2021.1

2. **How Many Data Points is a Prompt Worth?** NAACL 2021. ![](https://img.shields.io/badge/Analysis-green)

     *Teven Le Scao, Alexander M. Rush.*  [[pdf](https://arxiv.org/abs/2103.08493)], [[project](https://github.com/TevenLeScao/pet)], 2021.3

3. **Surface Form Competition-Why the Highest Probability Answer Isn’t Always Right.** Preprint. Preprint. ![](https://img.shields.io/badge/calibration-green)

   *Ari Holtzman, Peter West, Vered Schwartz, Yejin Choi, Luke Zettlemoyer.* [[pdf](https://arxiv.org/abs/2104.08315)][[project](https://github.com/peterwestuw/surface-form-competition)], 2021.4

4. **Natural Instructions: Benchmarking Generalization to New Tasks from Natural Language Instructions.** Preprint.  

      *Swaroop Mishra, Daniel Khashabi, Chitta Baral, Hannaneh Hajishirzi.* [[pdf](https://arxiv.org/abs/2104.08773)], [[project](https://arxiv.org/abs/2104.08773)], 2021.4

5. **Fantastically Ordered Prompts and Where to Find Them: Overcoming Few-Shot Prompt Order Sensitivity**. Preprint.  ![](https://img.shields.io/badge/Analysis-green)

    *Yao Lu, Max Bartolo, Alastair Moore, Sebastian Riedel, Pontus Stenetorp*. [[pdf](https://arxiv.org/abs/2104.08786)] 2021.4

6. **Meta-tuning Language Models to Answer Prompts Better.** Preprint. ![](https://img.shields.io/badge/meta_tuning-green)
   
   *Ruiqi Zhong, Kristy Lee\*, Zheng Zhang\*, Dan Klein*. [[pdf](https://arxiv.org/abs/2104.04670)] 2021.4

7. **True Few-Shot Learning with Language Models**. Preprint. ![](https://img.shields.io/badge/few_shot-green)

    *Ethan Perez, Douwe Kiela, Kyunghyun Cho*. [[pdf](https://arxiv.org/abs/2105.11447)], [[project](https://github.com/ethanjperez/true_few_shot)] 2021.5

8. **Why Do Pretrained Language Models Help in Downstream Tasks? An Analysis of Head and Prompt Tuning**. Preprint. ![](https://img.shields.io/badge/theoretical-green)

      *Colin Wei Sang Michael Xie Tengyu Ma* [[pdf](https://arxiv.org/abs/2106.09226)],  2021.6

9.  **Do Prompt-Based Models Really Understand the Meaning of their Prompts?** Preprint. ![](https://img.shields.io/badge/rethinking-green)

      *Albert Webson, Ellie Pavlick.* [[pdf](https://arxiv.org/abs/2109.01247)], [[project](https://github.com/awebson/prompt_semantics)] 2021.9

10. **Avoiding Inference Heuristics in Few-shot Prompt-based Finetuning.** Preprint.  ![](https://img.shields.io/badge/Sentence_Pair-brown) ![](https://img.shields.io/badge/shortcut-green)
   
      *Prasetya Ajie Utama, Nafise Sadat Moosavi, Victor Sanh, Iryna Gurevych.* [[pdf](https://arxiv.org/abs/2109.04144)], 2021.9

11. **Towards a Unified View of Parameter-Efficient Transfer Learning.** Preprint. ![](https://img.shields.io/badge/transfer-green) ![](https://img.shields.io/badge/unify-green)
    
     *Junxian He, Chunting Zhou, Xuezhe Ma, Taylor Berg-Kirkpatrick, Graham Neubig.* [[pdf](https://arxiv.org/abs/2110.04366)], 2021.10

12. **Exploring Low-dimensional Intrinsic Task Subspace via Prompt Tuning.** Preprint. ![](https://img.shields.io/badge/multitask-green)

     *Yujia Qin, Xiaozhi Wang, Yusheng Su, Yankai Lin, Ning Ding, Zhiyuan Liu, Juanzi Li, Lei Hou,Peng Li, Maosong Sun, Jie Zhou* [[pdf](https://arxiv.org/abs/2110.07867)]

13. **Exploring the Universal Vulnerability of Prompt-based Learning Paradigm.** Findings of NAACL 2022. ![](https://img.shields.io/badge/vulnerability-green)

      *Lei Xu, Yangyi Chen, Ganqu Cui, Hongcheng Gao, Zhiyuan Liu* [[pdf](https://arxiv.org/abs/2204.05239)], [[project](https://github.com/leix28/prompt-universal-vulnerability)]

14. **Rethinking the Role of Demonstrations:
What Makes In-Context Learning Work?.** Arxiv 2022. ![](https://img.shields.io/badge/vulnerability-green)

      *Sewon Min, Xinxi Lyu, Ari Holtzman, Mikel Artetxe, Mike Lewis, Hannaneh Hajishirzi, Luke Zettlemoyer* [[pdf](https://arxiv.org/abs/2202.12837)], [[project](https://github.com/Alrope123/rethinking-demonstrations)]
      
15. **Parameter-Efficient Prompt Tuning Makes Generalized and Calibrated Neural Text Retrievers.** Preprint. ![](https://img.shields.io/badge/generalization-green) ![](https://img.shields.io/badge/calibration-green)

      *Weng Lam Tam, Xiao Liu, Kaixuan Ji, Lilong Xue, Yuxiao Dong, Jiahua Liu, Maodi Hu, Jie Tang* [[pdf](https://arxiv.org/abs/2207.07087)] [[project](https://github.com/THUDM/P-tuning-v2/tree/main/PT-Retrieval)]
      
16. **Ignore Previous Prompt: Attack Techniques For Language Models.** Best Paper Award @ NeurIPS ML Safety Workshop 2022. ![](https://img.shields.io/badge/PromptInject-blue)

      *Fábio Perez, Ian Ribeiro* [[pdf](https://arxiv.org/abs/2211.09527)] [[project](https://github.com/agencyenterprise/PromptInject)], 2022.11

### Improvements
This section contains the improvement of the basic prompt tuning methods, include but not limitedd to using additional resources to improving the performances, making up the shortcomings of previous work or conducting prompt tuning in unsual ways.
1.  **Calibrate Before Use: Improving Few-Shot Performance of Language Models.**  Preprint. ![](https://img.shields.io/badge/Calibration-green) 

     *Tony Z. Zhao, Eric Wallace, Shi Feng, Dan Klein, Sameer Singh.*  [[pdf](https://arxiv.org/abs/2102.09690)], [[project](https://github.com/tonyzhaozh/few-shot-learning)], 2021.2

2.  **Text Generation with Efficient (Soft) Q-Learning.** Preprint. ![](https://img.shields.io/badge/Template_Generation-red)  ![](https://img.shields.io/badge/RL-green)

      *Han Guo, Bowen Tan, Zhengzhong Liu, Eric P. Xing, Zhiting Hu.* [[pdf](https://arxiv.org/abs/2106.07704)], 2021.6

3.  **Knowledgeable Prompt-tuning: Incorporating Knowledge into Prompt Verbalizer for Text Classification.** Preprint.  ![](https://img.shields.io/badge/KPT-blue) ![](https://img.shields.io/badge/Discrete_Template-red) ![](https://img.shields.io/badge/knowledge-green) 
         
      *Shengding Hu, Ning Ding, Huadong Wang, Zhiyuan Liu, Juanzi Li, Maosong Sun*. [[pdf](https://arxiv.org/abs/2108.02035)], [[project](https://github.com/ShengdingHu/KnowledgeablePromptTuning)], 2021.8

4.  **Noisy Channel Language Model Prompting for Few-Shot Text Classiﬁcation.** Preprint. ![](https://img.shields.io/badge/noisy_channel-green)

      *Sewon Min, Mike Lewis, Hannaneh Hajishirzi, Luke Zettlemoyer.*  [[pdf](https://arxiv.org/abs/2108.04106)], 2021.8

5. **Adapting Language Models for Zero-shot Learning by Meta-tuning on Dataset and Prompt Collection.** ![](https://img.shields.io/badge/meta_learning-green)
   
   *Ruiqi Zhong, Kristy Lee\* Zheng Zhang\*, Dan Klein.* [[pdf](http://nlp.cs.berkeley.edu/pubs/Zhong-Lee-Zhang-Klein_2021_MetaTuning_paper.pdf)], 2021.9

6. **Revisiting Self-Training for Few-Shot Learning of Language Model.** Preprint. ![](https://img.shields.io/badge/SFLM-blue) ![](https://img.shields.io/badge/Self_Training-green)
   
   *Yiming Chen, Yan Zhang, Chen Zhang, Grandee Lee, Ran Cheng, Haizhou Li.* [[pdf](https://arxiv.org/abs/2110.01256)], 2021.10

7. **LiST: Lite Self-training Makes Efficient Few-shot Learners.** Preprint. ![](https://img.shields.io/badge/LiST-blue) ![](https://img.shields.io/badge/Lightweight_Self_Training-green)

   *Yaqing Wang, Subhabrata Mukherjee, Xiaodong Liu, Jing Gao, Ahmed Hassan Awadallah, Jianfeng Gao.* [[pdf](https://arxiv.org/abs/2110.06274)], 2021.10

8. **Prototypical Verbalizer for Prompt-based Few-shot Tuning.** ACL 2022. ![](https://img.shields.io/badge/ProtoVerb-blue) ![](https://img.shields.io/badge/Discrete_Template-red) ![](https://img.shields.io/badge/Verbalizer-red) 
         
   *Ganqu Cui, Shengding Hu, Ning Ding, Longtao Huang, Zhiyuan Liu*. [[pdf](https://arxiv.org/abs/2203.09770)], [[project](https://github.com/thunlp/OpenPrompt)], 2022.3
   
9. **BBTv2: Pure Black-Box Optimization Can Be Comparable to Gradient Descent for Few-Shot Learning.** Preprint. ![](https://img.shields.io/badge/BBTv2-blue) ![](https://img.shields.io/badge/Derivative--free_optimization-red) 

   *Tianxiang Sun, Zhengfu He, Hong Qian, Xuanjing Huang, Xipeng Qiu* [[pdf](https://arxiv.org/abs/2205.11200)] [[project](https://github.com/txsun1997/Black-Box-Tuning)], 2022.5
   
### Specializations
This section contains the prompt learning methods designed for various NLP task. 


1. **Thinking Aloud: Dynamic Context Generation Improves Zero-Shot Reasoning Performance of GPT-2.** Preprint. ![](https://img.shields.io/badge/Discrete_Template-red) ![](https://img.shields.io/badge/Reasoning-brown)

   *Gregor Betz, Kyle Richardson, Christian Voigt.* [[pdf](https://arxiv.org/abs/2103.13033)] 2021.3

2. **GPT3Mix: Leveraging Large-scale Language Models for Text Augmentation.** Preprint. ![](https://img.shields.io/badge/GPT3Mix-blue) ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/DataAugmentation-brown)

   *Kang Min Yoo, Dongju Park, Jaewook Kang, Sang-Woo Lee, Woomyeong Park.* [[pdf](https://arxiv.org/abs/2104.08826)] 2021.4

3. **Constrained Language Models Yield Few-Shot Semantic Parsers.** Preprint. ![](https://img.shields.io/badge/Dynamic_Template-red) ![](https://img.shields.io/badge/Semantic_Parsing-brown) 
   
   *Richard Shin, Christopher H. Lin, Sam Thomson, Charles Chen, Subhro Roy, Emmanouil Antonios Platanios, Adam Pauls, Dan Klein, Jason Eisner, Benjamin Van Durme.* [[pdf]](https://arxiv.org/abs/2104.08768) 2021.4

4. **Label Verbalization and Entailment for Effective Zero- and Few-Shot Relation Extraction.** EMNLP 2021. ![](https://img.shields.io/badge/Relation_Extraction-brown) 
   
   *Oscar Sainz, Oier Lopez de Lacalle, Gorka Labaka, Ander Barrena, Eneko Agirre.* [[pdf](https://arxiv.org/abs/2109.03659)], 2021.4
   
5. **PADA: A Prompt-based Autoregressive Approach for Adaptation to Unseen Domains** Preprint.![](https://img.shields.io/badge/PADA-blue) ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/DomainAdaptation-brown)

   *Eyal Ben-David, Nadav Oved, Roi Reichart.* [[pdf](https://arxiv.org/abs/2102.12206)][[project](https://github.com/eyalbd2/PADA)] 2021.5



6. **Prompt-Learning for Fine-grained Entity Typing.** Preprint. ![](https://img.shields.io/badge/PLET-blue) ![](https://img.shields.io/badge/EntityTyping-brown)
   
   *Ning Ding, Yulin Chen, Xu Han, Guangwei Xu, Pengjun Xie, Hai-Tao Zheng, Zhiyuan Liu, Juanzi Li, Hong-Gee Kim* [[pdf](https://arxiv.org/abs/2108.10604)],2021.8

7. **KnowPrompt: Knowledge-aware Prompt-tuning with Synergistic Optimization for Relation Extraction.** WWW 2022. ![](https://img.shields.io/badge/KnowPrompt-blue) ![](https://img.shields.io/badge/Relation_Extraction-brown)

   *Xiang Chen, Xin Xie, Ningyu Zhang, Jiahuan Yan, Shumin Deng, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen.*.  [[pdf](https://arxiv.org/abs/2104.07650)], [[project](https://github.com/zjunlp/KnowPrompt)], 2021.9
   
8.  **Exploring Prompt-based Few-shot Learning for Grounded Dialog Generation.** Preprint. ![](https://img.shields.io/badge/dialogue-brown)

      *Chujie Zheng, Minlie Huang.* [[pdf](https://arxiv.org/abs/2109.06513)], 2021.9

9. **SentiPrompt: Sentiment Knowledge Enhanced Prompt-Tuning for Aspect-Based Sentiment Analysis.** Preprint. ![](https://img.shields.io/badge/SentiPrompt-blue) ![](https://img.shields.io/badge/Sentiment_Analysis-brown)
   
      *Chengxi Li, Feiyu Gao, Jiajun Bu, Lu Xu, Xiang Chen, Yu Gu, Zirui Shao, Qi Zheng, Ningyu Zhang, Yongpan Wang, Zhi Yu.*  [[pdf](https://arxiv.org/abs/2109.08306)] 2021.9


10.  **Template-free Prompt Tuning for Few-shot NER.** Preprint. ![](https://img.shields.io/badge/EntLM-blue) ![](https://img.shields.io/badge/NER-brown)
     
      *Ruotian Ma\*, Xin Zhou\*, Tao Gui, Yiding Tan, Qi Zhang, Xuanjing Huang.* [[pdf](https://arxiv.org/abs/2109.13532)], 2021.9

11. **Learning to Prompt for Vision-Language Models.** Preprint. ![](https://img.shields.io/badge/CoOp-blue) ![](https://img.shields.io/badge/Visual_LM-brown) 

      *Kaiyang Zhou, Jingkang Yang, Chen Change Loy, and Ziwei Liu.* [[pdf](https://arxiv.org/abs/2109.01134)], 2021.9
    

12. **CPT: Colorful Prompt Tuning for Pre-trained Vision-Language Models.** Preprint. ![](https://img.shields.io/badge/CPT-blue)![](https://img.shields.io/badge/Visual_Grounding-brown) 
   
      *Yuan Yao\*, Ao Zhang\*, Zhengyan Zhang, Zhiyuan Liu, Tat-Seng Chua, Maosong Sun.* [[pdf](https://arxiv.org/abs/2109.11797)], 2021.10

13. **MSP: Multi-Stage Prompting for Making Pre-trained Language Models Better Translators.** Preprint. ![](https://img.shields.io/badge/MSP-blue)![](https://img.shields.io/badge/Machine_Translation-brown) 

      *Zhixing Tan, Xiangwen Zhang, Shuo Wang, Yang Liu.* [[pdf](https://arxiv.org/abs/2110.06609)], 2021.10

15. **Few-Shot Bot: Prompt-Based Learning for Dialogue Systems.** Preprint. ![](https://img.shields.io/badge/dialogue-brown)

    *Andrea Madotto, Zhaojiang Lin, Genta Indra Winata, Pascale Fung* [[pdf](https://arxiv.org/abs/2110.08118)], 2021.10

16. **Control Prefixes for Text Generation.** Preprint. ![](https://img.shields.io/badge/Control_Prefixes-blue) ![](https://img.shields.io/badge/Generation-brown) ![](https://img.shields.io/badge/Dynamic_template-red)

      *Jordan Clive, Kris Cao, Marek Rei.* [[pdf](https://arxiv.org/abs/2110.08329)], 2021.10


17. **The Power of Prompt Tuning for Low-Resource Semantic Parsing.** Preprint. ![](https://img.shields.io/badge/Semantic_Parsing-brown) 

      *Nathan Schucher, Siva Reddy, Harm de Vries.* [[pdf](https://arxiv.org/abs/2110.08525)], 2021.10

18. **A Good Prompt Is Worth Millions of Parameters? Low-resource Prompt-based Learning for Vision-Language Models.** ![](https://img.shields.io/badge/FewVLM-blue) ![](https://img.shields.io/badge/Visual_LM-brown)

    *Woojeong Jin, Yu Cheng, Yelong Shen, Weizhu Chen, Xiang Ren.* [[pdf](https://arxiv.org/abs/2110.08484)]
    
19. **LightNER: A Lightweight Generative Framework with Prompt-guided Attention for Low-resource NER.**  COLING 2022. ![](https://img.shields.io/badge/LightNER-blue) ![](https://img.shields.io/badge/NER-brown) 

      *Xiang Chen, Lei Li, Shumin Deng, Chuanqi Tan, Changliang Xu, Fei Huang, Luo Si, Huajun Chen, Ningyu Zhang.* [[pdf](https://arxiv.org/abs/2109.00720)], [[project](https://github.com/zjunlp/DeepKE/tree/main/example/ner/few-shot)], 2021.8

20. **UnifiedSKG: Unifying and Multi-Tasking Structured Knowledge Grounding with Text-to-Text Language Models.** ![](https://img.shields.io/badge/UnifiedSKG-blue) ![](https://img.shields.io/badge/Structured_Knowledge_Grounding-brown)  ![](https://img.shields.io/badge/Continuous_Template-red)

    *Tianbao Xie\*, Chen Henry Wu\*, Peng Shi, Ruiqi Zhong, Torsten Scholak, Michihiro Yasunaga, Chien-Sheng Wu, Ming Zhong, Pengcheng Yin, Sida I. Wang, Victor Zhong, Bailin Wang, Chengzu Li, Connor Boyle, Ansong Ni, Ziyu Yao, Dragomir Radev, Caiming Xiong, Lingpeng Kong, Rui Zhang, Noah A. Smith, Luke Zettlemoyer, Tao Yu.*[[pdf](https://arxiv.org/abs/2201.05966)], [[project](https://github.com/hkunlp/unifiedskg)], [[website](https://unifiedskg.com/)], 2022.1


21. **Ontology-enhanced Prompt-tuning for Few-shot Learning.** WWW 2022. ![](https://img.shields.io/badge/OntoPrompt-blue) ![](https://img.shields.io/badge/Information_Extraction-brown) ![](https://img.shields.io/badge/Knowledge_Graph_Completion-red)

      *Hongbin Ye, Ningyu Zhang, Shumin Deng, Xiang Chen, Hui Chen, Feiyu Xiong, Xi Chen, Huajun Chen.* [[pdf](https://arxiv.org/abs/2201.11332)], 2022.1


22. **Learning to Prompt for Continual Learning.** CVPR 2022. ![](https://img.shields.io/badge/L2P-blue) ![](https://img.shields.io/badge/Continual_Learning-brown) ![](https://img.shields.io/badge/Prompt_Pool-red)

      *Zifeng Wang, Zizhao Zhang, Chen-Yu Lee, Han Zhang, Ruoxi Sun, Xiaoqi Ren, Guolong Su, Vincent Perot, Jennifer Dy, Tomas Pfister.* [[pdf](https://arxiv.org/abs/2112.08654)], [[project](https://github.com/google-research/l2p)], 2021.12
      
      
23. **Relation Extraction as Open-book Examination: Retrieval-enhanced Prompt Tuning.** SIGIR 2022. ![](https://img.shields.io/badge/RetrievalRE-blue) ![](https://img.shields.io/badge/Relation_Extraction-brown)

      *Xiang Chen, Lei Li, Ningyu Zhang, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen.* [[pdf](https://arxiv.org/abs/2205.02355)], [[project](https://github.com/zjunlp/PromptKG/tree/main/research/RetrievalRE)], 2022.5


24. **Good Visual Guidance Makes A Better Extractor: Hierarchical Visual Prefix for Multimodal Entity and Relation Extraction.** Findings of NAACL 2022. ![](https://img.shields.io/badge/HVPNeT-blue) ![](https://img.shields.io/badge/Information_Extraction-brown) ![](https://img.shields.io/badge/Multimodal-red)

      *Xiang Chen, Ningyu Zhang, Lei Li, Yunzhi Yao, Shumin Deng, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen.* [[pdf](https://arxiv.org/abs/2205.03521)], [[project](https://github.com/zjunlp/HVPNeT)], 2022.5


25. **Chain of Thought Prompting Elicits Reasoning in Large Language Models.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red) 

      *Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Ed Chi, Quoc Le, Denny Zhou.* [[pdf](https://arxiv.org/abs/2201.11903)]


26. **Self-Consistency Improves Chain of Thought Reasoning in Language Models.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red) 

      *Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Sharan Narang, Aakanksha Chowdhery, Denny Zhou.* [[pdf](https://arxiv.org/abs/2203.11171)]

27. **Large Language Models are Zero-Shot Reasoners.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red) 

      *Takeshi Kojima, Shixiang Shane Gu, Machel Reid, Yutaka Matsuo, Yusuke Iwasawa.* [[pdf](https://arxiv.org/abs/2205.11916)]

28. **Least-to-Most Prompting Enables Complex Reasoning in Large Language Models.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red) 
      
      *Denny Zhou, Nathanael Schärli, Le Hou, Jason Wei, Nathan Scales, Xuezhi Wang, Dale Schuurmans, Olivier Bousquet, Quoc Le, Ed Chi.* [[pdf](https://arxiv.org/abs/2205.10625)]

29. **Maieutic Prompting: Logically Consistent Reasoning with Recursive Explanations.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red)
      
      *Jaehun Jung, Lianhui Qin, Sean Welleck, Faeze Brahman, Chandra Bhagavatula, Ronan Le Bras, Yejin Choi*
[[pdf](https://arxiv.org/abs/2205.11822)]

30.  **On the Advance of Making Language Models Better Reasoners.** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red)

      *Yifei Li, Zeqi Lin, Shizhuo Zhang, Qiang Fu, Bei Chen, Jian-Guang Lou, Weizhu Chen* [[pdf](https://arxiv.org/abs/2205.11822)]
      

31. **Learning to Compose Soft Prompts for Compositional Zero-Shot Learning.** Preprint 2022. ![](https://img.shields.io/badge/CSP-blue) ![](https://img.shields.io/badge/Continuous_Template-red)

      *Nihal V. Nayak\*, Peilin Yu\*, Stephen H. Bach* [[pdf](https://arxiv.org/abs/2204.03574)], [[project](https://github.com/BatsResearch/csp)]

     
32. **Decoupling Knowledge from Memorization: Retrieval-augmented Prompt Learning.** NeurIPS 2022. ![](https://img.shields.io/badge/RetroPrompt-blue)  ![](https://img.shields.io/badge/Continuous_Template-red)

      *Xiang Chen, Lei Li, Ningyu Zhang, Xiaozhuan Liang, Shumin Deng, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen.* [[pdf](https://arxiv.org/abs/2205.14704)], [[project](https://github.com/zjunlp/PromptKG/tree/main/research/RetroPrompt)], 2022.5
    
      
33. **Exploring Length Generalization in Large Language Models.** Preprint 2022. ![](https://img.shields.io/badge/Continuous_Template-red)

      *Cem Anil, Yuhuai Wu, Anders Andreassen, Aitor Lewkowycz, Vedant Misra, Vinay Ramasesh, Ambrose Slone, Guy Gur-Ari, Ethan Dyer, Behnam Neyshabur* [[pdf](https://arxiv.org/abs/2207.04901)]
      
34. **Ask Me Anything: A simple strategy for prompting language models.** Preprint 2022. ![](https://img.shields.io/badge/Continuous_Template-red)
      
      *Simran Arora, Avanika Narayan, Mayee F. Chen, Laurel Orr, Neel Guha, Kush Bhatia, Ines Chami, Frederic Sala, Christopher Ré*
[[pdf](https://arxiv.org/abs/2210.02441)]

35. **Measuring And Narrowing The Compositionality Gap In Language Models**  Preprint 2022. ![](https://img.shields.io/badge/Continuous_Template-red)

      *Ofir Press, Muru Zhang, Sewon Min, Ludwig Schmidt, Noah A. Smith, Mike Lewis* [[pdf](https://ofir.io/self-ask.pdf)]

36. **RLPrompt: Optimizing Discrete Text Prompts with Reinforcement Learning** Preprint 2022. ![](https://img.shields.io/badge/Continuous_Template-red)
    
    *Mingkai Deng, Jianyu Wang, Cheng-Ping Hsieh, Yihan Wang, Han Guo, Tianmin Shu, Meng Song, Eric P. Xing, Zhiting Hu* 
    [[pdf](https://arxiv.org/abs/2205.12548)]
    
37. **Reasoning with Language Model Prompting: A Survey** Preprint 2022. ![](https://img.shields.io/badge/Reasoning-red) 
    
    *Shuofei Qiao, Yixin Ou, Ningyu Zhang, Xiang Chen, Yunzhi Yao, Shumin Deng, Chuanqi Tan, Fei Huang, Huajun Chen* 
    [[pdf](https://arxiv.org/abs/2212.09597)]
    

## Contribution

### Other contributors 
We thank [Yujia Qin](https://github.com/thuqinyj16), [Xiachong Feng](https://github.com/xcfcode), [Chenglei Si](https://github.com/NoviScl) , [Tianbao Xie](https://github.com/Timothyxxx), [Muhtasham Oblokulov](https://github.com/Muhtasham) for the paper recommendation.


### Contributing to this paper list
   - First, think about which category the work should belong to. 
   - Second, use the same format as the others to discribe the work. Note that there should be an empty line between the title and the authors list, and take care of the indentation.
   - Then, add [keywords tags](#keywords-convention). Add the pdf link of the paper. If it is an arxiv publication, we prefer /abs/ format to /pdf/ format.

   **Don't worry if you put all these wrong, we will fix them for you.** Just contribute and promote your awesome work here! 

   If you recommended a work that wasn't yours, you will be added to the contributor list (be sure to provide your information in [other contributors](#other-contributors)).
