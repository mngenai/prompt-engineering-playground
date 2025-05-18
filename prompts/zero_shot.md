# Zero shot prompt

### What "Zero-Shot" Means

- "Zero-shot" means the model is expected to handle the task based only on the instructions, not by learning from examples within the prompt.

- It relies purely on the model’s pre-trained knowledge.



# 🧠 Zero-Shot Prompt Examples

This file contains examples of zero-shot prompts — where we ask the LLM to perform a task without giving it any prior examples.

Each section contains:
- The prompt used
- The model (e.g., GPT-3.5)
- The LLM output (optional placeholder)
- Notes on the prompt’s effectiveness

---

## 1. Text Summarization

**Prompt:**
Summarize the following paragraph in 1-2 sentences:

"Large language models (LLMs) are AI systems trained on massive text corpora. They are capable of answering questions, summarizing information, translating languages, and more."

**Model:** GPT-3.5  
**Output:**  
AI builds systems that mimic intelligent behavior.

---

## 2. Tone Transformation

**Prompt:**
Rewrite the following email to sound more professional:

"Hey, I can’t make the meeting. Let’s talk later."

**Model:** GPT-4  
**Output:**  
"I won’t be able to attend the meeting. Let’s reschedule."

---

## 3. Explain Like I’m 5

**Prompt:**
Explain quantum entanglement like I'm 5 years old.

**Model:** GPT-4  
**Output:**  
"Imagine two magic dice that always show the same number..."

---

## 4. SQL Generation

**Prompt:**
Convert this request into SQL:
"List all customers from Germany who have placed more than 3 orders in the last month."

**Model:** GPT-3.5  
**Output:**  
```
SELECT * FROM customers
WHERE country = 'Germany'
AND customer_id IN (
  SELECT customer_id FROM orders
  WHERE order_date >= DATE_SUB(CURDATE(), INTERVAL 1 MONTH)
  GROUP BY customer_id
  HAVING COUNT(order_id) > 3
);
```

---

## 5. Classification Prompt

**Prompt:**
Classify the following text as either "Positive", "Neutral", or "Negative":
"I just got the new phone. It's okay, but not much different from the old one."

**Model:** GPT-3.5  
**Output:**  
(Your output here)

---

## 6. Data Extraction Prompt

**Prompt:**
Extract the person's name, email address, and phone number from this message:
"Hi, I'm Priya Sharma. You can reach me at priya@gmail.com or call me at +91-9876543210."

**Model:** GPT-3.5  
**Output:**  
```
Name: Priya Sharma

Email: priya@gmail.com

Phone: +91-9876543210
```

---

## 7. Code Explanation

**Prompt:**
Explain what the following Python code does in simple terms:
```
for i in range(10):
    if i % 2 == 0:
        print(i)
```

**Model:** GPT-4  
**Output:**  
Prints even numbers from 0 to 9.

---

## 8. Regex Generation

**Prompt:**
Write a regular expression to match all email addresses in a text.

**Model:** GPT-3.5  
**Output:**  
```
\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b
```

---

## 9. Creative Prompt

**Prompt:**
Write a short poem about the ocean in the style of Shakespeare.

**Model:** GPT-4  
**Output:**  
(Your output here)

---
