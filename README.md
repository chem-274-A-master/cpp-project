# Project 3

For this project, you will write a functioning matrix class in C++. We are
leaving some details up to you - a lot of programming is determining, from
a specification, how something should be implemented.

## Required features

1. The matrix class should be templated, so that it works with any
   type. Particularly, it should work with `double`, `float`,
   and `int`, along with the `std::complex` variations of those types.

2. There should be three constructors - one with no arguments, one with the
   desired number of rows/columns, and a copy constructor.

3. The matrix should have the ability to be resized. When using this function,
   the user should assume that any existing data is either destroyed or
   invalid after resizing

4. You should have the following operations:
   1. Matrix addition (can overload the + operator) 
   2. Matrix multiplication (can overload the * operator)
   3. Matrix element-wise multiplication
   4. Copy constructor and assignment operator (you don't have to necessarily write one, but it must be supported!)
   5. Comparison of two matrices (overload `operator==`. **HINT:** look up documentaton for `std::equal`)
   6. Printing of the matrix to a `std::ostream` object.

5. Accessing the elements of the matrix should be the parentheses operator. Ie, you should be able to
   access element 2,3 via `mat(2,3)`.

Overall, the class should be `const` correct and free of memory leaks. You
should throw exceptions when operations aren't valid (ie, matrix multiplication
of incompatible sizes).

Since this is a templated class, it should exist completely in a header
file. Also create a `.cpp` source file to demonstrate your matrix class and
its capabilities.
