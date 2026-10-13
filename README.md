# Experiment 10: Chain-of-Thought Prompting for Math Reasoning

## Aim
To demonstrate and compare direct prompting and Chain-of-Thought (CoT) prompting for solving a multi-step mathematical word problem using a Large Language Model (LLM).

## Problem Statement
A farmer has 15 cows. He buys 7 more cows. Then he sells half of his cows. How many cows does he have left?

## Tools and Technologies
- Python
- Google Gemini API
- Google Gen AI SDK
- Regular expressions for answer extraction

## Algorithm
1. Define the mathematical word problem.
2. Create a direct prompt containing the problem.
3. Create a CoT prompt by appending “Let's think step by step. Show each step.”
4. Send both prompts to the same LLM with temperature set to 0.
5. Extract the final numeric answer from each response.
6. Compare the extracted answers with the expected answer, 11.
7. Save the responses and comparison results.

## Expected Calculation
- Initial cows: 15
- After buying 7 cows: 15 + 7 = 22
- After selling half: 22 ÷ 2 = 11
- Final answer: 11 cows

## Output
The program displays both LLM responses and compares their extracted answers against the expected answer. The execution results are saved in `output.txt`.

## Conclusion
This experiment compares direct prompting with Chain-of-Thought prompting on a multi-step arithmetic task. CoT can make intermediate calculations more explicit and easier to inspect, but it does not guarantee a correct answer. The actual results should be recorded from the model execution.
