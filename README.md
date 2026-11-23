# Integer vs. Floating-Point Detector (C)

A small C program that reads a number from the user and determines whether it
represents an integer or a floating-point value, using a `union` to share memory
between the two interpretations.

## 🎯 What It Demonstrates

- **Unions in C** — a `union DataValue` overlays an `int` and a `float` in the
  same memory location, showing how C lets you reinterpret stored bytes.
- **Float inspection** — comparing a value against its own `floorf()` to detect
  whether it has a fractional part.
- **Defensive input handling** — checks `scanf`'s return value instead of trusting
  the user.

## 🚀 How to Run

Requires a C compiler (GCC/Clang) and the math library.

```bash
gcc main.c -o detector -lm
./detector
