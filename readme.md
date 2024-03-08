搜集有价值的prompt，至于怎么使用还在考虑

首先，可以用于大模型的特定任务
第二，可以用于instruct tuning
第三，主要思考一个问题，模型如何选择prompt？

最后，总结prompt的经验

-------
目前搜集的是llama_index项目中的prompt，主要是针对RAG、Text2SQL、extract（包括kg）

现在我的问题是
1、能不能用LLM根据任务选择一个合适的prompt？
2、能不能用LLM根据任务情景，直接生成prompt？

之前我测试的效果不理想，这次使用GPT和国内的GLM再测试一次，测试query和结果放在test目录下


目前测试的结果，kimi（月之暗面），newbing，都不错，特别是kimi，长度长，而且个别case比newbing还好（refine的case）
chatglm也不错，但是chatglm6b-32k不太稳定，有的时候答非所问，而有的时候又有一点惊喜，还是开源性价比。