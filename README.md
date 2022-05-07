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
| 7 | Friend Functions & Static Members | `friend`, `this`, `static` |
| 8 | Copy Constructor & Binary Operator Overloading | shallow/deep copy, `operator+` |
| 9 | Advanced Operator Overloading | unary `++`/`--`, cast operator, `operator()` |
| 10 | File Handling | `ofstream`, `ifstream`, `fstream`, `eof()`, `seekg/seekp` |
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
│   └── assignment_templates.cpp      # Template assignment: smallest, reverse, max├── |||_friend_static/
│   ├── prelab_friend_functions.cpp          # Complex number add + Prime sum (friend fn)
│   └── inlab_friend_class_static_this.cpp   # Integer array, this pointer, friend class, VICOBA
│
├──_copy_constructor_operator_overloading/
│   ├── prelab_shallow_deep_copy.cpp         # Shallow vs deep copy — Rectangle class
│   └── inlab_operator_overloading.cpp       # Student vector, Complex ops, Matrix, Polynomial
│
├── _operator_overloading_advanced/
│   └── advanced_operator_overloading.cpp    # BigInt, GPA (dynamic memory), cast, function call
│
├──_file_handling/
│   ├── file_handling_complete.cpp           # All 9 core file handling programs
│   └── file_handling_assignments.cpp        # 7 assignment programs
│
├── assignments/                             # (reserved for future assignment files)
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

### Lab 05 — Friend Functions & Static Members

| File | What it does |
|------|-------------|
| `prelab_friend_functions.cpp` | Two programs: (1) Adds two complex numbers using a friend function. (2) Checks if a number can be expressed as sum of two prime numbers using a friend function. |
| `inlab_friend_class_static_this.cpp` | Four programs: (1) `IntArray` class with friend functions to find largest, smallest, repeated elements, and sort. (2) `this` pointer demo — identifies which object invoked a function. (3) Friend class: Square is friend of Rectangle. (4) VICOBA microfinance account with static interest rate and static member function. |

### Lab 06 — Copy Constructor & Operator Overloading

| File | What it does |
|------|-------------|
| `prelab_shallow_deep_copy.cpp` | Side-by-side demo of shallow copy (dangerous — shared memory) and deep copy (safe — independent memory) using a Rectangle class with pointer members. |
| `inlab_operator_overloading.cpp` | Four programs: (1) Student vector with copy constructor. (2) Complex number class with all 4 operators overloaded (intentionally swapped per lab spec). (3) Matrix class with overloaded `+`, `-`, `*`. (4) Polynomial class with deep copy, `operator+`, `operator-`, and `[]` accessor. |

### Lab 07 — Advanced Operator Overloading

| File | What it does |
|------|-------------|
| `advanced_operator_overloading.cpp` | Five programs: (1) `BigInt` class with unary prefix `++` and `--` for arbitrary-size integers. (2) Dynamic memory — student GPA stored in heap array with proper `delete[]`. (3) Complex class with cast operator converting object to string `"a + bi"`. (4) Polynomial class with function call `operator()` to evaluate at a given x. (5) Matrix2D class with cast operator to convert 2D matrix to 1D vector. |

### Lab 08 — File Handling

| File | What it does |
|------|-------------|
| `file_handling_complete.cpp` | All 9 core programs: write/read integers, write/read strings, count vowels with `eof()`, combined create-and-read, file copy, word/line/size counter with `seekg`/`tellg`, student records. |
| `file_handling_assignments.cpp` | 7 assignment programs: book records, read/write demo, append mode (`ios::app`), merge two files, count digits/alphabets/spaces, count word occurrence, student detail records. |
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

### Friend Function
```cpp
class MyClass {
    private: int x;
    friend void showX(MyClass obj);   // declared inside class
};
void showX(MyClass obj) { cout << obj.x; }  // defined outside — can access private!
```

### `this` Pointer
```cpp
void print() {
    cout << "Object at: " << this << endl;   // 'this' = address of calling object
    this->x = 10;                            // same as: x = 10;
}
```

### Static Member
```cpp
class Counter {
    static int count;   // ONE copy shared by all objects
public:
    Counter() { count++; }
    static int getCount() { return count; }  // no 'this' pointer
};
int Counter::count = 0;   // define outside class
// Usage: Counter::getCount();
```

### Copy Constructor
```cpp
MyClass(const MyClass& obj) {
    ptr = new int(*obj.ptr);   //  DEEP — new memory, copied value
    // ptr = obj.ptr;          //  SHALLOW — shared memory, dangerous!
}
```

### Operator Overloading
```cpp
Complex operator+(const Complex& obj) {
    return Complex(real + obj.real, imag + obj.imag);
}
// Usage: Complex c3 = c1 + c2;
```

### Unary Operator
```cpp
void operator++()    { ++value; }        // prefix  ++obj
void operator++(int) { value++; }        // postfix  obj++
```

### Cast Operator
```cpp
operator string() const {
    return to_string(real) + " + " + to_string(imag) + "i";
}
// Usage: string s = myComplexObj;   // automatic conversion
```

### File Handling
```cpp
// Write
ofstream out("file.txt");
out << "Hello World";
out.close();

// Read
ifstream in("file.txt");
string line;
while (getline(in, line)) cout << line;
in.close();

// Append (don't overwrite)
ofstream app("file.txt", ios::app);
app << "New line added";
app.close();
```

### Dynamic Memory
```cpp
int* arr = new int[n];    // allocate on heap
// use arr...
delete[] arr;             //  MUST free memory!
arr = nullptr;            // good practice
```
---

##  Author

 Shehroz Sultani 
BS-IT — Session 2025–2029  
Punjab University Gujranwala Campus  
Course: Object-Oriented Programming (OOP)

---
---

