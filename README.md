# Palindromic-Ranges
DSA in python
Sure! Let's break the problem down into simpler terms:

### Palindromes:
- A **palindrome** is a number that reads the same forwards and backwards. For example, 121 is a palindrome because if you reverse it, it’s still 121. Similarly, 77 and 363 are palindromes. Non-palindromes, like 123, do not read the same backwards.

### Range:
- You are given a range of numbers from \(L\) to \(R\) (both included). For example, if \(L = 1\) and \(R = 7\), the range is \([1, 2, 3, 4, 5, 6, 7]\).

### Subranges:
- A **subrange** is just a smaller part of the main range. For instance, if the main range is \([1, 7]\), then \([2, 4]\) or \([5, 6]\) are examples of subranges.

### Interesting Subrange:
- A **subrange** is called "interesting" if it has **an even number of palindromes**.
  - For example, in the subrange \([1, 2]\), there’s only one palindrome (1), so this subrange is not interesting.
  - In the subrange \([1, 4]\), there are two palindromes (1 and 2), so this subrange is interesting because the number of palindromes is even (2).

### Problem:
- You are asked to find **how many interesting subranges** exist in the range \([L, R]\). 

### Example:
- If \(L = 1\) and \(R = 7\), the range is \([1, 2, 3, 4, 5, 6, 7]\). You need to check all possible subranges (like \([1, 2]\), \([1, 3]\), \([2, 5]\), etc.) and count how many of them have an even number of palindromes.

Let's dive deeper into **what makes a subrange "interesting."**

### What is an Interesting Subrange?

A subrange of numbers is called **"interesting"** if it contains an **even number** of palindromes. 

### Recap on Palindromes:
- A palindrome is a number that reads the same forwards and backwards, like 121, 77, or 5.
  
### Example:

Consider the range \( [1, 7] \), i.e., the sequence of numbers:  
\[ [1, 2, 3, 4, 5, 6, 7] \]

The palindromes in this range are **1, 2, 3, 4, 5, 6, and 7**. Every number here is actually a palindrome because each number reads the same forwards and backwards.

Now, let's look at how subranges can be "interesting."

### Example 1: Subrange [1, 2]
The numbers in this subrange are:  
\[ [1, 2] \]

- Palindromes: 1, 2 (both are palindromes).
- The count of palindromes = 2.

Since the number of palindromes is **even** (2), this subrange is **interesting**.

### Example 2: Subrange [1, 3]
The numbers in this subrange are:  
\[ [1, 2, 3] \]

- Palindromes: 1, 2, 3 (all are palindromes).
- The count of palindromes = 3.

Since the number of palindromes is **odd** (3), this subrange is **not interesting**.

### Example 3: Subrange [2, 4]
The numbers in this subrange are:  
\[ [2, 3, 4] \]

- Palindromes: 2, 3, 4 (all are palindromes).
- The count of palindromes = 3.

Again, the number of palindromes is **odd** (3), so this subrange is **not interesting**.

### Example 4: Subrange [1, 4]
The numbers in this subrange are:  
\[ [1, 2, 3, 4] \]

- Palindromes: 1, 2, 3, 4 (all are palindromes).
- The count of palindromes = 4.

Since the number of palindromes is **even** (4), this subrange is **interesting**.

### Example 5: Subrange [3, 5]
The numbers in this subrange are:  
\[ [3, 4, 5] \]

- Palindromes: 3, 4, 5 (all are palindromes).
- The count of palindromes = 3.

Since the number of palindromes is **odd** (3), this subrange is **not interesting**.

---

### Key Takeaways:
- **An "interesting" subrange** is one where the number of palindromes is **even**.
- Any subrange can be "interesting" if the palindromes inside that subrange add up to an even number.

In summary:
- The subrange \([1, 2]\) is interesting because it has 2 palindromes (even number).
- The subrange \([1, 3]\) is not interesting because it has 3 palindromes (odd number).
- The subrange \([1, 4]\) is interesting because it has 4 palindromes (even number).

The task is to count how many of these "interesting" subranges exist in the range you are given.
