# Set 3: Loops & Input Validation (Problems 21-30) 

This folder marks the transition from basic formulas to iterative logic. It focuses on using loops (`for`, `while`, `do-while`) for accumulating results, enforcing input constraints, and printing sequences.

## Problem List & File Names

| # | File Name | Description & Concepts |
| :-: | :--- | :--- |
| **21** | `21_Circle_Area_Circumference.cpp` | **Circle Area**: Calculating area via Circumference. |
| **22** | `22_Circle_Area_Isosceles_Triangle.cpp` | **Geometric Formulas**: Complex formula implementation. |
| **23** | `23_Circle_Area_Arbitrary_Triangle.cpp` | **Advanced Geometry**: Using `struct` for triangle sides & square root calculations. |
| **24** | `24_Validate_Age_Range.cpp` | **Range Check**: Simple Boolean validation logic. |
| **25** | `25_Read_Age_Until_Valid.cpp` | **Input Loop**: Using `do-while` loop to enforce valid input (18-45). |
| **26** | `26_Print_1_To_N.cpp` | **Counting Up**: Basic `for` loop (Increment). |
| **27** | `27_Print_N_To_1.cpp` | **Counting Down**: Basic `for` loop (Decrement). |
| **28** | `28_Sum_Odd_Numbers.cpp` | **Sum Odd**: Combining Loops with `if` conditions & `Enums`. |
| **29** | `29_Sum_Even_Numbers.cpp` | **Sum Even**: Accumulating even numbers in a range. |
| **30** | `30_Factorial_Calculator.cpp` | **Factorial (!)**: Using `long long` to prevent overflow in iterative multiplication. |

## Code Highlights

### 1. Robust Input Validation (Problem 25)
Using a `do-while` loop to ensure the program never proceeds until the user enters data within the specific range.
```cpp
int Read_Until_Age_Between(int From, int To)
{
    int Age = 0;
    do
    {
        Age = Get_User_Age();
    } while (!Validate_Number_In_Range(Age, From, To));
    return Age;
}