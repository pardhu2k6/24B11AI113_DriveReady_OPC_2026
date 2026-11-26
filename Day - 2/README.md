# Day 2 – Agentic AI Workshop

## Sweet Crumbs Home Bakery

### Overview

This assignment builds on Day 1 LLM fundamentals by exploring prompt engineering, few-shot classification, structured JSON output, conversation memory, and Python business functions.

### Technology Stack

- Python
- Google Colab
- Groq API
- GPT-OSS-120B (`openai/gpt-oss-120b`)
- OpenAI Python SDK

### Practical Tasks

| Task | Concept | Description |
|---|---|---|
| 1 | Prompt Parts | Compare responses to a one-hour delivery request with and without system prompt rules. |
| 2 | Few-shot Prompting | Use three examples to classify five new customer messages as order, question, or complaint. |
| 3 | JSON | Extract name, item, qty, date, and eggless from a customer order and parse the response using `json.loads()` with `try/except`. |
| 4 | Memory | Set `MAX_TURNS = 2` and observe how limiting conversation history affects name recall. |
| 5 | Business System Prompt | Create a bakery menu dictionary, a price calculation function with a docstring, and a dedicated system prompt. |

### Learning Outcomes

- Understand the importance of roles, facts, rules, and response formats.
- Apply few-shot prompting to customer intent classification.
- Convert unstructured messages into structured JSON data.
- Understand limited conversation memory.
- Use Python dictionaries and functions to represent business information.
- Handle API and JSON parsing errors.

### Execution

1. Open the Day 2 notebook in Google Colab.
2. Add `GROQ_API_KEY` to Colab Secrets and enable notebook access.
3. Run the setup cells and execute all five tasks in order.
4. Review the actual outputs and compare model behaviour.

Never commit API keys to GitHub.

### Preparation for Day 3

- Reuse the ten customer FAQs prepared on Day 1.
- Prepare the bakery catalogue as a Python dictionary.
- Get ready to explore agent loops and LangChain.

### Conclusion

Day 2 establishes the foundation for building a business-specific chatbot with structured responses, limited conversation memory, and Python functions. These concepts prepare the chatbot for agent-based workflows and future tool calling.
