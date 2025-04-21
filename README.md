# Scheme to Assembly Compiler (OCaml)

This project is a compiler that translates a subset of the Scheme programming language into low-level assembly-like code. It was developed as a final project for the **Principles of Compilation** course at university.

## 🎯 Project Objective

To understand and apply compilation techniques by building a working compiler from Scheme to an x86-like assembly language. The project focuses on parsing, semantic analysis, intermediate representation (IR), and code generation.

## ⚙️ Key Features

- Written in OCaml using functional programming paradigms
- Parses core Scheme constructs: `define`, `lambda`, arithmetic, conditionals
- Performs variable binding and lexical scoping analysis
- Generates readable assembly-like output from AST
- Custom modules for parsing, AST generation, IR, and emitter
- Tail recursion and scoping optimizations (if implemented)

## 🛠 Technologies Used

- OCaml
- Menhir or ocamllex (if used for parsing)
- Custom parser and compiler backend
- Unix/Linux environment for testing

## 🚀 How to Build and Run

1. Navigate to the project folder:
   ```bash
   cd scheme-to-assembly-ocaml
   ```

2. Compile the project (if using dune or make):
   ```bash
   make
   ```

3. Run the compiler:
   ```bash
   ./compiler path/to/source.scm
   ```

4. Output will be written to the terminal or an output file (based on your setup)

## 🧪 Example Input & Output

### Input (Scheme)
```scheme
(define square (lambda (x) (* x x)))
(square 5)
```

### Output (Assembly-like)
```
LABEL square
LOAD x
MUL x
RET
CALL square, 5
```

## ✍️ Author

- [Niv Yaakobov](https://github.com/Niv-Yaakobov)

> Developed as part of the **Principles of Compilation** course using OCaml.
