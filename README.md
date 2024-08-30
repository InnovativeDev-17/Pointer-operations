# Pointer-operations
**Objective:**
To examine the concepts of call by value and call by reference using pointers.

**Theory:**

**Call by Reference:**
- **Definition:** Call by Reference involves passing the address (reference) of the actual parameters to a function. This approach allows the function to modify the original values directly.
- **How It Works:** The function receives pointers to the variables, enabling it to alter the original variables' values directly.

**Call by Value:**
- **Definition:** Call by Value involves passing a copy of the actual parameters to the function. Any modifications to the parameters within the function do not affect the original variables.

**Algorithm:**

**Call by Reference:**
1. **Start**
2. **Define Function:** `swap(int *x, int *y)`
3. **Input:** Pointers to two integers `x` and `y`
4. **Output:** Swapped values of the integers pointed to by `x` and `y`
5. **Steps:**
   - Create a temporary variable `temp`.
   - Assign the value pointed to by `x` to `temp` (`temp = *x`).
   - Assign the value pointed to by `y` to the location pointed to by `x` (`*x = *y`).
   - Assign the value of `temp` to the location pointed to by `y` (`*y = temp`).
6. **In the Main Function:**
   - Define integers `a` and `b` with values 5 and 2, respectively.
   - Call `swap(&a, &b)` function.
   - Print the value of `a`.
   - Print the value of `b`.
7. **End**

**Call by Value:**
1. **Start**
2. **Define Function:** `swap(int x, int y)`
3. **Input:** Two integers `x` and `y`
4. **Output:** Swapped values of `x` and `y`
5. **Inside Swap Function:**
   - Create a temporary variable `temp`.
   - Assign the value of `x` to `temp`.
   - Assign the value of `y` to `x`.
   - Assign the value of `temp` to `y`.
6. **Inside Main Function:**
   - Define two integers `a` and `b` with values 5 and 2, respectively.
   - Call `swap(a, b)`.
   - Print the value of `a`.
   - Print the value of `b`.
7. **End**
