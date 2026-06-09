# Task1
## Score Table

| Tool       | Faithfulness | Brevity     | Rule Compliance             | Score (/5) |
| ---------- | ------------ | ----------- | --------------------------- | ---------- |
| ChatGPT    | Good         | Excellent   | Follows 15-word limit       | **4.5/5**  |
| Claude     | Very Good    | Mostly good | One bullet slightly long    | **4.5/5**  |
| Gemini     | Good         | Excellent   | Adds less specific detail   | **4/5**    |
| Perplexity | Excellent    | Good        | Some bullets close to limit | **5/5**    |

- Perplexity is best for summarization because it preserves the most important points while staying concise.

# Task2

## Score Table

| Tool           | Score   | Correctness                                                              | Readability                                          | Constraint Adherence                                           |
| -------------- | ------- | ------------------------------------------------------------------------ | ---------------------------------------------------- | -------------------------------------------------------------- |
| **ChatGPT**    | **5/5** | Function works correctly and returns the required output shape.          | Clean naming, concise logic, docstring included.     | Uses only the standard library and follows all requirements.   |
| **Claude**     | **4/5** | Handles edge cases and provides a robust scoring approach.               | Very well documented, but somewhat over-engineered.  | Uses only the standard library and meets requirements.         |
| **Gemini**     | **4/5** | Works correctly on test cases but uses a simpler matching strategy.      | Readable and concise with a clear docstring.         | Uses only the standard library and returns the correct format. |
| **Perplexity** | **5/5** | Works correctly, handles edge cases, and identifies missing skills well. | Clear structure, good docstring, easy to understand. | Fully complies with the standard-library-only requirement.     |

- ChatGPT is best for coding because it provides the cleanest, most readable solution while fully satisfying the prompt requirements.

# Task3

## Score Table

| Tool           | Score   | Accuracy                                    | Transparency                       | Confidence Calibration  |
| -------------- | ------- | ------------------------------------------- | ---------------------------------- | ----------------------- |
| **ChatGPT**    | **5/5** | Correct answer (8:10 AM, 20 minutes early). | Every step shown explicitly.       | Appropriate confidence. |
| **Claude**     | **5/5** | Correct answer (8:10 AM, 20 minutes early). | Clear step-by-step reasoning.      | Appropriate confidence. |
| **Gemini**     | **5/5** | Correct answer (8:10 AM, 20 minutes early). | All calculations shown explicitly. | Appropriate confidence. |
| **Perplexity** | **5/5** | Correct answer (8:10 AM, 20 minutes early). | Every step shown explicitly.       | Appropriate confidence. |

- All four tools solved the reasoning task correctly. Claude provided the clearest and most transparent explanation, making it my preferred tool for reasoning-heavy tasks.


| Tool           | Task 1 (Summarise) | Task 2 (Code) | Task 3 (Reason) | My Verdict                                                                                |
| -------------- | ------------------ | ------------- | --------------- | ----------------------------------------------------------------------------------------- |
| **ChatGPT**    | **4.5**            | **5**         | **5**           | *Best all-rounder. Produces clean summaries, readable code, and reliable reasoning.*      |
| **Claude**     | **4.5**            | **4**         | **5**           | *Best for detailed writing and transparent step-by-step reasoning. Can be verbose.*       |
| **Gemini**     | **4**              | **4**         | **5**           | *Good for concise responses and factual information. Less sophisticated coding approach.* |
| **Perplexity** | **5**              | **5**         | **5**           | *Best for research-oriented tasks, source-backed summaries, and strong coding solutions.* |


Perplexity — Highest overall score; strongest for summarization, fact verification, and research.
ChatGPT — Best all-rounder; strongest balance of usability, coding, and reasoning.
Claude — Best for transparent explanations, long-form writing, and careful reasoning.
Gemini — Good general-purpose assistant, but less distinguished in this evaluation.