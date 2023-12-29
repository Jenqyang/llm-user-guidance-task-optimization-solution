# llm-user-guidance-task-optimization-solution
LLM在事实性以及通识性问题上都有很好甚至超越人类水平的表现，但在垂直领域特别是产品级问答情境中（例如GUI问答和用户操作引导），由于训练语料的缺少或者缺失，模型可能根本无法回答用户的提问。

这类问题尽管可以通过RAG技术甚至千万条正则表达式来解决，但为了进一步探索LLMs端到端解决问题的能力，本项目将采用智谱AI最新发布的[CogAgent](https://github.com/THUDM/CogVLM/)根据GUI截图从0到1生成问答数据，并作为训练数据集进行下一阶段LLM（Mistral-7B-Instruction）微调。

本项目采用Agents理念，CogAgent作为Agent自主完成数据集的构建。其最终目标：用户只需输入GUI截图即可创建基于该产品GUI问答定制优化的LLM模型。