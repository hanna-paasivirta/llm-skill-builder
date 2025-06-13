# Prompt Engineering & Task Decomposition Practice
This is a practice exercise for working with LLMs. The `data_exploration.ipynb` notebook provides a starting point for the task.

## Task description

Use an LLM to identify vaccine batches stored at inappropriate temperatures.

## Data

Storage temperature requirements: `who_audit_summary_synthetic.md`  
Temperature data: `who_audit_synthetic_data.csv`  

**Key points**: The dataset contains misleading information in some columns. You should identify the temperature range columns for batches that show the lowest and the highest temperature for that batch.

## Task details
**Develop a prompting strategy that can get the LLM to correctly identify the vaccine batches that have been stored at inappropriate temperatures.**  

**Target:** There are 3 batches that have been stored inappropriately:

B10046 (2025-02-14 8:00:00)  
B10048 (2025-02-16 16:00:00)  
B10001 (2025-01-01 8:00:00)  

See `data_exploration.ipynb` for an example. You will need to break the task down into steps instead of relying on a single prompt. 

Using a larger LLM will make the task easier, and using a small one will make it more challenging.


## Questions

I suggest you note down your answers for these questions, then chat with an LLM, me or a friend to review your answer and consider other possible perspectives.  

1. What are some prompts that you tried that didn't help get the correct answer from the LLM? What are your working theories about why they didn't work?  

2. If you try solving the task on a chat UI (like claude.ai), you might find that the model IS able to get to the answer (try it out!). But when you use the same LLM in your code in the Jupyter Notebook (e.g. Claude Sonnet 4), it can't find the correct answer. Why could this be?  

3. Can you think of prompts that help you get closer to the correct answer? (Hint: you could try identifying separate, simple tasks within the overall complex task)  

4. Reflect on the approaches you have used to prompt the LLM:
a) What risks would there be in relying on an LLM if we were dealing with a real-life vaccine storage problem?  
b) Would there be ways to leverage an LLM safely in a real-life version of the vaccine storage problem?  
c) Do you think we could use an LLM in this scenario in such a way that the benefits would outweigh the risks?  