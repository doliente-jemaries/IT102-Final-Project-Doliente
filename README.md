# IT101-Final-Project-Doliente
A menu-driven console application developed in C for the IT101 – Programming 1 Final Project. This program combines different programming activities into one application, allowing users to select and perform different operations through a simple menu system.

## FEATURES

## 1. Pattern Generator

Generates different geometric shapes using asterisks (*) based on user-defined dimensions.

- Right Triangle – Prints a standard ascending triangle.
- Square – Prints an N × N grid of asterisks.
- Isosceles Triangle – Prints a centered pyramid of stars.
- Inverted Right Triangle – Prints a triangle pointing downwards.
- Christmas Tree – Prints multiple centered triangles with a trunk.

## 2. Pascal's Triangle

Calculates and prints Pascal's Triangle based on the number of rows entered by the user.

## 3. Grade Calculator and Evaluator

Accepts the student's grades and calculates the average.

- Accepts Prelim, Midterm, Semifinal, and Final grades.
- Calculates the average grade.
- Displays the corresponding result.

## 4. Palindrome Checker

Checks whether an entered word or sentence is a palindrome.

- Accepts user input.
- Compares characters from both ends.
- Displays whether the input is a palindrome or not.

Console Interface

The program runs in a console or terminal where users can select a module, enter the required information, and view the results.

Programming Language

- C Programming Language
- Standard Input and Output ("stdio.h")
- Loops and Conditional Statements
- Arrays
- Basic Mathematical Operations





## Code & Documentation Review Notes

### 1. Source Code Analysis (`codes.c`)
The implementation exhibits several structural and stylistic patterns commonly associated with LLM-generated code, alongside manual customization:
* **Uniform Formatting & Scaffolding:** Consistent uppercase section headers (`// 1. PATTERN GENERATOR`, `// 2. PASCAL'S TRIANGLE`, etc.) and standardized `===` / `---` console banners.
* **Upfront Variable Grouping:** All local variables across all four modules are declared in grouped blocks at the top of `main()` rather than scoped locally where used.
* **Defensive Input Handling & Workarounds:** Uses buffer-safe width specifiers (`scanf(" %99[^\n]", word)`), in-place two-pointer whitespace removal, and manual ASCII offset math (`+ 32`) instead of standard library headers (`<ctype.h>`, `<string.h>`), paired with unprompted bounds checking on all inputs.
* **Localized Customization:** Incorporates a Philippine grading scale (`1.00` to `5.00`) in the Grade Evaluator and duplicated triangle loops in the Christmas Tree pattern (`shape == 5`).

### 2. Design Documentation (`ALGORITHMN AND PSEUDOCODE.pdf` & Flowchart)
* **Commit Sequence:** Uploaded in a subsequent commit (`22ef0e9`) after `codes.c` was already present in the repository[cite: 1].
* **Reverse-Engineered Structure:** The algorithm steps and pseudocode mirror the exact implementation details of `codes.c` (such as displaying `"PATTERN GENERATOR"` and explicitly printing three separate triangles for the Christmas Tree) rather than serving as an independent pre-coding design specification[cite: 1].
