# Mission 5 — Numbers and Data

## Mission Objective

The objective of this mission was to understand how computers represent numbers and text using different number systems, including decimal, binary and hexadecimal. I also practised converting numbers manually, verifying conversions using Python and building a small number converter.

---

## Task 5.1 — Convert Numbers by Hand

### 1. Decimal 13 to Binary

Using repeated division by 2:

| Division | Quotient | Remainder |
|---|---:|---:|
| 13 ÷ 2 | 6 | 1 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

Reading the remainders from bottom to top:

**(13)₁₀ = (1101)₂**

### 2. Decimal 25 to Binary

Using repeated division by 2:

| Division | Quotient | Remainder |
|---|---:|---:|
| 25 ÷ 2 | 12 | 1 |
| 12 ÷ 2 | 6 | 0 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

Reading the remainders from bottom to top:

**(25)₁₀ = (11001)₂**

### 3. Binary 1010 to Decimal

Using powers of 2:

= (1 × 2³) + (0 × 2²) + (1 × 2¹) + (0 × 2⁰)

= 8 + 0 + 2 + 0

**(1010)₂ = (10)₁₀**

### 4. Binary 1101 to Decimal

= (1 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰)

= 8 + 4 + 0 + 1

**(1101)₂ = (13)₁₀**

### 5. Hexadecimal A to Decimal

In hexadecimal, A represents 10.

**(A)₁₆ = (10)₁₀**

### 6. Hexadecimal 1F to Decimal

= (1 × 16¹) + (15 × 16⁰)

= 16 + 15

**(1F)₁₆ = (31)₁₀**

### 7. Binary 1111 to Hexadecimal

First, convert binary to decimal:

= 8 + 4 + 2 + 1

= 15

In hexadecimal, 15 is represented by F.

**(1111)₂ = (F)₁₆**

---

## Task 5.2 — Verify Using Python

I opened the Python interactive environment using Terminal with:

```bash
python3
```

I used Python's built-in conversion functions to verify my manual calculations.

### Expressions Tested

| Python Expression | Python Result | Manual Result | Status |
|---|---|---|---|
| `bin(13)` | `0b1101` | `1101` | Match |
| `bin(25)` | `0b11001` | `11001` | Match |
| `int('1010', 2)` | `10` | `10` | Match |
| `int('1101', 2)` | `13` | `13` | Match |
| `hex(13)` | `0xd` | Additional check | Correct |
| `int('1F', 16)` | `31` | `31` | Match |
| `hex(int('1111', 2))` | `0xf` | `F` | Match |

### Python Functions Used

- `bin()` converts a decimal integer into binary.
- `int(value, 2)` converts a binary number into decimal.
- `hex()` converts a decimal integer into hexadecimal.
- `int(value, 16)` converts a hexadecimal number into decimal.

**Note:** Python uses `0b` as a prefix for binary numbers and `0x` as a prefix for hexadecimal numbers.

All the tested conversions matched the manual calculations.

---

## Task 5.3 — Build a Small Number Converter

I created a Python program named `number_converter.py` inside the `mission-05-numbers-data` folder.

### Program Code

```python
num = int(input("Enter a decimal number: "))

binary_num = bin(num)
hex_num = hex(num)

print("Binary:", binary_num)
print("Hexadecimal:", hex_num)
```

### Explanation

1. `input()` takes a decimal number from the user.
2. `int()` converts the input into an integer.
3. `bin()` converts the decimal number into binary.
4. `hex()` converts the decimal number into hexadecimal.
5. `print()` displays the converted results.

### Testing the Program

I ran the program using:

```bash
python3 number_converter.py
```

I tested it with three different positive numbers.

| Decimal Input | Binary Output | Hexadecimal Output |
|---|---|---|
| 13 | `0b1101` | `0xd` |
| 25 | `0b11001` | `0x19` |
| 31 | `0b11111` | `0x1f` |

All three tests produced the expected outputs.

---

## Task 5.4 — How Is Text Stored?

Computers store and process information in binary form. Character-encoding standards assign numerical values to characters so that computers can store, transmit and interpret text consistently.

### ASCII Values

| Character | ASCII Decimal Value |
|---|---:|
| A | 65 |
| a | 97 |

### Character Not Included in Basic ASCII

Example: **₹ (Indian Rupee symbol)**

The Indian Rupee symbol is not included in basic ASCII.

UTF-8 supports a much wider range of characters than basic ASCII, including characters from different languages, symbols and emojis.

---

## What I Learned

- How to convert decimal numbers into binary using repeated division by 2.
- How to convert binary numbers into decimal using powers of 2.
- How to convert hexadecimal numbers into decimal.
- How to convert binary numbers into hexadecimal.
- How to use Python's built-in `bin()`, `hex()` and `int()` functions.
- How to create and execute a basic Python number converter.
- How computers represent text using character-encoding standards such as ASCII and UTF-8.

### Challenges and Understanding

One important thing I learned was to read the remainders from bottom to top when converting decimal numbers into binary.

I also understood the difference between binary and hexadecimal prefixes in Python (`0b` and `0x`) and how character encoding helps computers represent text.

---

## Conclusion

Through this mission, I learned how numbers and text are represented inside computers. I practised manual conversions, verified my answers using Python and successfully built a number converter that converts decimal numbers into binary and hexadecimal.
