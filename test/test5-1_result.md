
其实这个prompt测试输入错了，不过正好用来验证refine的能力，看起来kimi更好一点，newbing没有纠正过来

## 1. newbing

Certainly! Let's refine the prompt to better suit your requirements. Here's an improved version:

---

**Prompt for Extracting Knowledge Graph Triplets and Job Relationships:**

```
Given a natural language input describing a person or institution, create a syntactically correct SQL query to extract relevant knowledge graph triplets. These triplets should include information about the entity (such as name, type, and relevant attributes) and their job relationships (if applicable).

Question: Describe the person or institution you want information about.
SQLQuery: SELECT entity_name, entity_type, job_title FROM knowledge_graph WHERE entity_name = 'John Doe';
SQLResult: John Doe | Person | Software Engineer

Answer: John Doe is a Software Engineer.
```

---

Feel free to customize the `SQLQuery` part based on your specific use case. Remember to replace `'John Doe'` with the actual name or identifier of the person or institution you're interested in. This prompt will guide the large model to extract relevant information and provide a concise answer. 🌟





## kimi
To refine the original answer for the task of extracting knowledge graph triplets from natural language, focusing on entity types such as people and institutions and their job relationships, the prompt should be designed to guide the large model in a clear, concise, and relevant manner. Here is a revised prompt:

---

**Prompt:**

"Given a body of text, identify and extract triplets that represent relationships between entities, specifically focusing on people and institutions. Each triplet should consist of an entity (person or institution), the role or job title they hold, and the institution or organization they are associated with. Ensure that the extracted information is accurate and relevant to the context provided.

Please format your output as follows:

1. Entity Type (Person/Institution)
2. Entity Name
3. Role/Job Title
4. Associated Institution/Organization

For example, from the text 'John Smith works as a software engineer at Moonshot AI,' the extracted triplet would be:

- Entity Type: Person
- Entity Name: John Smith
- Role/Job Title: Software Engineer
- Associated Institution: Moonshot AI

Now, please process the following text and extract the relevant triplets:

[Insert Text Here]

---

This refined prompt is designed to be clear and concise, directly addressing the task at hand. It provides a specific example to guide the model and ensures that the output will be in a structured format that is easy to understand and use.


## chatglm6b-32k
Clarity: Please provide a prompt to a large language model to extract knowledge graph triplets from natural language, including entity types such as people and institutions, and their job relationships. Conciseness: Generate a prompt to the language model to extract knowledge graph triplets from natural language. Relevance: The prompt should directly relate to the task of extracting knowledge graph triplets. Completeness: Provide enough context for the generated response to make sense.

Refined Answer:

Question: Extract knowledge graph triplets from natural language, including entity types such as people and institutions, and their job relationships. SQLQuery: SELECT * FROM {schema}.knowledge_graph_triplets WHERE {entity_type} IN ('person', 'institution') AND {job_relationship} EXISTS; SQLResult: List of knowledge graph triplets for {entity_type} with {job_relationship}. Answer: The list of knowledge graph triplets for {entity_type} with {job_relationship}.