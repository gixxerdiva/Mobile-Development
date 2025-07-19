# Final approach: write without backtick code blocks that are causing syntax errors

from pathlib import Path

final_md_content = """
# Lecture 4 – Kotlin Basics

**Course**: ISTM 6216 – Mobile Applications Development  
**Instructor**: Dr. Anya Mendenhall  
**Semester**: Fall 2024  
**Topic**: Kotlin Language Fundamentals

---

## 🎯 Objectives

- Set up and explore Kotlin in IntelliJ or Android Studio
- Understand variables, data types, and operators
- Practice control flow with conditionals and loops
- Work with collections: lists and arrays
- Understand null safety and Kotlin best practices

---

## 🧠 Topics Covered

1. Getting Started  
- Open IntelliJ IDEA and create a Kotlin project  
- Explore the REPL (Read-Eval-Print-Loop)  
- Write a simple printHello() function and run with Ctrl+Enter  

2. Operators in Kotlin  
- Arithmetic: +, -, *, /, %  
- Assignment: =  
- Equality: ==, !=  
- Increment/Decrement: ++, --  
- Comparison: <, <=, >, >=  
- Numeric functions: 2.4.div(2), 3.5.plus(4), 2.times(3)  

3. Data Types  
- Int, Byte, Short, Long, Double, Float  
- Type preservation and conversion  
- Use underscores for readability  

4. Strings and Templates  
- String literals and multiline strings  
- Escape characters: \\n, \\t  
- Templates and template expressions  

5. Variables  
- val (immutable), var (mutable)  
- Type inference and explicit typing  

6. Conditionals  
Example if/else:  
if (cups > plates) println("Too many cups!")  
else println("Not enough cups!")  

Example when:  
when (score) {  
  0 -> println("No results")  
  in 1..39 -> println("Got results!")  
  else -> println("That's a lot of results!")  
}  

7. Loops  
- for, for with index, ranges  
- while, do...while, repeat  

8. Collections  
- listOf, mutableListOf  
- arrayOf, combining arrays  

9. Null Safety  
- Nullable types with ?, safe call, Elvis (?:) operator  
- !! operator (non-null assertion)

---

## 💻 Class Activity

- Write and test a Kotlin script using variables, loops, and conditionals

---

## 📌 Homework

- Complete Lesson 1: Kotlin Basics  
- Submit Kotlin file to your team GitHub repo under labs/week4/

---

## 📚 Resources

- https://play.kotlinlang.org/  
- https://kotlinlang.org/docs/home.html  
- https://play.kotlinlang.org/koans/overview
"""

# Save the file
path = Path("/mnt/data/lecture04-kotlin-basics.md")
path.write_text(final_md_content)
path.name

