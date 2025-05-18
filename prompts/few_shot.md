#  Few-Shot Prompt 

### What "Few-Shot" Means
Few-shot prompting involves showing the LLM one or more examples before asking it to perform a similar task. This helps the model learn the expected format or pattern.

#### When to Use Few-Shot Prompting:
- The task needs format guidance
- Output needs to be structured consistently
- You want the model to mimic your tone, role, or logic pattern



---

## 1. Summarization Example

**Prompt:**
Summarize the following customer support messages into a short sentence.

Example 1:  
Input: "I got double charged for my order and I want a refund!"  
Output: "Customer was double charged and is requesting a refund."

Example 2:  
Input: "I received the wrong color of the item I ordered."  
Output: "Customer received the wrong color item."

Now summarize:  
"I was told delivery would be 2 days, but it’s been a week and nothing has arrived."

**Model:** GPT-3.5  
**Output:**  
Customer reports a delayed delivery; item has not arrived after a promised 2-day timeframe.

---

## 2. Sentiment Classification

**Prompt:**
Label the following texts as Positive, Neutral, or Negative.

Example 1: "The product exceeded my expectations!" → Positive  
Example 2: "It's okay, not great but not bad." → Neutral  

Text: "This is the worst customer service I've ever had."

**Model:** GPT-3.5  
**Output:**  
Label: Negative

---

## 3. Code Description

**Prompt:**
Describe what each Python snippet does.

Example 1:
```
x = [1, 2, 3]
print(sum(x))
```
This prints the sum of the list, which is 6.

Example 2:
```
for i in range(3):
    print(i)
```
This prints numbers 0 through 2, one per line.

Now describe:
```
nums = [2, 4, 6]
print([n**2 for n in nums])
```

**Model:** GPT-4  
**Output:**  
This creates a new list containing the squares of each number in the nums list and prints it. The output will be [4, 16, 36].

---

## 4. Role-Based Rewrite

**Prompt:**
Rewrite casual texts as if written by a company’s customer support team.

Example 1:
"Hey, your product didn’t work. Fix this ASAP!"  
"Hello, I received a product that isn’t functioning correctly. Could you please assist?"

Example 2:
"Where’s my order? It’s late."  
"I’d like to check the status of my delayed order."

Now rewrite:
"Still no response about my refund. This is getting frustrating."

**Model:** GPT-4  
**Output:**  
I’m following up on my refund request, as I haven’t received a response yet. I’d appreciate any updates at your earliest convenience.

---

## 5. Structured Data Extraction

**Prompt:**
Extract Name, Email, and Date from the following messages.

Example 1:
"Hi, this is John Doe. You can reach me at john@example.com. Let’s meet on Friday."
→ Name: John Doe, Email: john@example.com, Date: Friday

Now extract:
"Hello, I’m Sita Malhotra, my email is sita@domain.com. Let's connect on Monday."

**Model:** GPT-3.5  
**Output:**  
```
Name: Sita Malhotra
Email: sita@domain.com
Date: Monday
```

---
