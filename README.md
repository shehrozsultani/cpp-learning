#  C++ Object-Oriented Programming — Lab Tasks & Assignments

> A complete collection of **C++ OOP lab exercises and assignments** from BS-IT (Session 2025–2029) at **Punjab University Gujranwala Campus**.  
> Topics covered: Classes, Constructors, Inheritance, Deep/Shallow Copy, Templates, and more.

---

##  Table of Contents

- [About the Project](#about-the-project)
- [Topics Covered](#topics-covered)
- [Folder Structure](#folder-structure)
- [File Descriptions](#file-descriptions)
- [How to Run](#how-to-run)
- [Key Concepts Explained](#key-concepts-explained)
- [Known Issues & Fixes](#known-issues--fixes)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

##  About the Project

This repository contains all lab programs and assignments written in **C++** for the **Object-Oriented Programming (OOP)** course. Each file is clearly commented and organized by topic, making it easy to revise concepts and use as a reference.

Whether you are a student learning OOP for the first time or reviewing for exams — this repository is designed to be **beginner-friendly and easy to follow**.

---

##  Topics Covered

| #  | Topic                          | Folder                     |
|----|--------------------------------|----------------------------|
| 1  | Constructors & Destructors     | `lab01_constructors/`      |
| 2  | Static Members & Array of Objects | `lab02_static_arrays/`  |
| 3  | Classes, Objects & Fundamentals | `lab03_objects_classes/`  |
| 4  | Deep Copy vs Shallow Copy      | `lab04_deep_shallow_copy/` |
| 5  | Inheritance (All Types)        | `lab05_inheritance/`       |
| 6  | Templates (Function & Class)   | `lab06_templates/`         |
| —  | Assignments                    | `assignments/`             |

---

##  Folder Structure

```
cpp-oop-lab/
│
├── _constructors/
│   ├── task1_department.cpp          # Constructor overloading — Department class
│   ├── task2_area_calculator.cpp     # Area of Square, Rectangle, Circle, Triangle
│   └── task3_constructor_basics.cpp  # Default vs Parameterized constructors
│
├──_static_arrays/
│   └── task1_student_average.cpp     # Array of objects — student marks & average
│
├── _objects_classes/
│   ├── task1_student_box.cpp         # Class basics — Student & Box classes
│   └── lab_task1_fundamentals.cpp    # First programs, palindrome, word count, etc.
│
├── _deep_shallow_copy/
│   └── deep_vs_shallow_copy.cpp      # Shallow vs Deep copy constructors
│
├── _inheritance/
│   ├── inheritance_all_types.cpp          # Public, Multiple, Multilevel inheritance
│   └── inheritance_real_world_examples.cpp # Person→Student, Simple→Complex calculator
│
├── _templates/
│   └── templates_all.cpp             # All template programs combined
│
├── assignments/
│   ├── gpa_calculator.cpp            # GPA calculator using classes
│   └── assignment_templates.cpp      # Template assignment: smallest, reverse, max
│
└── README.md
```

---

##  File Descriptions

###  — Constructors

| File | What it does |
|------|-------------|
| `task1_department.cpp` | Creates a `Department` class. Uses **default** and **parameterized** constructors to show a message with or without a department name. |
| `task2_area_calculator.cpp` | One class `Area` calculates areas of **4 different shapes** using constructor overloading. C++ picks the right constructor based on how many arguments you pass. |
| `task3_constructor_basics.cpp` | Demonstrates the **lifecycle of an object** — when a constructor fires, what happens in memory, and how default vs parameterized constructors differ. |

###  — Array of Objects

| File | What it does |
|------|-------------|
| `task1_student_average.cpp` | Stores 5 students in an **array of objects**. Each student has roll number + marks in 3 subjects. Calculates and displays average for each. |

###  — Classes & Objects

| File | What it does |
|------|-------------|
| `task1_student_box.cpp` | Introduces **private/public/protected** access specifiers using a `Student` and `Box` class. Shows how private data is accessed through member functions. |
| `lab_task1_fundamentals.cpp` | Beginner tasks: Hello World, finding the middle number, word/character counter, palindrome check, geometry class, and a common **bug-fix exercise** on a Student class. |

###  — Deep vs Shallow Copy

| File | What it does |
|------|-------------|
| `deep_vs_shallow_copy.cpp` | Side-by-side comparison of **shallow copy** (dangerous — shares pointer memory) vs **deep copy** (safe — allocates new independent memory). Visual output shows the difference clearly. |

###  — Inheritance

| File | What it does |
|------|-------------|
| `inheritance_all_types.cpp` | Demonstrates **Public**, **Multiple**, and **Multilevel** inheritance with access specifier rules and object sizing. |
| `inheritance_real_world_examples.cpp` | Real-world examples: `Person → Student` class chain, and a `SimpleCalc → ComplexCalc` override for input-validated arithmetic. |

###  — Templates

| File|-- | What it does |
|-----------------|
| `templates_all.cpp` | All template programs in one place: generic `display()`, `abs()`, two-type template, `Calc<T>` class template, `findSmallest()`, and `displayReverse()`. |

### Assignments

| File | What it does |
|------|-------------|
| `gpa_calculator.cpp` | Full GPA calculator. Takes marks + credit hours for 5 subjects, converts to grade points, and computes cumulative GPA. |
| `assignment_templates.cpp` | Template assignment: find smallest of 3 mixed-type values, reverse display, find max in a typed array. |

---

##  How to Run

### Prerequisites
- A C++ compiler: [g++](https://gcc.gnu.org/) (Linux/Mac) or [MinGW](https://www.mingw-w64.org/) (Windows)
- Or an IDE: [VS Code](https://code.visualstudio.com/), [Dev-C++](https://www.bloodshed.net/), [Code::Blocks](http://www.codeblocks.org/)

### Compile and Run (Terminal)

```bash
# Step 1: Navigate to the file's folder
cd lab01_constructors

# Step 2: Compile with g++
g++ task1_department.cpp -o task1_department

# Step 3: Run the output
./task1_department       # Linux/Mac
task1_department.exe     # Windows
```

### Using VS Code
1. Install the **C/C++ Extension** by Microsoft.
2. Open any `.cpp` file.
3. Press `Ctrl + Shift + B` to build, then run the terminal.

---

##  Key Concepts Explained

### Constructor Overloading
Same class, multiple constructors with different parameters. C++ picks the right one automatically.
```cpp
Department();             // Called with no argument
Department(string name);  // Called with a string argument
```

### Deep vs Shallow Copy
```
Shallow Copy: obj2.ptr ──────────────► [same memory as obj1.ptr]
Deep Copy:    obj2.ptr ──► [new memory] = value from obj1
```

### Inheritance Types
```
Single:     A → B
Multiple:   A + B → C
Multilevel: A → B → C
```

### Templates
```cpp
template<class T>
T add(T a, T b) { return a + b; }
// Works for int, float, double — anything!
```

---

##  Known Issues & Fixes

| Issue Found | Location | Fix Applied |
|-------------|----------|-------------|
| `#include <conio.h>` used (`clrscr`, `getch`) | `INHERITENCE_Types_` (original) | Removed — not portable (Windows only). Standard C++ used instead. |
| `cin >> id` before `cin.getline()` skips input | Inheritance IT series example | Added `cin.ignore()` to flush the newline buffer. |
| `return 0.0` inside `int set()` function when marks < 50 | GPA Calculator (original) | Fixed: extracted grade point logic to a separate private method `getGradePoint()`. |
| Arrays copied with `=` operator | `lab_task1 bug` section | Fixed: used a loop to copy array elements one by one. |
| Missing `using namespace std` and `<string>` include | Original assignment file | Fixed in corrected version with proper includes. |

---

##  Future Improvements

- [ ] Add **operator overloading** examples (e.g., `+`, `==`, `<<` for custom classes)
- [ ] Add **virtual functions** and **polymorphism** examples
- [ ] Add **file handling** programs (read/write with classes)
- [ ] Add **exception handling** (`try`, `catch`, `throw`)
- [ ] Add **STL** examples (vectors, maps, sets)
- [ ] Create a simple **makefile** to build all programs at once
- [ ] Add expected output comments at the bottom of each file

---

##  Author

** Shehroz Sultani**  
BS-IT — Session 2025–2029  
Punjab University Gujranwala Campus  
Course: Object-Oriented Programming (OOP)

---
---

