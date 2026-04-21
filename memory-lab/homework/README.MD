# 🧠 Memory Logger – Explanation

## 📌 What the program does

This program:
1. Reads 5 words from the user
2. Allocates memory for each word using `malloc`
3. Capitalizes the first letter of each word
4. Writes all words to `log.txt`
5. Frees all allocated memory

---

## 🧱 Full Flow

### Input
hello
world
pointers
are
fun

---

## ⚙️ Memory Allocation

Each word is stored in heap memory:

```c
words[i] = malloc(strlen(input) + 1);
✏️ String Processing

First letter is capitalized:

words[i][0] = toupper(words[i][0]);

Example:

hello → Hello
world → World
💾 File Writing

All words are saved into log.txt:

fprintf(file, "%s\n", words[i]);

Result in file:

Hello
World
Pointers
Are
Fun
🧹 Memory Cleanup

After finishing, memory is freed:

free(words[i]);

This prevents memory leaks.

🧠 Key Concepts
malloc → allocates memory on the heap
free → releases allocated memory
strcpy → copies strings
toupper → capitalizes characters
fopen / fprintf / fclose → file handling
🎯 Goal of this program

To understand:

Heap vs stack memory
Dynamic memory allocation
String manipulation in C
File input/output operations
