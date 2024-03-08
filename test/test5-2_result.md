
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