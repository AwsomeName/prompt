## 1. new_bing

Certainly! Here's a prompt you can use with a large language model to extract knowledge graph triplets related to people and institutions, along with their job relationships:

```
Given the following natural language text, extract knowledge graph triplets:

Text: "{text}"

Entities:
- {Person1} (Person)
- {Person2} (Person)
- {Institution1} (Institution)
- {Institution2} (Institution)

Relationships:
- {Person1} works at {Institution1}
- {Person2} is affiliated with {Institution2}
```

Replace `{text}`, `{Person1}`, `{Person2}`, `{Institution1}`, and `{Institution2}` with the relevant information from your input text. This prompt instructs the model to identify entities (people and institutions) and their job-related relationships. Feel free to adapt it as needed for your specific use case! 🌟


## 2. kimi
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



## 3. chatglm3, 优点是没有给出多余的信息，但是本次回答缺少对格式的显式约束
Prompt: Given a natural language text input, please extract the knowledge graph triplets containing entities such as people and institutions, and their job relationships. The output should be in the format of a knowledge graph, where each entity is represented as a node, and the relationships are represented as edges between the nodes. Please also provide a brief description of the input text for context.
Example input text: "Steve Jobs was the co-founder of Apple Inc. He was responsible for revolutionizing the technology industry with innovative products like the iPhone and Macintosh computer. Tim Cook, who succeeded him as CEO, continued to drive the company's growth and expansion."

## 4. chatglm3-6b-32k， 这是2次的结果
Sure, here's a prompt that you can use to train a large model to extract knowledge graph triplets from natural language, including entity types such as people and institutions, and extract their job relationships:

"Provide a dataset of natural language text, along with corresponding entity-linkable information (such as names, organization names, and job titles). The dataset should include examples of text with various types of entities, including people and institutions, as well as text with entities that are not mentioned in the entity-linkable information.

The model should be trained to extract knowledge graph triplets from the text, where a triplet consists of three entities (such as "John Smith" (person), "Google" (organization), and "Software Engineer" (job title)). The model should be able to handle a variety of entity types, including names, organization names, and job titles, and should be able to generalize to new types of entities.

The model should also be able to extract job relationships from the text, such as "John Smith" being a "Software Engineer" at "Google". The model should be evaluated on its ability to extract valid and consistent knowledge graph triplets from the text, and should be able to generalize to new examples of text.

Please provide the dataset and any additional details or constraints that are relevant to training the model."