# Hack Bug Report: Stack Overflow in Recursive Function

This repository demonstrates a common error in Hack: a stack overflow caused by uncontrolled recursion.  The `foo` function calculates the factorial recursively but lacks a base case to prevent infinite calls when the input `x` is negative. The `bar` function calls `foo` with a positive value but the recursive nature still allows negative inputs to be encountered internally, leading to the error.

The solution demonstrates how to add a proper base case check to prevent the stack overflow.  It also illustrates the importance of considering all possible input scenarios when writing recursive functions.