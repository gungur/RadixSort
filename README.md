# Radix Sort Implementation

A Java implementation of the Radix Sort algorithm with example usage and printing capabilities.

## Overview

This project contains two main Java classes that implement and demonstrate the Radix Sort algorithm:

- **RadixSorter.java**: Implements the radix sort algorithm using counting sort as a subroutine
- **SortPrinter.java**: Demonstrates the sorting algorithm on sample arrays

## Algorithm Details

### Radix Sort
Radix sort is a non-comparative integer sorting algorithm that sorts numbers by processing individual digits. It processes digits from least significant to most significant, using a stable sorting algorithm (counting sort in this implementation) at each digit position.

### Time Complexity
- **Worst-case**: O(d·(n + k))
- **Average-case**: O(d·(n + k))
- **Best-case**: O(d·(n + k))

Where:
- `n` = number of elements
- `d` = number of digits in the maximum number
- `k` = the radix (base 10 in this implementation)

## Files

### RadixSorter.java
Contains the main radix sort implementation with the following methods:

- `radixSort(int[] array)`: Main method that performs radix sort on the given array
- `countingSort(int[] array, int digit)`: Helper method that performs counting sort based on a specific digit
- `getMax(int[] array)`: Utility method to find the maximum value in an array

### SortPrinter.java
Demonstrates the usage of the RadixSorter class with sample arrays and prints the sorted results.

## Usage

### Compilation
```bash
javac RadixSorter.java SortPrinter.java
```

### Execution
```bash
java SortPrinter
```

### Example Output
```
[2, 3, 5, 7, 8]
[2, 5, 12, 15, 20, 49, 80]
```

## Features

- **In-place sorting**: Modifies the original array directly
- **Stable sorting**: Maintains the relative order of elements with equal keys
- **Base-10 implementation**: Works with decimal numbers
- **Efficient**: Handles large numbers efficiently by processing digit by digit

## Requirements

- Java Development Kit (JDK) 8 or higher
- No external dependencies required
