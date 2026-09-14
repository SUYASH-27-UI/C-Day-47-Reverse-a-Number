# C-Day-47-Reverse-a-Number
# C Day 47 - Reverse a Number

This program reverses the digits of a given number using a `while` loop.

## Example

Input:

```text
58321
```

Output:

```text
Reversed number = 12385
```

## Concepts Used

* `while` loop
* Modulus operator `%`
* Division operator `/`
* Digit extraction
* Variables
* Number reversing

## How It Works

1. Take a number from the user.
2. Extract the last digit using `% 10`.
3. Add the digit to the reverse number.
4. Remove the last digit using `/ 10`.
5. Repeat until the number becomes `0`.
6. Print the reversed number.

## C Code

```c
#include <stdio.h>

int main()
{
    int num, digit;
    int reverse = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0)
    {
        digit = num % 10;

        reverse = reverse * 10 + digit;

        num = num / 10;
    }

    printf("Reversed number = %d", reverse);

    return 0;
}
```

## Output

```text
Enter a number: 58321
Reversed number = 12385
```

## Goal

The goal of this project is to practice loops, modulus, division, and digit manipulation in C.
