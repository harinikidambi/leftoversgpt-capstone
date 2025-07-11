# 🥕 LeftoversGPT: AI Product Management Capstone Project

This project is part of my AI Product Management certification, led by Miqdad Jaffer (Product Lead, OpenAI). The goal was to build an AI-powered assistant to reduce food waste by helping users turn leftover ingredients into personalized, creative meals.

**LeftoversGPT** uses LLMs to:
- Interpret ingredients from text or images
- Generate recipes tailored to dietary needs, cooking skills, and preferences
- Offer substitutions, cooking guidance, and sustainability tips

---

## 📄 Project Files

| File / Folder | Description |
|---------------|-------------|
| `[Harini] Capstone Submission 1 - Product Faculty AI Product Certification` | Full product requirements document (problem framing, journey map, MVP scope, LLM application, etc.) |
| `AI Capstone Project - Evaluation Questions` | Golden dataset (input-output pairs) for evaluation |
| `LeftoversGPT Evaluation Summary` | Screenshot of model evaluation summary showing grader config and pass rates |
| `eval_items_OutputDataItemStatusParam.ALL_2025-07-11_04-21-24.jsonl` | Raw results from 65 evaluation test cases with grading by custom OpenAI model graders |
| `README.md` | You're here :) |

---

## 🔬 Evaluation Summary

We evaluated the assistant using OpenAI’s structured evaluation framework with custom graders for:
- **Sentiment tone** (friendly, helpful)
- **Prompt adherence** (did the model follow instructions?)
- **Output quality** (did it generate a useful, relevant response?)

**Model used**: `gpt-4o-mini`  
**Test cases**: 65  
**Results**:
- ✅ 100% pass on tone and instruction-following
- ✅ 95% pass on overall output quality

---

## 📌 Highlights

- 🔁 Each test is defined as a single JSON object (JSONL format)
- 🧠 Graders applied: `sentiment-classification`, `chat-criteria-model-grader`, `discrete-classification-model-grader`
- 🧪 Includes both successful and edge-case interactions
- 👩🏽‍🍳 Dataset reflects real-world inputs like dietary substitutions, image input ambiguity, and kid-friendly constraints

---

## 💡 How to Use This Repo

If you're building or evaluating AI assistants, feel free to:
- Explore the PRD for structured thinking around user needs and LLM application
- Reuse the evaluation framework and JSONL format
- Fork the repo and adapt the test set to your domain

---

## 📬 Questions or Collaboration

Happy to chat! You can reach me via [LinkedIn](https://linkedin.com/in/harinikidambi) or raise an issue in this repo.

---

© 2025 Harini Kidambi Sekar
