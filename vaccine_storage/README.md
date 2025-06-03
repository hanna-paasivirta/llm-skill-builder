# Prompt Engineering & Task Decomposition Practice
This is a practice exercise for working with LLMs. The `data_exploration.ipynb` notebook provides a starting point for the task.

## Task description

Use an LLM to identify vaccine batches stored at inappropriate temperatures.

**Data sources:**

Storage temperature requirements: `who_audit_summary_synthetic.md`
Temperature data: `who_audit_synthetic_data.csv`

**Key points**: The dataset contains misleading information in some columns. You should identify the temperature range columns for batches that show the lowest and the highest temperature for that batch.

**Target:** Find the 3 batches stored inappropriately:

B10046 (2025-02-14 8:00:00)  
B10048 (2025-02-16 16:00:00)  
B10001 (2025-01-01 8:00:00)  

**Your task**: Develop a prompting strategy that gets the LLM to correctly identify these batches. 

See `data_exploration.ipynb` for an example. You will need to break the task down into steps instead of relying on a single prompt. 

Using a larger LLM will make the task easier, and using a small one will make it more challenging.

If you can get to the answer, consider the reliablity of the methods you used. Would they be appropriate for using in a real project? Are there risks, or other methods that could be more reliable?