[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/cm6PS4yt)
# Week 1 Homework: Evidence Desk Patterns
## Student Name

Anu Dumjan

## Summary

This homework asks us to practice several important data structure patterns that are commonly used in Python programming. The assignment focuses on counting frequencies with dictionaries, detecting duplicates using sets, validating matching tags with stacks, and performing efficient lookups with dictionaries. These patterns demonstrate how different data structures can be selected to solve different types of problems effectively.

Through these exercises, I learned how dictionaries can be used to organize and count data, how sets provide a fast way to detect repeated values, and how stacks can be used to validate nested structures. I also practiced using dictionaries as lookup tables to quickly retrieve information. Overall, this homework strengthened my understanding of basic data structures and improved my ability to choose appropriate solutions for data-processing tasks.

# Problem Notes

## 1. Evidence Counter

### Pattern

Frequency Counting

### Data Structure

Dictionary

### Approach

* Step 1: Create an empty dictionary to store counts for each evidence label.
* Step 2: Iterate through every item in the evidence list.
* Step 3: If the label already exists in the dictionary, increase its count.
* Step 4: If the label does not exist, add it with a starting count of one.
* Step 5: Return the completed dictionary after processing all items.

### Complexity

* Time: `O(n)`
* Space: `O(n)`

Explain briefly:

The algorithm visits each evidence label exactly once. A dictionary is used because it allows fast updates and retrieval of counts. The amount of memory used depends on the number of unique evidence labels.

### Edge Cases Checked

* [x] Empty list
* [x] One item
* [x] Repeated items
* [x] Different labels

---

## 2. Repeat Suspect ID

### Pattern

Duplicate Detection

### Data Structure

Set

### Approach

* Step 1: Create an empty set to track IDs that have already been seen.
* Step 2: Iterate through the list of suspect IDs.
* Step 3: Check whether the current ID already exists in the set.
* Step 4: If it exists, return that ID as the first repeated value.
* Step 5: Otherwise, add the ID to the set and continue.
* Step 6: Return the appropriate value if no duplicates are found.

### Complexity

* Time: `O(n)`
* Space: `O(n)`

Explain briefly:

A set provides very fast membership checking. This allows duplicate IDs to be detected efficiently without needing nested loops that would increase runtime.

### Edge Cases Checked

* [x] Empty list
* [x] No repeated IDs
* [x] First two IDs match
* [x] Multiple repeated IDs

---

## 3. Evidence Tag Validator

### Pattern

Stack Matching

### Data Structure

List used as a Stack

### Approach

* Step 1: Create an empty stack.
* Step 2: Scan the string one character at a time.
* Step 3: Push opening tags or brackets onto the stack.
* Step 4: When a closing tag appears, check whether it matches the most recent opening tag.
* Step 5: Remove matched opening tags from the stack.
* Step 6: Continue until all characters are processed.
* Step 7: Return true only if every tag matches correctly and the stack is empty.

### Complexity

* Time: `O(n)`
* Space: `O(n)`

Explain briefly:

The stack follows a Last-In, First-Out structure, making it ideal for matching nested tags. Every character is processed once, resulting in linear runtime.

### Edge Cases Checked

* [x] Empty string
* [x] Correctly nested tags
* [x] Mismatched tags
* [x] Closing tag before opening tag
* [x] Unclosed opening tag
* [x] Non-bracket characters

---

## 4. Alias Directory

### Pattern

Lookup Table

### Data Structure

Dictionary

### Approach

* Step 1: Store aliases and corresponding values in a dictionary.
* Step 2: Receive the alias being searched for.
* Step 3: Check whether the alias exists in the dictionary.
* Step 4: Return the associated value if found.
* Step 5: Return the default result if the alias does not exist.

### Complexity

* Time: `O(1)`
* Space: `O(n)`

Explain briefly:

Dictionaries support constant-time average lookups, making them one of the most efficient structures for searching and retrieving stored information.

### Edge Cases Checked

* [x] Known alias
* [x] Unknown alias
* [x] Empty dictionary

# Assistance & Sources

## AI Used?

* [x] Yes
* [ ] No

## If yes, what did AI help with?

* Reviewed the logic used for each function.
* Explained how dictionaries, sets, and stacks solve different types of problems.
* Helped verify test cases and improve README documentation.

## Other Sources

None

