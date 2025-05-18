
#  Chain-of-Thought (CoT) Prompt

CoT prompts encourage the LLM to “think step by step” before answering. This improves accuracy in tasks requiring reasoning or logic.

Each example below includes:
- A CoT-style prompt
- The model used
- Output and interpretation (optional)

---

## 1. Simple Math Word Problem

**Prompt:**
Q: If there are 12 bananas and 4 people, and each person eats 2 bananas, how many bananas are left?

**Chain of Thought:**
- Step 1: Each of the 4 people eats 2 bananas → 4 x 2 = 8 bananas eaten
- Step 2: Start with 12 bananas : 12 - 8 = 4
- A: 4 bananas left

**Model:** GPT-3.5  
**Output:** 
There are 4 bananas left.

---

## 2. Logical Planning

**Prompt:**
You have to attend 3 meetings: one at 9 AM, one at 11 AM, and one at 2 PM. It takes 30 minutes to commute to your office. What’s the latest you can leave home?

**Chain of Thought:**
- First meeting starts at 9 AM
- You need to reach by 9 AM, and it takes 30 minutes to commute
- So you must leave home by 8:30 AM

**Model:** GPT-4  
**Output:** 
The latest you can leave home is 8:30 AM

---

## 3. Multi-step Unit Conversion

**Prompt:**
Convert 120 minutes into days.

**Chain of Thought:**
- 60 minutes = 1 hour → 120 minutes = 2 hours
- 24 hours = 1 day → 2 hours = 2 / 24 = 0.083 days

**A:** 0.083 days

**Model:** GPT-3.5  
**Output:** 
120 minutes is equal to 0.083 days.

---

## 4. Deductive Reasoning

**Prompt:**
John is taller than Alice. Alice is taller than Bob. Who is the shortest?

**Chain of Thought:**
- John > Alice > Bob
- Therefore, Bob is the shortest.

**Model:** GPT-3.5  
**Output:** 
Bob is the shortest.

---

## 5. Debugging

**Prompt:**
What’s wrong with this code and how can we fix it?
```python
def greet():
print("Hello, world!")
```

**Chain of Thought:**
- The function is missing an indentation
- Python requires indentation for function bodies
- Fix: add 4 spaces before the print statement

**Fixed Code:**
```python
def greet():
    print("Hello, world!")
```

**Model:** GPT-4  
**Output:** 
The issue with the code is that the print statement is not indented inside the function. In Python, the body of a function must be indented. Here's the corrected version:

---
