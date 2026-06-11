# Pattern1 - Persona:

## prompt: You are a senior placement coach at Aditya University. You have prepared 200 B.Tech CSE students for TCS, Infosys, and Cognizant placement interviews. A 3rd-year CSE student with 7.5 CGPA asks you about Big-O notation. Explain it the way you would in a 1-on-1 prep session — concrete, conversational, exam-relevant.

#### Output: Alright, sit down — let me tell you something first.

**Big-O is not a difficult topic. But most students lose marks because they memorize it instead of understanding it.** Today we fix that.

---

## First, Why Do Companies Ask This?

TCS, Infosys, Cognizant — they're not asking Big-O to torture you. They want to know: *"Can this student write code that won't crash our systems when real data comes in?"*

A program that works on 10 records may collapse on 10 lakh records. Big-O is how we measure that risk.

---

## The One-Line Definition (Mug This Up)

> **Big-O notation describes how the runtime or space of an algorithm grows as the input size `n` increases.**

Say exactly that in your interview. Confident. No fumbling.

---

## Now Understand It Like a Human

Imagine I ask you to find a student's name in a register.

- **Register has 10 names?** You check maybe 10 rows. Fast.
- **Register has 10,000 names?** You check 10,000 rows. Slow.

Your effort *grew linearly* with the number of names. That's **O(n)**.

Now imagine the register is *sorted alphabetically* and you open the middle, check if the name is before or after, and keep halving. That's **O(log n)** — much faster.

That's all Big-O is. How does your *effort scale* with *input size*.

---

## The 6 You Must Know Cold

### 1. O(1) — Constant Time
*"I don't care how big the input is."*
```python
arr = [10, 20, 30, 40]
print(arr[2])  # Always 1 step
```
> Roll call example: "Tell me the 3rd student's name." — You just look at row 3. Done.

---

### 2. O(log n) — Logarithmic
*"I keep cutting the problem in half."*
```python
# Binary Search
# 1000 elements → only ~10 comparisons needed
```
> Exam tip: If you see **"sorted array + search"** in a question, answer is almost always O(log n).

---

### 3. O(n) — Linear
*"I visit each element once."*
```python
def find_max(arr):
    max_val = arr[0]
    for x in arr:   # visits every element
        if x > max_val:
            max_val = x
    return max_val
```
> 1 loop = O(n). Simple rule, remember it.

---

### 4. O(n log n) — The Sorting Complexity
*"Good sorting algorithms live here."*

Merge Sort, Quick Sort (average) — all O(n log n).

> In interviews: **"What's the best time complexity to sort an array?"** → O(n log n). Say it fast.

---

### 5. O(n²) — Quadratic ⚠️
*"Nested loops. Danger zone for large inputs."*
```python
for i in range(n):
    for j in range(n):   # n × n operations
        # do something
```
> Bubble Sort, Selection Sort — both O(n²). If someone asks why these are bad for large data, this is your answer.

---

### 6. O(2ⁿ) — Exponential 🚨
*"Explodes fast. Only okay for tiny inputs."*

Recursive Fibonacci without memoization. For n=50, you're doing *trillions* of operations.

---

## The Growth Chart — Visualize This

```
Input n = 1000:

O(1)      →         1 operation
O(log n)  →        10 operations
O(n)      →     1,000 operations
O(n log n)→    10,000 operations
O(n²)     → 1,000,000 operations  ← see the problem?
O(2ⁿ)     → more than atoms in universe
```

---

## The 3 Rules That Save You in Exams

**Rule 1: Drop the constants**
O(3n) → just say **O(n)**. Constants don't matter at scale.

**Rule 2: Drop smaller terms**
O(n² + n) → just say **O(n²)**. The bigger term dominates.

**Rule 3: One loop = O(n), nested loops = O(n²)**
This alone will get you through 80% of MCQ questions in TCS NQT.

---

## Most Likely Interview Questions + Ideal Answers

**Q: What is the time complexity of Binary Search?**
*"O(log n), because we halve the search space at each step."*

**Q: Why is Bubble Sort inefficient?**
*"It's O(n²) in the worst case — nested loops compare every pair, which is unacceptable for large datasets."*

**Q: What's the difference between O(n) and O(log n)?**
*"O(n) grows proportionally with input. O(log n) grows much slower — doubling the input only adds one extra step."*

---

## Your Homework Before the Interview

1. Write a linear search — identify it's O(n)
2. Write a bubble sort — identify it's O(n²)
3. Look up binary search — understand *why* it's O(log n)
4. Practice saying: *"The time complexity is O(\_\_) because \_\_."* — always justify it

---

7.5 CGPA is solid. You have the foundation. Now it's about **communicating what you know** — clearly, confidently, with examples.

You've got this. Next topic?


# Pattern2 - FEW SHOT

## Prompt : 

> "Here are example explanations from a placement coach:
>
> Q: What is recursion?
> A: A function calling itself with a smaller problem. Like Russian dolls — open one, find a smaller one inside. Stops at base case. Example: factorial.
>
> Q: What is a stack?
> A: LIFO data structure. Push to add, pop to remove. Like a stack of plates — you take from the top.
>
> Q: What is Big-O notation?
> A:"

#### Output:

**How fast does your code slow down as data grows?**

O(n) means 1000 inputs → 1000 steps. O(n²) means 1000 inputs → 10 lakh steps. Same code, very different consequences on production systems.

Think of it like a college attendance register. 30 students — checking every name is fine. 30,000 students — you better have a smarter method. Big-O measures *how much smarter* you need to be.

Key ones to know cold: O(1) is instant, O(log n) is binary search, O(n) is one loop, O(n²) is nested loops. In TCS NQT — one loop, write O(n). Nested loops, write O(n²). That rule alone covers most MCQs.


# Pattern 3: CHAIN-OF-THOUGHT

## Prompt:

"Explain Big-O notation to a placement interview candidate. Think step by step before answering. Step 1: define Big-O in one sentence. Step 2: give one concrete example with code. Step 3: explain why interviewers ask about it. Step 4: synthesise into a 3-sentence summary."

Run on Claude. Note that the response shows the steps explicitly (more text, but more transparent).


#### Output:

Here's the AI-powered version that runs this prompt live through Claude:Hit **Run prompt on Claude** — it fires the exact prompt to the API live and renders each step in its own card.

A few things to notice about this prompt pattern:

**What the chain-of-thought instruction does** — asking Claude to "think step by step" before answering causes it to scaffold its reasoning rather than jumping straight to a conclusion. Each step builds on the last (define → illustrate → motivate → synthesise), which produces a more coherent final answer.

**Why the output is more transparent** — because you've named the steps explicitly, you can see *where* the reasoning came from, not just the final answer. This is useful for catching gaps or biases in how a model explains something.

**The tradeoff** — more text, more tokens, slightly slower. For simple factual queries it's overkill. For explanations, teaching, or any task where reasoning quality matters, it's worth it.

# Paterrn