# Fine-Tuning Qwen2.5-1.5B-Instruct for Arabic News Tasks

This project fine-tunes **Qwen2.5-1.5B-Instruct** using **LoRA** to perform two tasks on Arabic news articles:

1. **Extract structured details**  
   - Title  
   - Keywords  
   - Summary points  
   - Category  
   - Named entities  
   (All following a Pydantic JSON schema)

2. **Translate Arabic news to English**  
   - Translated title  
   - Translated content  
   (Also using a Pydantic JSON schema)

The main goal is to improve the model’s ability to follow strict instructions and generate valid structured JSON outputs.

---

## 🚀 Features

•	Fine-tuned Qwen2.5-1.5B-Instruct using LoRA on a custom dataset (2.7k samples) for structured Arabic news parsing and Arabic→English translation.
•	Built an end-to-end NLP pipeline: dataset construction, Pydantic JSON schemas, instruction formatting, supervised fine-tuning, and model evaluation.
•	Served the fine-tuned LoRA adapter with vLLM for fast inference and consistent JSON-structured outputs.
•	Implemented robust JSON generation using schema-guided prompts, error handling, and output validation.


---

## 🎯 Use Cases

- Structured metadata extraction for news
- Arabic → English translation
- JSON-based NLP pipelines

