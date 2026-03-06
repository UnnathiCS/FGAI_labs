

# 1. Zero-Shot Prompting

**Definition:**
The model is given **no examples** and must perform the task directly.

**Example Prompt**

```
Classify the sentiment of the sentence as Positive, Negative, or Neutral.

Sentence: "The movie was amazing and very entertaining."
```

**Expected Output**

```
Positive
```

**Key Idea**

* No training examples are provided.
* The model relies on **pretrained knowledge**.

---

# 2. One-Shot Prompting

**Definition:**
The model is given **one example** before the task.

**Example Prompt**

```
Classify the sentiment.

Example:
Sentence: "I hate waiting in long lines."
Sentiment: Negative

Now classify:
Sentence: "The service was excellent and fast."
```

**Expected Output**

```
Positive
```

**Key Idea**

* One example helps the model understand the **expected format**.

---

# 3. Few-Shot Prompting

**Definition:**
The model is given **multiple examples** to learn the pattern.

**Example Prompt**

```
Classify the sentiment.

Sentence: "The food was delicious."
Sentiment: Positive

Sentence: "The app keeps crashing."
Sentiment: Negative

Sentence: "The delivery was quick."
Sentiment: Positive

Sentence: "The product stopped working in a day."
Sentiment:
```

**Expected Output**

```
Negative
```

**Key Idea**

* Multiple examples improve **accuracy and consistency**.

---

# 4. Chain-of-Thought Prompting

**Definition:**
The model is encouraged to **reason step-by-step** before answering.

**Example Prompt**

```
Q: If a class has 30 students and 12 are girls, how many are boys?
Let's think step by step.
```

**Expected Output**

```
Total students = 30
Girls = 12
Boys = 30 - 12 = 18

Answer: 18
```

**Key Idea**

* Improves **reasoning for math, logic, and problem solving**.

---

# 5. Tabular Format Prompting

**Definition:**
The output is structured in **table format** for clarity.

**Example Prompt**

```
List 3 programming languages with their primary use and year created in a table.
```

**Expected Output**

| Language | Primary Use             | Year Created |
| -------- | ----------------------- | ------------ |
| Python   | AI / Data Science       | 1991         |
| Java     | Enterprise Applications | 1995         |
| C++      | System Programming      | 1985         |

**Key Idea**

* Useful for **structured data generation**.

---

# 6. Fill-in-the-Blank Prompting

**Definition:**
The model completes the **missing information**.

**Example Prompt**

```
Fill in the blank:

The capital of France is ______.
```

**Expected Output**

```
Paris
```

**Key Idea**

* Often used in **educational or quiz systems**.

---

# 7. RGC Prompting (Role-Goal-Context)

**Definition:**
The prompt specifies **Role, Goal, and Context** to guide the model.

**Example Prompt**

```
Role: You are a cybersecurity expert.
Goal: Explain phishing attacks.
Context: The explanation is for beginner college students.

Explain phishing attacks in simple terms.
```

**Expected Output (Example)**

```
Phishing is a cyber attack where attackers trick users into revealing sensitive
information like passwords or credit card details by pretending to be a
trusted organization through emails or fake websites.
```

**Key Idea**

* Improves **relevance and tone** of responses.

---

# Quick Comparison

| Prompting Technique | Key Idea               | Example Use           |
| ------------------- | ---------------------- | --------------------- |
| Zero-Shot           | No examples            | Quick tasks           |
| One-Shot            | One example            | Formatting guidance   |
| Few-Shot            | Multiple examples      | Better accuracy       |
| Chain-of-Thought    | Step-by-step reasoning | Math / logic          |
| Tabular Format      | Structured output      | Reports / comparisons |
| Fill-in-the-Blank   | Complete missing info  | Education             |
| RGC                 | Role + Goal + Context  | Controlled responses  |

