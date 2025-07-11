
# Grading Criteria for LeftoversGPT Evaluation

This file documents the custom grading logic used during model evaluation for LeftoversGPT.

## 1. Sentiment Classification (sentiment-classification-model-grader)
**Goal**: Ensure the assistant’s tone is friendly, helpful, and non-judgmental.

- **Positive Grade**: 1 (Tone is warm, encouraging, and supportive)
- **Neutral/Negative/Unsure Grade**: 0 (Tone is flat, rude, dismissive, or inappropriate)

---

## 2. Prompt Adherence (chat-criteria-model-grader)
**Goal**: Check if the output followed the system prompt instructions.

- **True Grade**: 1 (Output is crisp and conversational, aligns with guidance)
- **False Grade**: 0 (Verbose, robotic, or unhelpful)

Custom Criteria: "The response should be crisp and conversational"

---

## 3. Response Similarity (discrete-classification-model-grader)
**Goal**: Evaluate how closely the model’s output matched the expected behavior or answer.

Prompt Template:
```
Measure the degree of similarity between output and ground truth on a scale of 1-5. Only output a single integer in your response.

Output: {{item.Input Query}}
Ground Truth: {{item.Input Query}}
```

Grading Mapping:
- 1 or 2: Grade 0 (Low relevance)
- 3, 4, or 5: Grade 1 (Sufficiently aligned)

---

## Evaluation Notes
- A test case passes if it receives a Grade = 1 on all relevant graders
- Model used: `gpt-4o-mini`
- Grading executed via OpenAI Eval framework
