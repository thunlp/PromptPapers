# PromptPapers


![](https://img.shields.io/github/last-commit/thunlp/PromptPapers?color=green) ![](https://img.shields.io/badge/PaperNumber-18-brightgreen) ![](https://img.shields.io/badge/PRs-Welcome-red) 

Must-read papers on prompt-based tuning for pre-trained language models. The paper list is mainly mantained by [Ning Ding](https://github.com/ningding97) and [Shengding Hu](https://github.com/shengdinghu).

## Introduction

This is a paper list about *prompt-based tuning* for large-scale pre-trained language models. Different from traditional fine-tuning that uses an explicit classifier, prompt-based tuning directly uses the pre-trained models to conduct the pre-training tasks for classification or regression. 



## Papers

1. **Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer.**  JMLR.  ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Seq2seq-blue)

   *Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu.* [[pdf](https://arxiv.org/pdf/1910.10683.pdf)], [[project](https://github.com/google-research/text-to-text-transfer-transformer)], **(T5)**.  2019.10. 

2. **Parameter-Efficient Transfer Learning for NLP.** ICML 2019. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Neil Houlsby, Andrei Giurgiu, Stanislaw Jastrzebski, Bruna Morrone, Quentin de Laroussilhe, Andrea Gesmundo, Mona Attariyan, Sylvain Gelly*.  [[pdf](http://proceedings.mlr.press/v97/houlsby19a/houlsby19a.pdf)], [[project](https://github.com/google-research/adapter-bert)],  2019.6

3. **Language Models as Knowledge Bases?** EMNLP 2019.  ![](https://img.shields.io/badge/Resource-green)

   *Fabio Petroni, Tim Rocktaschel, Patrick Lewis, Anton Bakhtin, Yuxiang Wu, Alexander H. Miller, Sebastian Riedel.*  [[pdf](https://arxiv.org/pdf/1909.01066.pdf)], [[project](https://github.com/facebookresearch/LAMA)] **(LAMA)**, 2019.9 

4. **How Can We Know What Language Models Know?** TACL 2020. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Probing-blue)

   *Zhengbao Jiang, Frank F. Xu, Jun Araki, Graham Neubig*.  [[pdf](https://arxiv.org/pdf/1911.12543.pdf)], [[project](https://github.com/jzbjyb/LPAQA)], 2019.11

5. **Language Models are Few-shot Learners.** NeurIPS 2020. ![](https://img.shields.io/badge/Discrete-red)

   *Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, Sandhini Agarwal, Ariel Herbert-Voss, Gretchen Krueger, Tom Henighan, Rewon Child, Aditya Ramesh, Daniel M. Ziegler, Jeffrey Wu, Clemens Winter, Christopher Hesse, Mark Chen, Eric Sigler, Mateusz Litwin, Scott Gray, Benjamin Chess, Jack Clark, Christopher Berner, Sam McCandlish, Alec Radford, Ilya Sutskever, Dario Amodei.*   [[pdf](https://arxiv.org/abs/2005.14165)], [[website](https://openai.com/blog/gpt-3-apps/)]  **(GPT-3)**, 2020.5

6. **It’s Not Just Size That Matters: Small Language Models Are Also Few-Shot Learners.** NAACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Timo Schick, Hinrich Schütze.* [[pdf](https://arxiv.org/pdf/2009.07118.pdf)], [[project](https://github.com/timoschick/pet)], 2020.9

7. **Autoprompt: Eliciting knowledge from language models with automatically generated prompts.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue) ![](https://img.shields.io/badge/Probing-blue)

   *Taylor Shin, Yasaman Razeghi, Robert L. Logan IV, Eric Wallace, Sameer Singh.*  [[pdf](https://arxiv.org/pdf/2010.15980.pdf)], [[website](https://ucinlp.github.io/autoprompt/)] **(AutoPrompt)**, 2020.10

8. **Making Pre-trained Language Models Better Few-shot Learners.** ACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Tianyu Gao, Adam Fisch, Danqi Chen.*  [[pdf](https://arxiv.org/pdf/2012.15723.pdf)], [[project](https://github.com/princeton-nlp/LM-BFF)]  **(LM-BFF)**, 2020.12

9. **Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference.** EACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

   *Timo Schick, Hinrich Schütze.*  [[pdf](https://arxiv.org/pdf/2001.07676.pdf)], [[project](https://github.com/timoschick/pet)] **(PET)**, 2021.1

10. **Prefix-tuning: Optimizing continuous prompts for generation**. Preprint. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Generation-blue)
    
    *Xiang Lisa Li, Percy Liang.* [[pdf](https://arxiv.org/pdf/2101.00190.pdf)], [[project](https://github.com/XiangLi1999/PrefixTuning)], 2021.1

11.  **Calibrate Before Use: Improving Few-Shot Performance of Language Models.**  Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)
      
		*Tony Z. Zhao, Eric Wallace, Shi Feng, Dan Klein, Sameer Singh.*  [[pdf](https://arxiv.org/pdf/2102.09690.pdf)], [[project](https://github.com/tonyzhaozh/few-shot-learning)], 2021.2


12.  **Prompt Programming for Large Language Models: Beyond the Few-Shot Paradigm.**  Preprint. ![](https://img.shields.io/badge/Discrete-red)
    
     *Laria Reynolds, Kyle McDonell.*  [[pdf](https://arxiv.org/pdf/2102.07350)], 2021.2


13.  **The Power of Scale for Parameter-Efﬁcient Prompt Tuning.** Preprint. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Classification-blue)

     *Brian Lester, Rami Al-Rfou, Noah Constant*. [[pdf](https://arxiv.org/pdf/2104.08691.pdf)], [[implementation](https://github.com/kipgparker/soft-prompt-tuning)], 2021.4


14.  **How Many Data Points is a Prompt Worth?** NAACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Teven Le Scao, Alexander M. Rush.*  [[pdf](https://arxiv.org/pdf/2103.08493.pdf)], [[project](https://github.com/TevenLeScao/pet)], 2021.3


15.  **GPT understands, too.** Preprint. ![](https://img.shields.io/badge/Continuous-red) ![](https://img.shields.io/badge/Probing-blue) ![](https://img.shields.io/badge/Classification-blue)

     *Xiao Liu, Yanan Zheng, Zhengxiao Du, Ming Ding, Yujie Qian, Zhilin Yang, Jie Tang*.  [[pdf](https://arxiv.org/pdf/2103.10385.pdf)], [[project](https://github.com/THUDM/P-tuning)] **(P-tuning)**, 2021.3


16.  **Factual Probing Is [MASK]: Learning vs. Learning to Recall.** NAACL 2021. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Probing-blue)

     *Zexuan Zhong, Dan Friedman, Danqi Chen.*  [[pdf](https://arxiv.org/pdf/2104.05240.pdf)], [[project](https://github.com/princeton-nlp/OptiPrompt)], 2021.4


17.  **AdaPrompt: Adaptive Prompt-based Finetuning for Relation Extraction.** Preprint. ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Xiang Chen, Xin Xie, Ningyu Zhang, Jiahuan Yan, Shumin Deng, Chuanqi Tan, Fei Huang, Luo Si, Huajun Chen*.  [[pdf](https://arxiv.org/pdf/2104.07650.pdf)], 2021.4
     

18.  **PTR: Prompt Tuning with Rules for Text Classification.** Preprint.  ![](https://img.shields.io/badge/Discrete-red) ![](https://img.shields.io/badge/Classification-blue)

     *Xu Han, Weilin Zhao, Ning Ding, Zhiyuan Liu, Maosong Sun.*  [[pdf](https://arxiv.org/pdf/2105.11259.pdf)] **(PTR)**, 2021.5
     
     
    
    
    
    
