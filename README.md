# Stack-Based Radix Sort Algorithm

## Introduction
This repository holds a custom implementation of a radix sort algorithm, specifically designed to sort stacks. The algorithm uses bitwise operations to determine the sorting order of indices, which are then used to sort the actual values in the stack. This method is efficient and well-suited for data structures where direct value comparisons are not as optimal.

## Algorithm Details
The `ft_radix` function is the core of this algorithm. It takes two stacks, `a_stack` and `b_stack`, and sorts the indices in `a_stack` according to the bits set in their binary representation. The process is as follows:
- Iteratively check each bit position of the indices starting from the least significant bit.
- If the current bit is set, perform a rotate operation; otherwise, push the index to a temporary stack.
- After all indices are processed for the current bit, the ones with unset bits are pushed back, and the algorithm moves to the next bit position.
- This continues until the entire stack is sorted.

## Installation
Clone this repository to your local machine using the following command:
- git clone https://github.com/Dragoshiz/sorting_algorithm.git

# Navigate to the project directory and run:
- make

## Usage
After compiling the program, you can sort stacks by executing the compiled binary with the appropriate parameters.<br>
Here's an example command:
- ./push_swap 6 3 2 9 1

