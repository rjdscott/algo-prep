# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python repository for Data Structures and Algorithms interview preparation using Jupyter notebooks. The codebase follows the Neetcode roadmap, organizing problems by common patterns to build systematic problem-solving skills.

## Repository Structure

Problems are organized by pattern/category in the `problems/` directory:

```
problems/
├── arrays_and_hashing/      # Array manipulation, hash tables
├── two_pointers/            # Two pointer technique
├── sliding_window/          # Window-based problems
├── stack/                   # Stack operations
├── binary_search/           # Search algorithms
├── linked_list/             # Linked list problems
├── trees/                   # Binary trees, BST, traversals
├── tries/                   # Prefix trees
├── heap_priority_queue/     # Heap problems
├── backtracking/            # Combinatorial problems
├── graphs/                  # Graph traversal
├── advanced_graphs/         # Advanced graph algorithms
├── dynamic_programming_1d/  # 1D DP problems
├── dynamic_programming_2d/  # 2D DP problems
├── greedy/                  # Greedy algorithms
├── intervals/               # Interval problems
├── math_and_geometry/       # Mathematical problems
└── bit_manipulation/        # Bitwise operations

tests/
└── [mirrors problems/ structure]
```

## Development Setup

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Lab (recommended)
jupyter lab

# Or launch Jupyter Notebook
jupyter notebook

# Run tests
pytest

# Run tests with coverage
pytest --cov=problems

# Run specific test file
pytest tests/arrays_and_hashing/test_two_sum.py -v
```

## Notebook Structure

All problems are implemented as Jupyter notebooks (.ipynb) with the following structure:

1. **Problem Statement** - Full problem description, constraints, examples
2. **Initial Observations** - Key insights before solving
3. **Approach 1: Brute Force** - Naive solution with explanation
4. **Approach 2+: Optimized** - Improved solutions
5. **Detailed Walkthrough** - Step-by-step trace with verbose output
6. **Edge Cases** - Comprehensive test cases
7. **Complexity Analysis** - Time/space analysis for each approach
8. **Interview Tips** - What to say during interviews
9. **Related Problems** - Similar problems to practice

## File Naming Convention

Problems use the format: `{leetcode_number}_{problem_name}.ipynb`

Examples:
- `001_two_sum.ipynb`
- `217_contains_duplicate.ipynb`
- `049_group_anagrams.ipynb`

## Creating New Problems

Use `problems/TEMPLATE.ipynb` as a starting point for new problems. The template includes:
- Standardized structure and sections
- Complexity analysis tables
- Test case framework
- Verbose walkthrough skeleton

When implementing solutions:
- Start with brute force approach
- Progress to optimized solutions
- Include multiple approaches when applicable
- Add detailed complexity analysis
- Provide step-by-step walkthroughs with print statements
- Cover edge cases thoroughly
- Include visual representations where helpful

## Study Approach

Recommended order for interview preparation:

1. **Core Patterns** (Start here - Essential for all interviews)
   - arrays_and_hashing
   - two_pointers
   - sliding_window
   - stack
   - binary_search

2. **Data Structures**
   - linked_list
   - trees
   - tries
   - heap_priority_queue

3. **Advanced Patterns** (For more challenging interviews)
   - backtracking
   - graphs
   - dynamic_programming_1d
   - dynamic_programming_2d
   - greedy
   - intervals

4. **Specialized**
   - advanced_graphs
   - math_and_geometry
   - bit_manipulation

## Testing

Tests are located in `tests/` directory mirroring the `problems/` structure. Each notebook should have a corresponding test file that:
- Tests all solution approaches
- Covers edge cases
- Validates time complexity on large inputs
- Includes the original test cases from the problem

Create tests using pytest:

```python
# tests/arrays_and_hashing/test_two_sum.py
import pytest
from problems.arrays_and_hashing.two_sum import two_sum

def test_two_sum_basic():
    assert two_sum([2, 7, 11, 15], 9) == [0, 1]

def test_two_sum_edge_cases():
    assert two_sum([3, 3], 6) == [0, 1]
```

## Key Patterns to Master

Each category teaches specific problem-solving patterns:

- **Arrays & Hashing**: Hash maps for O(1) lookup, frequency counting
- **Two Pointers**: Left/right pointers, fast/slow pointers
- **Sliding Window**: Expanding/contracting windows, substring problems
- **Binary Search**: Search space reduction, rotated arrays
- **Trees**: DFS (in/pre/post-order), BFS, recursion
- **Dynamic Programming**: Memoization, tabulation, state transitions
- **Graphs**: DFS/BFS traversal, topological sort, shortest paths
- **Backtracking**: Decision trees, pruning, constraint satisfaction

## Interview Best Practices

When solving problems in notebooks for interview prep:

1. **Communicate clearly**: Use markdown to explain your thought process
2. **Start simple**: Begin with brute force, then optimize
3. **Analyze complexity**: Always state time and space complexity
4. **Test thoroughly**: Include edge cases and walk through examples
5. **Multiple approaches**: Show different solutions and trade-offs
6. **Verbalize trade-offs**: Explain why you chose one approach over another

## Tools and Utilities

The notebooks include helper functions for:
- Verbose step-by-step execution
- Visual representations of data structures
- Performance comparison between approaches
- Test case generation and validation
