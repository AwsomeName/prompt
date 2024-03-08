
## 1. kimi

Refined Answer:

"Your goal is to extract structured knowledge graph triplets from a given text, focusing on entities such as people and institutions and their job-related connections. To assist you in this task, please adhere to the following prompt:

1. Identify and label entities as 'Person' or 'Institution'.
2. Determine the 'Job Relationship' between the entities.
3. Format your output as a triplet: (Entity1, Job Relationship, Entity2).

For example, if the text states 'Alice works at Quantum Corp', the extracted triplet would be: (Alice, works at, Quantum Corp).

To ensure the quality of your extraction, please:
- Clearly define entities and relationships.
- Extract each distinct job relationship separately.
- Infer relationships when not explicitly stated, using context for guidance.
- Exclude any information that is not relevant or lacks clarity.

Now, proceed with the text analysis and present a list of the extracted, well-defined triplets."




## newbing

Certainly! Let's refine the prompt to generate a more concise and relevant instruction for the large model. Here's an improved prompt:

---

"Extract knowledge graph triplets from the provided natural language text. Identify entities as either people or institutions and determine their job relationships. Follow these guidelines:

1. **Entity Types**: Person and Institution.
2. **Relationship Type**: Job or Position held.
3. **Triplet Format**: (Entity1, Relationship, Entity2).

For example, if the text mentions 'John Smith is the CEO of Moonshot AI,' the extracted triplet would be: (John Smith, is CEO of, Moonshot AI).

Ensure clarity, accuracy, and exclude irrelevant or incomplete information."

---

Feel free to use this prompt directly for the large model to perform the task. If you have any further requirements or need additional context, please let me know!


## chatglm6b-32k
Given the new context, the refined answer is as follows:

""" You are tasked with extracting knowledge graph triplets from the provided text. Please identify and categorize entities as either people or institutions and determine the job relationships between them. Your extracted triplets should include the following elements:

Entity Types: Person and Institution.
Relationship Type: Job or Position held.
Triplet Format: (Entity1, Relationship, Entity2).
In addition, please ensure that the extracted triplets are relevant to the context of the text and that they are accurate and clearly defined. If multiple job relationships are mentioned, extract each one separately. If the relationship is not explicitly stated or is ambiguous, infer the most likely type of relationship based on the context. If the text contains any irrelevant or incomplete information, exclude it from your extraction.

Please follow these guidelines while processing the text:

Ensure that the entities and relationships are clearly defined and accurate.
If multiple job relationships are mentioned, extract each one separately.
If the relationship is not explicitly stated or is ambiguous, infer the most likely type of relationship based on the context.
Exclude any irrelevant or incomplete information.
Please provide a list of the extracted triplets. """




## chatglm3
The refined answer considering the new context is as follows:
------------\n
"""
As an AI language model, I am capable of extracting knowledge graph triplets from natural language. I will identify entities as either people or institutions and determine the job relationships between them based on the provided text. The triplets will be in the format of (Entity1, Relationship, Entity2). Here's an example: If the text states "John Smith is the CEO of Moonshot AI," the triplet extracted would be: (John Smith, is CEO of, Moonshot AI).
I will adhere to the guidelines provided, ensuring clear and accurate definitions of entities and relationships. If multiple job relationships are mentioned, I will extract each one separately. In cases where the relationship is not explicitly stated or is ambiguous, I will infer the most likely type of relationship based on the context. I will exclude any irrelevant or incomplete information to ensure the quality and accuracy of the extracted triplets.
Please provide the text that needs to be processed, and I will generate a list of the extracted triplets accordingly.
"""
------------\n