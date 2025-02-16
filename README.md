
# Rotated Sorted Array Search

## Description
This repository contains a C++ implementation of a **modified binary search algorithm** to find the index of a target value in a **rotated sorted array**. The algorithm efficiently searches for the target in **O(log n)** time complexity.

## Problem Statement
Given a **rotated sorted array** (e.g., `[4, 5, 6, 7, 0, 1, 2]`) and a target value, the goal is to find the index of the target in the array. If the target does not exist, the function returns `-1`.

## Key Features
- **Efficient Search:** Uses binary search to achieve **O(log n)** time complexity.
- **Handles Rotated Arrays:** Works for arrays that have been rotated at an unknown pivot point.
- **Edge Cases:** Handles edge cases such as empty arrays, single-element arrays, and targets not present in the array.

## Code Explanation
The algorithm works as follows:
1. Initialize two pointers, `low` and `high`, to the start and end of the array.
2. Calculate the middle index `mid`.
3. If `arr[mid]` equals the target, return `mid`.
4. Determine if the left or right half of the array is sorted.
5. Check if the target lies within the sorted half:
   - If yes, search that half.
   - If no, search the other half.
6. Repeat until the target is found or the search range is exhausted.

## Example
### Input:
arr = [4, 5, 6, 7, 0, 1, 2]
target = 0

### Output:
4


### Explanation:
- The target `0` is found at index `4` in the array.

## Complexity Analysis
- **Time Complexity:** O(log n)
- **Space Complexity:** O(1)

## How to Use
1. Clone the repository:
   
   git clone https://github.com/your-username/rotated-sorted-array-search.git
   
2. Navigate to the project directory:
   
   cd rotated-sorted-array-search
   
3. Compile the code:
   
   g++ search.cpp -o search
   
4. Run the executable:
  
   ./search
  

## Dependencies
- C++ compiler (e.g., g++)

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.


