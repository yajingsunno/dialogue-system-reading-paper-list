# 对话系统论文阅读列表 

----------
## 综述类 ##
- 李纪为博士论文[teaching machines to converse](https://github.com/topics/teaching-machines-to-converse)
- 微软小冰产品设计结构[The Design and Implementation of XiaoIce, an Empathetic Social Chatbot](https://arxiv.org/pdf/1812.08989v1.pdf)  
- 黄民列组综述论文[Challenges in Building Intelligent Open-domain Dialog Systems](https://arxiv.org/abs/1905.05709)
## 数据集 ## 
- Budzianowski, Paweł, et al. **“MultiWOZ - A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling.”**Empirical Methods in Natural Language Processing, 2018, pp. 5016–5026.  
## 对话生成模型 ##
- Liao, Yi, et al. **“QuaSE: Sequence Editing under Quantifiable Guidance.”** Empirical Methods in Natural Language Processing, 2018, pp. 3855–3864.
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
	- Saizheng Zhang,Emily Dinan,Jack Urbanek,Arthur Szlam,Douwe Kiela,Jason Weston **Personalizing Dialogue Agents: I have a dog, do you have pets too?**AAAI2018
	- Kaixiang Mo, Shuangyin Li, Yu Zhang, Jiajun Li, Qiang Yang**Personalizing a Dialogue System with Transfer Learning.**AAAI2018
	 
- 引入结构化知识（背景信息，知识图谱等）
	- Zhou H, Young T, Huang M, et al. **Commonsense Knowledge Aware Conversation Generation with Graph Attention**[C]. international joint conference on artificial intelligence, 2018: 4623-4629.
	
	- He H, Balakrishnan A, Eric M, et al. **Learning Symmetric Collaborative Dialogue Agents with Dynamic Knowledge Graph Embeddings**[J]. meeting of the association for computational linguistics, 2017: 1766-1776.  
	 
	- Li J, Miller A H, Chopra S, et al. **Learning through Dialogue Interactions by Asking Questions**[J]. international conference on learning representations, 2017.  
	
	- Ghazvininejad M, Brockett C, Chang M, et al. **A Knowledge-Grounded Neural Conversation Model**[J]. national conference on artificial intelligence, 2018: 5110-5117.
	
	- Zhu W, Mo K, Zhang Y, et al. **Flexible End-to-End Dialogue System for Knowledge Grounded Conversation.**[J]. arXiv: Computation and Language, 2017.  
	- Guo, Daya, et al. **“Dialog-to-Action: Conversational Question Answering Over a Large-Scale Knowledge Base.”** NIPS 2018: The 32nd Annual Conference on Neural Information Processing Systems, 2018, pp. 2946–2955
	- Fan Wang Jinhua Peng Hua Wu Rongzhong Lian, Min Xie. **Learning to select knowledge for response generation in dialog systems.** arXiv preprint arXiv:1902.04911, 2019.
	- **Mem2Seq: Effectively Incorporating Knowledge Bases into End-to-End Task-Oriented Dialog Systems** ACL2018 
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
	
## 检索式对话模型    
- Wu Y, Wu W, Xing C, et al. **Sequential Matching Network: A New Architecture for Multi-turn Response Selection in Retrieval-Based Chatbots**[J]. meeting of the association for computational linguistics, 2017: 496-505.  

- Wu Y, Wei F, Huang S, et al. **Response Generation by Context-aware Prototype Editing.**[J]. arXiv: Computation and Language, 2018.
- Tom Young, Erik Cambria, Iti Chaturvedi, Minlie Huang, Hao Zhou, Subham Biswas.**Augmenting End-to-End Dialog Systems with Commonsense Knowledge.** AAAI2018  

- Liu B, Yu T, Mengshoel O J, et al. **Customized Nonlinear Bandits for Online Response Selection in Neural Conversation Models**[J]. national conference on artificial intelligence, 2018: 5245-5252.
- Rajendran, Janarthanan, et al.**“Learning End-to-End Goal-Oriented Dialog with Multiple Answers.”** Empirical Methods in Natural Language Processing, 2018, pp. 3834–3843.
- Luo, Liangchen , et al. **"Learning Personalized End-to-End Goal-Oriented Dialog."** (2018).





