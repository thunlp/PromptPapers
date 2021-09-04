# PromptPapers


![](https://img.shields.io/github/last-commit/thunlp/PromptPapers?color=green) ![](https://img.shields.io/badge/PaperNumber-37-brightgreen) ![](https://img.shields.io/badge/PRs-Welcome-red) 

Must-read papers on prompt-based tuning for pre-trained language models. The paper list is mainly mantained by [Ning Ding](https://github.com/ningding97) and [Shengding Hu](https://github.com/shengdinghu). 

## Contents

- [PromptPapers](#promptpapers)
  - [Contents](#contents)
  - [Introduction](#introduction)
  - [Papers](#papers)
    - [Survey](#survey)
    - [Prompt Designing](#prompt-designing)
    - [Prompt Analysis](#prompt-analysis)
    - [Prompt Application](#prompt-application)
  - [Other Contributors](#other-contributors)



## Introduction

This is a paper list about *prompt-based tuning* for large-scale pre-trained language models. Different from traditional fine-tuning that uses an explicit classifier, prompt-based tuning directly uses the pre-trained models to conduct the pre-training tasks for classification or regression. 



## Papers

### Survey

1. **Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing.**  Preprint.

   *Liu, Pengfei, Weizhe Yuan, Jinlan Fu, Zhengbao Jiang, Hiroaki Hayashi, and Graham Neubig.*  [[pdf](https://arxiv.org/pdf/2107.13586)] [[project](http://pretrain.nlpedia.ai)], 2021.7


### Prompt Designing

1. **Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer.**  JMLR.  ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Seq2seq-blue)

   *Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu.* [[pdf](https://arxiv.org/pdf/1910.10683.pdf)], [[project](https://github.com/google-research/text-to-text-transfer-transformer)], **(T5)**.  2019.10. 

2. **Parameter-Efficient Transfer Learning for NLP.** ICML 2019. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Neil Houlsby, Andrei Giurgiu, Stanislaw Jastrzebski, Bruna Morrone, Quentin de Laroussilhe, Andrea Gesmundo, Mona Attariyan, Sylvain Gelly*.  [[pdf](http://proceedings.mlr.press/v97/houlsby19a/houlsby19a.pdf)], [[project](https://github.com/google-research/adapter-bert)],  2019.6


3. **How Can We Know What Language Models Know?** TACL 2020. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Probing-blue)

   *Zhengbao Jiang, Frank F. Xu, Jun Araki, Graham Neubig*.  [[pdf](https://arxiv.org/pdf/1911.12543.pdf)], [[project](https://github.com/jzbjyb/LPAQA)], 2019.11

4. **Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference.** EACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Timo Schick, Hinrich Schütze.*  [[pdf](https://arxiv.org/pdf/2001.07676.pdf)], [[project](https://github.com/timoschick/pet)] **(PET)**, 2020.1

5. **Language Models are Few-shot Learners.** NeurIPS 2020. ![](https://img.shields.io/badge/Discrete-red)

   *Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, Sandhini Agarwal, Ariel Herbert-Voss, Gretchen Krueger, Tom Henighan, Rewon Child, Aditya Ramesh, Daniel M. Ziegler, Jeffrey Wu, Clemens Winter, Christopher Hesse, Mark Chen, Eric Sigler, Mateusz Litwin, Scott Gray, Benjamin Chess, Jack Clark, Christopher Berner, Sam McCandlish, Alec Radford, Ilya Sutskever, Dario Amodei.*   [[pdf](https://arxiv.org/abs/2005.14165)], [[website](https://openai.com/blog/gpt-3-apps/)]  **(GPT-3)**, 2020.5

6. **It’s Not Just Size That Matters: Small Language Models Are Also Few-Shot Learners.** NAACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Timo Schick, Hinrich Schütze.* [[pdf](https://arxiv.org/pdf/2009.07118.pdf)], [[project](https://github.com/timoschick/pet)], 2020.9

7. **Autoprompt: Eliciting knowledge from language models with automatically generated prompts.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue) ![](https://img.shields.io/badge/Probing-blue)

   *Taylor Shin, Yasaman Razeghi, Robert L. Logan IV, Eric Wallace, Sameer Singh.*  [[pdf](https://arxiv.org/pdf/2010.15980.pdf)], [[website](https://ucinlp.github.io/autoprompt/)] **(AutoPrompt)**, 2020.10

8. **Automatically Identifying Words That Can Serve as Labels for Few-Shot Text Classification.** COLING 2020. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

      *Timo Schick, Helmut Schmid, Hinrich Schütze* [[pdf](https://arxiv.org/pdf/2010.13641.pdf)], [[project](https://github.com/timoschick/pet)], 2020.12


9. **Making Pre-trained Language Models Better Few-shot Learners.** ACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Tianyu Gao, Adam Fisch, Danqi Chen.*  [[pdf](https://arxiv.org/pdf/2012.15723.pdf)], [[project](https://github.com/princeton-nlp/LM-BFF)]  **(LM-BFF)**, 2020.12



10.  **Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference.** EACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

      *Timo Schick, Hinrich Schütze.*  [[pdf](https://arxiv.org/pdf/2001.07676.pdf)], [[project](https://github.com/timoschick/pet)] **(PET)**, 2021.1

11.  **Prefix-tuning: Optimizing continuous prompts for generation**. ACL 2021. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Generation-blue)

      *Xiang Lisa Li, Percy Liang.* [[pdf](https://arxiv.org/pdf/2101.00190.pdf)], [[project](https://github.com/XiangLi1999/PrefixTuning)], 2021.1

12.  **Calibrate Before Use: Improving Few-Shot Performance of Language Models.**  Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Tony Z. Zhao, Eric Wallace, Shi Feng, Dan Klein, Sameer Singh.*  [[pdf](https://arxiv.org/pdf/2102.09690.pdf)], [[project](https://github.com/tonyzhaozh/few-shot-learning)], 2021.2


13. **Prompt Programming for Large Language Models: Beyond the Few-Shot Paradigm.**  Preprint. ![](https://img.shields.io/badge/Discrete-red)

       *Laria Reynolds, Kyle McDonell.*  [[pdf](https://arxiv.org/pdf/2102.07350)], 2021.2

14.    **Improving and Simplifying Pattern Exploiting Training.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)


       *Derek Tam, Rakesh R Menon, Mohit Bansal, Shashank Srivastava, Colin Raffel.* [[pdf]](https://arxiv.org/pdf/2103.11955.pdf), 2021.3

15.    **GPT understands, too.** Preprint. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Probing-blue) ![](https://img.shields.io/badge/Classification-blue)

       *Xiao Liu, Yanan Zheng, Zhengxiao Du, Ming Ding, Yujie Qian, Zhilin Yang, Jie Tang*.  [[pdf](https://arxiv.org/pdf/2103.10385.pdf)], [[project](https://github.com/THUDM/P-tuning)] **(P-tuning)**, 2021.3

16.    **The Power of Scale for Parameter-Efﬁcient Prompt Tuning.** Preprint. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Classification-blue)

       *Brian Lester, Rami Al-Rfou, Noah Constant*. [[pdf](https://arxiv.org/pdf/2104.08691.pdf)], [[implementation](https://github.com/kipgparker/soft-prompt-tuning)], 2021.4

17.    **Learning How to Ask: Querying LMs with Mixtures of Soft Prompts.** NAACL 2021. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Classification-blue)

       *Guanghui Qin, Jason Eisner* [[pdf](https://arxiv.org/pdf/2104.06599.pdf)][[project](https://github.com/hiaoxui/soft-prompts)], 2021.4



18.    **Factual Probing Is [MASK]: Learning vs. Learning to Recall.** NAACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Probing-blue)

       *Zexuan Zhong, Dan Friedman, Danqi Chen.*  [[pdf](https://arxiv.org/pdf/2104.05240.pdf)], [[project](https://github.com/princeton-nlp/OptiPrompt)], 2021.4


19.    **AdaPrompt: Adaptive Prompt-based Finetuning for Relation Extraction.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

       *Xiang Chen, Xin Xie, Ningyu Zhang, Jiahuan Yan, Shumin Deng, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen*.  [[pdf](https://arxiv.org/pdf/2104.07650.pdf)], 2021.4

20.    **PTR: Prompt Tuning with Rules for Text Classification.** Preprint.  ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

        *Xu Han, Weilin Zhao, Ning Ding, Zhiyuan Liu, Maosong Sun.*  [[pdf](https://arxiv.org/pdf/2105.11259.pdf)] **(PTR)**, 2021.5

21.    **Cutting Down on Prompts and Parameters: Simple Few-Shot Learning with Language Models.** Preprint. 

        *Robert L. Logan IV, Ivana Balažević, Eric Wallace, Fabio Petroni, Sameer Singh, Sebastian Riedel*.   [[pdf](https://arxiv.org/pdf/2106.13353)], 2021.6


22.  **WARP: Word-level Adversarial ReProgramming.**  ACL 2021. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Classification-blue)

      *Karen Hambardzumyan, Hrant Khachatrian, Jonathan May.*  [[pdf](https://arxiv.org/pdf/2101.00121.pdf)], [[project](https://github.com/YerevaNN/WARP)], 2021.6

23.  **Knowledgeable Prompt-tuning: Incorporating Knowledge into Prompt Verbalizer for Text Classification.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)
         
      *Shengding Hu, Ning Ding, Huadong Wang, Zhiyuan Liu, Juanzi Li, Maosong Sun*. [[pdf](https://arxiv.org/abs/2108.02035)], 2021.8

24.  **Noisy Channel Language Model Prompting for Few-Shot Text Classiﬁcation.** Preprint. ![](https://img.shields.io/badge/Classification-blue)

      *Sewon Min, Mike Lewis, Hannaneh Hajishirzi, Luke Zettlemoyer.*  [[pdf](https://arxiv.org/abs/2108.04106)], 2021.8

### Prompt Analysis

1. **Language Models as Knowledge Bases?** EMNLP 2019.  ![](https://img.shields.io/badge/Resource-green) ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Probing-blue)

   *Fabio Petroni, Tim Rocktaschel, Patrick Lewis, Anton Bakhtin, Yuxiang Wu, Alexander H. Miller, Sebastian Riedel.*  [[pdf](https://arxiv.org/pdf/1909.01066.pdf)], [[project](https://github.com/facebookresearch/LAMA)] **(LAMA)**, 2019.9 

2. **What Makes Good In-Context Examples for GPT-3?**. Preprint. ![](https://img.shields.io/badge/Analysis-green)

    *Jiachang Liu, Dinghan Shen, Yizhe Zhang, Bill Dolan, Lawrence Carin, Weizhu Chen*. [[pdf](https://arxiv.org/pdf/2101.06804)] 2021.1

3. **How Many Data Points is a Prompt Worth?** NAACL 2021. Preprint. ![](https://img.shields.io/badge/Analysis-green) ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Teven Le Scao, Alexander M. Rush.*  [[pdf](https://arxiv.org/pdf/2103.08493.pdf)], [[project](https://github.com/TevenLeScao/pet)], 2021.3

4. **Surface Form Competition-Why the Highest Probability Answer Isn’t Always Right.** Preprint. Preprint. ![](https://img.shields.io/badge/Analysis-green)

   *Ari Holtzman, Peter West, Vered Schwartz, Yejin Choi, Luke Zettlemoyer.* [[pdf](https://arxiv.org/pdf/2104.08315.pdf)][[project](https://github.com/peterwestuw/surface-form-competition)], 2021.4

5. **Natural Instructions: Benchmarking Generalization to New Tasks from Natural Language Instructions.** Preprint.  ![](https://img.shields.io/badge/Resource-green)

      *Swaroop Mishra, Daniel Khashabi, Chitta Baral, Hannaneh Hajishirzi.* [[pdf](https://arxiv.org/pdf/2104.08773.pdf)], [[project](https://arxiv.org/pdf/2104.08773.pdf)] 2021.4

6. **Fantastically Ordered Prompts and Where to Find Them: Overcoming Few-Shot Prompt Order Sensitivity**. Preprint.  ![](https://img.shields.io/badge/Analysis-green)

    *Yao Lu, Max Bartolo, Alastair Moore, Sebastian Riedel, Pontus Stenetorp*. [[pdf](https://arxiv.org/pdf/2104.08786.pdf)] 2021.4

7. **Meta-tuning Language Models to Answer Prompts Better.** Preprint. ![](https://img.shields.io/badge/Analysis-green)
   
   *Ruiqi Zhong, Kristy Lee\*, Zheng Zhang\*, Dan Klein*. [[pdf](https://arxiv.org/abs/2104.04670.pdf)] 2021.4

8. **True Few-Shot Learning with Language Models**. Preprint. ![](https://img.shields.io/badge/Analysis-green)

    *Ethan Perez, Douwe Kiela, Kyunghyun Cho*. [[pdf](https://arxiv.org/pdf/2105.11447.pdf)], [[project](https://github.com/ethanjperez/true_few_shot)] 2021.5



### Prompt Application

1. **Thinking Aloud: Dynamic Context Generation Improves Zero-Shot Reasoning Performance of GPT-2.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Reasoning-blue)

   *Gregor Betz, Kyle Richardson, Christian Voigt.* [[pdf](https://arxiv.org/pdf/2103.13033.pdf)] 2021.3

2. **GPT3Mix: Leveraging Large-scale Language Models for Text Augmentation.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/DataAugmentation-blue)

    *Kang Min Yoo, Dongju Park, Jaewook Kang, Sang-Woo Lee, Woomyeong Park.* [[pdf](https://arxiv.org/pdf/2104.08826.pdf)] 2021.4

3. **PADA: A Prompt-based Autoregressive Approach for Adaptation to Unseen Domains** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/DomainAdaptation-blue)

     *Eyal Ben-David, Nadav Oved, Roi Reichart.* [[pdf](https://arxiv.org/pdf/2102.12206)][[project](https://github.com/eyalbd2/PADA)] 2021.5

4. **Prompt-Learning for Fine-grained Entity Typing** Preprint. ![](https://img.shields.io/badge/EntityTyping-blue)
    
     *Ning Ding, Yulin Chen, Xu Han, Guangwei Xu, Pengjun Xie, Hai-Tao Zheng, Zhiyuan Liu, Juanzi Li, Hong-Gee Kim* [[pdf](https://arxiv.org/pdf/2108.10604.pdf)] 2021.8




## Other Contributors

 We thank [Yujia Qin](https://github.com/thuqinyj16), [Xiachong Feng](https://github.com/xcfcode), [Chenglei Si](https://github.com/NoviScl) , [Tianbao Xie](https://github.com/Timothyxxx)for the paper recommendation. Pull requests and issues are welcomed!
