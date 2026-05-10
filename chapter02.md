# Chapter 2 Variables and Basic Types

## 2.1 Primitive Built-in Types

### 2.1.1 Arithmetic Types

### 2.1.2 Type Conversions

```cpp
bool b = 42;          // b is true
int i = b;            // i has value 1
i = 3.14;             // i has value 3
double pi = i;        // pi has value 3.0
unsigned char c = -1; // assuming 8-bit chars, c has value 255
signed char c2 = 256; // assuming 8-bit chars, the value of c2 is undefined
```

```cpp
int i = 42;
if (i) // condition will evaluate as true
    i = 0;
```

```cpp
unsigned u = 10;
int i = -42;
std::cout << i + i << std::endl; // prints -84
std::cout << u + i << std::endl; // if 32-bit ints, prints 4294967264
```

```cpp
unsigned u1 = 42, u2 = 10;
std::cout << u1 - u2 << std::endl; // ok: result is 32
std::cout << u2 - u1 << std::endl; // ok: but the result will wrap around
```

```cpp
// WRONG: u can never be less than 0; the condition will always succeed
for (unsigned u = 10; u >= 0; --u)
    std::cout << u << std::endl;
```

```cpp
unsigned u = 11; // start the loop one past the first element we want to print
while (u > 0)
{
    --u; // decrement first, so that the last iteration will print 0
    std::cout << u << std::endl;
}
```

### 2.1.3 Literals

## 2.2 Variables

### 2.2.1 Variable Definitions

### 2.2.2 Variable Declarations and Definitions

### 2.2.3 Identifiers

### 2.2.4 Scope of a Name

## 2.3 Compound Types

### 2.3.1 References

### 2.3.2 Pointers

### 2.3.3 Understanding Compound Type Declarations

## 2.4 const Qualifier

### 2.4.1 References to const

### 2.4.2 Pointers and const

### 2.4.3 Top-Level const

### 2.4.4 constexpr and Constant Expressions

## 2.5 Dealing with Types

### 2.5.1 Type Aliases

### 2.5.2 The auto Type Specifier

### 2.5.3 The decltype Type Specifier

## 2.6 Defining Our Own Data Structures

### 2.6.1 Defining the Sales_data Type

### 2.6.2 Using the Sales_data Class

### 2.6.3 Writing Our Own Header Files
