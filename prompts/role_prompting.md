
# Role-Based Prompting 

Role-based prompts guide the LLM to respond in a specific tone, style, or domain context by assigning it a "persona" or professional identity.


---

## 1. Software Engineer Reviewer

**Prompt:**
You are a senior Python developer. Review this function and suggest improvements.
```python
def multiply(a, b):
return a * b
```

**Model:** GPT-4  
**Output:**  
The function is syntactically correct and functionally simple, but there are a few areas for improvement depending on context...

---

## 2. Customer Support Agent

**Prompt:**
Act as a customer support representative for an e-commerce company. Respond to this message:
"I received the wrong item in my order. What now?"

**Model:** GPT-3.5  
**Output:**  
I'm really sorry to hear that you received the wrong item! We're here to help make it right.

Please reply with your order number and a photo of the item you received, and we’ll get started on resolving this for you. Once we have that information, we can either send you the correct item or arrange a return if needed.

Thank you for your patience, and again, we apologize for the inconvenience.

---

## 3. HR Manager for Resume Advice

**Prompt:**
You are an HR manager. Rewrite this resume bullet point to make it more impactful:
"Managed a team of developers."

**Model:** GPT-4  
**Output:**  
Led a cross-functional team of 6 software developers, driving project delivery, enhancing team productivity by 25%, and ensuring adherence to Agile best practices.



---

## 4. Language Teacher

**Prompt:**
Act as an English teacher. Correct the grammar in the following sentence and explain the correction:
"He go to the market every Sunday."

**Model:** GPT-3.5  
**Output:**  
The subject "he" is third person singular, so the verb should be conjugated accordingly. In the present simple tense, most verbs take an “-s” at the end when used with "he," "she," or "it." Therefore, "go" becomes "goes."

---

## 5. Career Coach

**Prompt:**
You are a career coach. Give advice on how to answer this interview question:
"What’s your biggest weakness?"

**Model:** GPT-4  
**Output:**  
When answering this question, choose a real weakness—something genuine but not critical to the role—and focus on how you’re actively working to improve it. The goal is to demonstrate self-awareness, accountability, and a growth mindset...

---
