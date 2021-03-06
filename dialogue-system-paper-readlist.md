# 对话系统论文阅读列表 

----------
## 综述类 ##
- 李纪为博士论文[teaching machines to converse](https://github.com/topics/teaching-machines-to-converse)
- 微软小冰产品设计结构[The Design and Implementation of XiaoIce, an Empathetic Social Chatbot](https://arxiv.org/pdf/1812.08989v1.pdf)  
- 黄民烈组开放域综述论文[Challenges in Building Intelligent Open-domain Dialog Systems](https://arxiv.org/abs/1905.05709)
- 黄民烈组任务型对话综述论文[Recent Advances and Challenges in Task-oriented Dialog Systems]
- 赵天成博士论文[LEARNING TO CONVERSE WITH LATENT ACTIONS](https://www.cs.cmu.edu/~tianchez/data/phd_thesis.pdf)
## 数据集 ## 
**任务型数据集**
- 【DSTC2】Jason D Williams, Antoine Raux, Deepak Ramachandran, and Alan W Black.**The dialog state tracking challenge.** In Proceed- ings of the SIGDIAL 2013 Conference, pages 404–413, 2013.
- 【Camrest676】Tsung-Hsien Wen, David Vandyke, Nikola Mrksˇic ́, Milica Gasic, Lina M Rojas Barahona, Pei-Hao Su, Stefan Ultes, and Steve Young. **A network-based end-to-end trainable task-oriented dialogue system.** In Proceedings of the 15th Conference of the European Chapter of the Association for Computational Linguistics: Volume 1, Long Papers, pages 438–449, 2017.
- 【MultiWoZ】Budzianowski, Paweł, et al. **“MultiWOZ - A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling.”**Empirical Methods in Natural Language Processing, 2018, pp. 5016–5026.  [对应链接]https://github.com/budzianowski/multiwoz
- 【SGD】Abhinav Rastogi, Xiaoxue Zang, Srinivas Sunkara, Raghav Gupta, and Pranav Khaitan. **Towards scalable multi-domain conversational agents: The schema-guided dialogue dataset.** In Proceedings of the AAAI Conference on Artificial Intelligence, volume 34, 2020.
- 【AirDialogue】Wei Wei, Quoc Le, Andrew Dai, and Jia Li. **Airdialogue: An environ- ment for goal-oriented dialogue research.** In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pages 3844–3854, 2018.

**Note** 更多数据集介绍可参考黄民烈老师组任务型综述对话论文中有详细介绍

**开放域**
情感类：
- STC   单轮 无情感标注
- Cornell Movie Dialogs  多轮 无情感标注
- OpenSubtitles  多轮 噪声较大 无情感标注
- Twitter  单轮高质量 有标签
- DailyDialog 多轮高质量 有标签


## 对话生成模型 ##
- Liao, Yi, et al. **“QuaSE: Sequence Editing under Quantifiable Guidance.”** Empirical Methods in Natural Language Processing, 2018, pp. 3855–3864.
- [DialoGPT: Large-Scale Generative Pre-training for Conversational Response Generation](https://www.microsoft.com/en-us/research/publication/dialogpt-large-scale-generative-pre-training-for-conversational-response-generation/)
- [Hello, It's GPT-2 -- How Can I Help You? Towards the Use of Pretrained Language Models for Task-Oriented Dialogue Systems](http://arxiv.org/abs/1907.05774)
- [PLATO: Pre-trained Dialogue Generation Model with Discrete Latent Variable](http://arxiv.org/abs/1910.07931)
- 基于控制**主题**的seq2seq模型  
	- Xing C, Wu W, Wu Y, et al. **Topic Aware Neural Response Generation**.[J]. national conference on artificial intelligence, 2017: 3351-3357.  
	
	- Wang W, Huang M, Xu X, et al. **Chat More: Deepening and Widening the Chatting Topic via A Deep Model**[C]. international acm sigir conference on research and development in information retrieval, 2018: 255-264  


	- Mou L , Song Y , Yan R , et al. **Sequence to Backward and Forward Sequences: A Content-Introducing Approach to Generative Short-Text Conversation**[J]. 2016.  
  
	- Yao L, Zhang Y, Feng Y, et al. **Towards implicit contentintroducing for generative short-text conversation systems**[C]//Proceedings of the 2017 Conference on Empirical Methods in Natural Language Processing. 2017: 2190-2199.    

	- Li J, Sun X. **A Syntactically Constrained BidirectionalAsynchronous Approach for Emotional Conversation Generation**[C]//Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing. 2018: 678-683.
	 
	- Zhou G, Luo P, Cao R, et al.**Mechanism-Aware Neural Machine for Dialogue Response Generation.**[C]. national conference on artificial intelligence, 2017: 3400-3407.  
- 基于控制属性**（句式，情感信息）**的seq2seq模型
	- Ke P, Guan J, Huang M, et al. **Generating Informative Responses with Controlled Sentence Function**[C]//Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers). 2018, 1: 1499-1508.  
	  
	- Zhou H, Huang M, Zhang T, et al. **Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory**[J]. national conference on artificial intelligence, 2018: 730-739.
	
	- Yansen Wang, Chenyi Liu, Minlie Huang, Liqiang Nie. **Learning to ask questions in open-domain conversation systems**. ACL 2018  
	- Can Xu, Wei Wu, Chongyang Tao, Huang Hu, Matt Schuerman, Ying Wang: **Neural Response Generation with Meta-words** ACL (1) 2019: 5416-5426
	- Topic-Aware Multi-turn Dialogue Modeling.AAAI2021
	- Qintong Li. Towards Empathetic Dialogue Generation over Multi-type Knowledge.WWW2021


 
- 修改beamsearch/decoder/模型结构
	- Li J, Monroe W, Jurafsky D. **A simple, fast diverse decoding algorithm for neural generation**[J]. arXiv preprint arXiv:1611.08562, 2016.  
  
	- Vijayakumar A K, Cogswell M, Selvaraju R R, et al. **Diverse beam search: Decoding diverse solutions from neural sequence models**[J]. arXiv preprint arXiv:1610.02424, 2016  
	
	- Jiwei Li, Michel Galley, Chris Brockett, Jianfeng Gao, and Bill Dolan. 2016a. **A diversitypromoting objective function for neural conversation models.** NAACL  
	 
	- Jiwei Li, Will Monroe, and Dan Jurafsky. 2016c. **A simple, fast diverse decoding algorithm for neural generation.** arXiv preprint arXiv:1611.08562 
	 
	- Wu Y, Wu W, Li Z, et al. **Neural Response Generation with Dynamic Vocabularies**[J]. national conference on artificial intelligence, 2018: 5594-5601.  
	- **Towards Less Generic Responses in Neural Conversation Models: A Statistical Re-weighting Method**EMNLP2018
- 引入personality保持对话一致
	- Li J, Galley M, Brockett C, et al.**A Persona-Based Neural Conversation Model**[J]. meeting of the association for computational linguistics, 2016: 994-1003.  
	
	- Qian Q, Huang M, Zhao H, et al. **Assigning Personality/Profile to a Chatting Machine for Coherent Conversation Generation**[J]. international joint conference on artificial intelligence, 2018: 4279-4285. 
	 
	- Eric Chu, Prashanth Vijayaraghavan, Deb Roy. **"Learning Personas from Dialogue with Attentive Memory Networks."** EMNLP (2018). 
	- Saizheng Zhang,Emily Dinan,Jack Urbanek,Arthur Szlam,Douwe Kiela,Jason Weston **Personalizing Dialogue Agents: I have a dog, do you have pets too?**  AAAI2018
	- **Exploiting Persona Information for Diverse Generation of Conversational Responses** IJCAI2019
	- Kaixiang Mo, Shuangyin Li, Yu Zhang, Jiajun Li, Qiang Yang**Personalizing a Dialogue System with Transfer Learning.**AAAI2018
	- Casanueva I, Hain T, Christensen H, et al. **Knowledge transfer between speakers for personalised dialogue management**[C]//Proceedings of the 16th Annual Meeting of the Special Interest Group on Discourse and Dialogue. 2015: 12-21.
	- [1911.04700 A Pre-training Based Personalized Dialogue Generation Model with Persona-sparse Data](https://arxiv.org/abs/1911.04700)
	- Generate, Delete and Rewrite: A Three-Stage Framework for Improving Persona Consistency of Dialogue Generation AAAI2020
	- Learning to Customize Model Structures for Few-shot Dialogue Generation Tasks ACL2020
	- A Pre-training Based Personalized Dialogue Generation Model with Persona-sparse Data AAAI2020
	- You Impress Me: Dialogue Generation via Mutual Persona Perception AAAI2020
	- Will I Sound Like Me? Improving Persona Consistency in Dialogues through Pragmatic Self-Consciousness ICLR2020





	
	
- 基于预训练模型的可控对话生成
	- Zeng Y, Nie J Y. **Generalized Conditioned Dialogue Generation Based on Pre-trained Language Model**[J]. arXiv preprint arXiv:2010.11140, 2020.
	- Zheng Y, Chen Z, Zhang R, et al. **Stylized Dialogue Response Generation Using Stylized Unpaired Texts**[J]. arXiv e-prints, 2020: arXiv: 2009.12719.
- 基于数据增强的对话生成
	- Data Manipulation: Towards Effective Instance Learning for Neural Dialogue Generation via Learning to Augment and Reweight. ACL2020
	- Diversifying Task-oriented Dialogue Response  Generation with Prototype Guided Paraphrasing. ACL2020
	- SMRT Chatbots: Improving Non-Task-Oriented Dialog with Simulated Multiple Reference Training. EMNLP2020
	
- 引入结构化知识（背景信息，知识图谱等）
	- Zhou H, Young T, Huang M, et al. **Commonsense Knowledge Aware Conversation Generation with Graph Attention**[C]. international joint conference on artificial intelligence, 2018: 4623-4629.
	
	- He H, Balakrishnan A, Eric M, et al. **Learning Symmetric Collaborative Dialogue Agents with Dynamic Knowledge Graph Embeddings**[J]. meeting of the association for computational linguistics, 2017: 1766-1776.  
	 
	- Li J, Miller A H, Chopra S, et al. **Learning through Dialogue Interactions by Asking Questions**[J]. international conference on learning representations, 2017.  
	
	- Ghazvininejad M, Brockett C, Chang M, et al. **A Knowledge-Grounded Neural Conversation Model**[J]. national conference on artificial intelligence, 2018: 5110-5117.
	
	- Zhu W, Mo K, Zhang Y, et al. **Flexible End-to-End Dialogue System for Knowledge Grounded Conversation.**[J]. arXiv: Computation and Language, 2017.  
	- Guo, Daya, et al. **“Dialog-to-Action: Conversational Question Answering Over a Large-Scale Knowledge Base.”** NIPS 2018: The 32nd Annual Conference on Neural Information Processing Systems, 2018, pp. 2946–2955
	- Fan Wang Jinhua Peng Hua Wu Rongzhong Lian, Min Xie. **Learning to select knowledge for response generation in dialog systems.** arXiv preprint arXiv:1902.04911, 2019.
	- **Mem2Seq: Effectively Incorporating Knowledge Bases into End-to-End Task-Oriented Dialog Systems** ACL2018 
	
	- Liu Z, Niu Z Y, Wu H, et al. **Knowledge Aware Conversation Generation with Reasoning on Augmented Graph**[J]. arXiv preprint arXiv:1903.10245, 2019.
	- Rongzhong Lian, Min Xie, Fan Wang, Jinhua Peng, Hua Wu,et al. **Learning to select Knowledge for Response Generation in Dialog System** arXiv preprint arXiv:1902.04911, 2019.
	- History-Adaption Knowledge Incorporation Mechanism for Multi-Turn Dialogue System  AAAI2020
	- Sequential latent knowledge selection for knowledge-grounded dialogue. ICLR2020
	- Difference-aware Knowledge Selection for Knowledge-grounded Conversation Generation. 2020
	- Knowledge-Grounded Dialogue Generation with Pre-trained Language Models. 2020
	- dge Graph Grounded Goal Planning for Open-Domain Conversation Generation. AAAI2020
	- Conversational Graph Grounded Policy Learning for Open-Domain Conversation Generation ACL2020

- 基于GAN的对话系统  
	- Xu Z, Liu B, Wang B, et al. **Neural Response Generation via GAN with an Approximate Embedding Layer.**[C]. empirical methods in natural language processing, 2017: 617-626.
	- Young, Tom, et al.  **Augmenting End-to-End Dialogue Systems with Commonsense Knowledge.”**National Conference on Artificial Intelligence, 2018, pp. 4970–4977.    
	- Zhang, Yizhe, et al. **“Generating Informative and Diverse Conversational Responses via Adversarial Information Maximization.”** Neural Information Processing Systems, 2018, pp. 1815–1825.
	
	
- 基于强化学习的对话系统
	- Jiwei Li, Will Monroe, Alan Ritter, Michel Galley, Jianfeng Gao, and Dan Jurafsky. 2016d. **Deep reinforcement learning for dialogue generation.** EMNLP .  
	
	- Jiwei Li, Will Monroe, and Dan Jurafsky. 2017c. **Learning to decode for future success**. arXiv preprint arXiv:1701.06549 .    
	- Zhou G, Luo P, Xiao Y, et al. **Elastic Responding Machine for Dialog Generation with Dynamically Mechanism Selecting**[C]. national conference on artificial intelligence, 2018: 5730-5737.
	- Liu, Bing, et al. **“Customized Nonlinear Bandits for Online Response Selection in Neural Conversation Models.”** National Conference on Artificial Intelligence, 2018, pp. 5245–5252
- 对话历史信息建模
	- Xing C, Wu Y, Wu W, et al. **Hierarchical Recurrent Attention Network for Response Generation**[J]. national conference on artificial intelligence, 2018: 5610-5617. 
	
	- Ruizhe Li, Chenghua Lin, Matthew Collinson, Xiao Li, Guanyi Chen. "**A Dual-Attention Hierarchical Recurrent Neural Network for Dialogue Act Classification**." arXiv:1810.09154 (2018).  
	- Bao S, He H, Wang F, et al. **Know More about Each Other: Evolving Dialogue Strategy via Compound Assessment**[J]. arXiv preprint arXiv:1906.00549, 2019.

- 对话策略
	- Wu W, Guo Z, Zhou X, et al. **Proactive Human-Machine Conversation with Explicit Conversation Goals**[J]. arXiv preprint arXiv:1906.05572, 2019.
	
## 检索式对话模型    
- Wu Y, Wu W, Xing C, et al. **Sequential Matching Network: A New Architecture for Multi-turn Response Selection in Retrieval-Based Chatbots**[J]. meeting of the association for computational linguistics, 2017: 496-505.  

- Wu Y, Wei F, Huang S, et al. **Response Generation by Context-aware Prototype Editing.**[J]. arXiv: Computation and Language, 2018.
- Tom Young, Erik Cambria, Iti Chaturvedi, Minlie Huang, Hao Zhou, Subham Biswas.**Augmenting End-to-End Dialog Systems with Commonsense Knowledge.** AAAI2018  

- Liu B, Yu T, Mengshoel O J, et al. **Customized Nonlinear Bandits for Online Response Selection in Neural Conversation Models**[J]. national conference on artificial intelligence, 2018: 5245-5252.
- Rajendran, Janarthanan, et al.**“Learning End-to-End Goal-Oriented Dialog with Multiple Answers.”** Empirical Methods in Natural Language Processing, 2018, pp. 3834–3843.
- Luo, Liangchen , et al. **"Learning Personalized End-to-End Goal-Oriented Dialog."** (2018).
- Zhao X, Tao C, Wu W, et al. **A Document-grounded Matching Network for Response Selection in Retrieval-based Chatbots**[J]. arXiv preprint arXiv:1906.04362, 2019.





