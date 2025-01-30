Mahjong Winning Hands Calculator

Overview

This Python program calculates the number of distinct Mahjong winning hands, w(n, s, t), where:

n is the range of tile numbers.

s is the number of suits available.

t is the number of triples (each being either a Chow or a Pung) plus one Pair.

The result is computed modulo 1,000,000,007 to handle large numbers efficiently.

Features

Uses modular arithmetic for fast calculations.

Implements combinatorial mathematics (C(n, k)) to count valid hands.

Supports large values of n, s, and t.

Mathematical Approach

Combination Formula (C(n, k)):

Uses factorial and modular inverse for efficient computation.

Computed using:



Triple Formation:

Chow: A sequence of three consecutive numbers in the same suit.

Pung: A set of three identical numbers in the same suit.

Computation Process:

Iterates over possible distributions of Chows and Pungs.

Uses combinatorial counting to determine the number of valid hands.

Applies modular arithmetic to keep calculations manageable.

Dependencies

Python 3.12

math module (for factorial calculations)

How to Run

Ensure you have Python installed.

Run the script:

python mahjong_winning_hands.py

Modify the n, s, and t values as needed in the script.

Example Usage

n = 10**8
s = 10**8
t = 30
result = count_winning_hands(n, s, t)
print(result)

License

This project is open-source and free to use.
