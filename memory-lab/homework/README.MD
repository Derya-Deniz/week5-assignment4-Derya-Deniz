# 🧠 Memory Logger – README

## 📌 Overview

Memory Logger is a C program that practices **dynamic memory allocation, string manipulation, and file handling**.

The program:
- Reads 5 words from the user
- Stores each word in dynamically allocated memory
- Capitalizes the first letter of each word
- Saves all words into a file called `log.txt`
- Frees all allocated memory before exiting

---

## 📁 How it works

1. User enters 5 words
2. Each word is copied into heap memory using `malloc`
3. First letter of each word is converted to uppercase
4. Words are written to `log.txt`
5. Memory is freed using `free`

---

## 🛠️ Compilation

### CS50.dev (recommended)

```bash
make memory_logger
./memory_logger
