## 1. kimi
当然，以下是一个为大模型设计的prompt，用于从自然语言中抽取知识图谱三元组，特别是关于人物和机构的任职关系：

---

**Prompt:**

请仔细阅读以下文本，并从中抽取知识图谱三元组。你需要识别出文本中提到的所有人物和机构实体，并确定它们之间的任职关系。请确保你抽取的三元组包含以下元素：

1. 实体类型：人物（Person）和机构（Organization）。
2. 关系类型：任职关系（Employment）。
3. 具体的三元组格式应为：(实体1, 关系, 实体2)。

例如，如果你在文本中发现“张伟是月之暗面科技有限公司的首席执行官”，那么你应该抽取的三元组是：(张伟, 是首席执行官, 月之暗面科技有限公司)。

请在处理文本时注意以下指导原则：
- 确保实体和关系的定义清晰准确。
- 如果文本中提到了多个任职关系，请分别抽取每个关系。
- 如果文本中的关系不明确或含糊，请根据上下文推断最可能的关系类型。
- 忽略任何不相关或不完整的信息。

现在，请开始处理文本并提供抽取的三元组列表。

---

这个prompt为大模型提供了清晰的任务描述和执行指南，确保模型能够理解并执行抽取知识图谱三元组的任务。



### 英文==========

Certainly! Here's a prompt designed for a large model to extract knowledge graph triplets focusing on job relationships between people and institutions from natural language:

---

**Prompt:**

You are tasked with extracting knowledge graph triplets from the provided text. Please identify and categorize entities as either people or institutions and determine the job relationships between them. Your extracted triplets should include the following elements:

1. Entity Types: Person and Institution.
2. Relationship Type: Job or Position held.
3. Triplet Format: (Entity1, Relationship, Entity2).

For instance, if the text mentions "John Smith is the CEO of Moonshot AI," the triplet you should extract would be: (John Smith, is CEO of, Moonshot AI).

Please follow these guidelines while processing the text:
- Ensure that the entities and relationships are clearly defined and accurate.
- If multiple job relationships are mentioned, extract each one separately.
- If the relationship is not explicitly stated or is ambiguous, infer the most likely type of relationship based on the context.
- Exclude any irrelevant or incomplete information.

Now, please begin processing the text and provide a list of the extracted triplets.

---

This prompt gives the large model a clear task description and guidelines to follow, ensuring that the model can understand and perform the task of extracting knowledge graph triplets effectively.