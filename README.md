# Binary to Decimal Converter (Assembly)

This program is written in 16-bit x86 assembly and converts a user-input binary number to its decimal equivalent. It also validates the binary input, ensuring that only valid binary digits (`0` and `1`) are accepted. If the input is invalid, an error message is displayed, and the user is prompted to try again.

## Features

- **Binary Input:** Prompts the user to enter a binary number.
- **Binary to Decimal Conversion:** Converts the inputted binary number into its decimal equivalent.
- **Error Handling:** Checks if the input contains only `0` or `1`; otherwise, displays an error message and restarts the input process.
- **Displays Result:** After successfully entering a binary number, the corresponding decimal value is displayed.

## Program Flow

1. The program prompts the user to "write a binary number."
2. The user inputs a binary number, which the program validates.
3. If the input contains any character other than `0` or `1`, an error message is displayed, and the user is asked to re-enter the number.
4. Upon entering a valid binary number, the program calculates its decimal equivalent.
5. The decimal result is displayed, and the program terminates.

## How it Works

- The binary number is read character by character.
- Each `0` or `1` is processed and accumulated into a register (`bx`), shifting the bits accordingly.
- The accumulated binary value is then converted into decimal using division by 10 and displayed character by character.
