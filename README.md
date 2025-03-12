# Narcissistic Numbers Script

This script checks for narcissistic numbers within a given range and prints them out.

## Execution Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/<your_username>/narcissistic-numbers.git
    ```
   
2. **Navigate to the repository directory**:
    ```bash
    cd narcissistic-numbers
    ```

3. **Run the script**:
    ```bash
    python <script_name.py>  # Replace <script_name.py> with the actual name of your script file
    ```

## Errors Found and Changes Made

1. **Function Definition Error**:
    - **Original**: `def is_narc(n)`
    - **Fixed**: Added a colon at the end of the line.
    - **Fixed Code**:
    ```python
    def is_narc(n):
    ```

2. **Variable Assignment Error**:
    - **Original**: `num_str == str(n)` and `num_digits == len(num_str)`
    - **Fixed**: Changed `==` to `=` for proper variable assignment.
    - **Fixed Code**:
    ```python
    num_str = str(n)
    num_digits = len(num_str)
    ```

3. **Power Calculation Error**:
    - **Original**: `sum(int(digit) *** num_digits for digit in num_str)`
    - **Fixed**: Changed `***` to `**` for proper power calculation.
    - **Fixed Code**:
    ```python
    sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)
    ```

4. **Function Call Error**:
    - **Original**: `print_narc_numbers(1000, 5000)`
    - **Fixed**: Updated the function call to match the corrected function name.
    - **Fixed Code**:
    ```python
    print_narcis_numbers(1000, 5000)
    ```

5. **Function Name Consistency**:
    - **Original**: Function name inconsistency between `print_narc_numbers` and `print_narcis_numbers`.
    - **Fixed**: Ensured that the function names are consistent throughout the script.
    - **Fixed Code**:
    ```python
    def print_narcis_numbers(start, end):
        for num in range(start, end + 1):
            if is_narc(num):
                print(num)
    ```
