# Set 2: Math Algorithms & Conditional Logic (Problems 11-20)

This folder focuses on mathematical algorithms, geometric calculations, and referencing variables. It demonstrates how to translate mathematical formulas into efficient C++ code.

## Problem List & File Names

| # | File Name | Description & Concepts |
| :-: | :--- | :--- |
| **11** | `11_Average_Pass_Fail.cpp` | **Average & Status**: Using `Arrays` and `Enums` to determine Pass/Fail. |
| **12** | `12_Max_Of_2_Numbers.cpp` | **Max of 2**: Simple comparison logic using `struct`. |
| **13** | `13_Max_Of_3_Numbers.cpp` | **Max of 3**: Nested `if-else` logic to find the largest value. |
| **14** | `14_Swap_Numbers.cpp` | **Swap Variables**: Implementation of **Pass by Reference** to modify original values. |
| **15** | `15_Rectangle_Area.cpp` | **Rectangle Area**: Basic arithmetic operations. |
| **16** | `16_Rectangle_Area_Diagonal.cpp` | **Rectangle via Diagonal**: Using `cmath` library (`sqrt`, `pow`). |
| **17** | `17_Triangle_Area.cpp` | **Triangle Area**: handling geometry formulas with `struct`. |
| **18** | `18_Circle_Area.cpp` | **Circle Area**: Using Math Constants (`M_PI`) for precision. |
| **19** | `19_Circle_Area_Diameter.cpp` | **Circle Area (Diameter)**: Formula adaptation. |
| **20** | `20_Circle_Area_Inscribed_Square.cpp` | **Inscribed Circle**: Input validation loops (`do-while`) & geometry. |

## Code Highlights

### 1. Pass by Reference (Problem 14)
Unlike passing by value, here we access the memory address directly to swap values in the `main` function from within a void function.
```cpp
void Swap_Number(int& Num_1, int& Num_2)
{
    int Temp = Num_1;
    Num_1 = Num_2;
    Num_2 = Temp;
}