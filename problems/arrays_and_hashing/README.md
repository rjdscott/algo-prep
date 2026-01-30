# Arrays & Hashing

This is the foundational pattern for coding interviews. Master these problems first before moving to other patterns.

## Core Concepts

- **Hash Tables/Maps**: O(1) lookup, insertion, deletion
- **Hash Sets**: Unique element tracking, duplicate detection
- **Frequency Counting**: Character/element frequency maps
- **Array Traversal**: Single pass, two pass algorithms
- **Index Manipulation**: Using array indices as hash keys

## Problems (Easy → Medium → Hard)

### Easy - Start Here

- ✓ `217_contains_duplicate.ipynb` - Hash set basics
- ✓ `242_valid_anagram.ipynb` - Frequency counting
- ✓ `001_two_sum.ipynb` - Hash map for complements
- `217_contains_duplicate_ii.ipynb` - Sliding window with hash map (if added)
- `383_ransom_note.ipynb` - Frequency map comparison (if added)

### Medium

- `049_group_anagrams.ipynb` - Hash map with custom keys
- `347_top_k_frequent_elements.ipynb` - Frequency + sorting/heap
- `238_product_of_array_except_self.ipynb` - Prefix/suffix products
- `271_encode_decode_strings.ipynb` - String manipulation
- `128_longest_consecutive_sequence.ipynb` - Hash set with O(n)
- `036_valid_sudoku.ipynb` - Multiple hash sets

### Hard

- `041_first_missing_positive.ipynb` - Index as hash key
- `316_remove_duplicate_letters.ipynb` - Hash map + stack

## Key Patterns

### 1. Hash Map for Complements/Pairs
```python
seen = {}
for i, num in enumerate(nums):
    complement = target - num
    if complement in seen:
        return [seen[complement], i]
    seen[num] = i
```

### 2. Frequency Counting
```python
from collections import Counter
freq = Counter(array)
# or manually:
freq = {}
for item in array:
    freq[item] = freq.get(item, 0) + 1
```

### 3. Hash Set for Uniqueness
```python
seen = set()
for item in array:
    if item in seen:
        return True
    seen.add(item)
```

### 4. Using Index as Hash
```python
# For arrays with values in range [1, n]
for i in range(len(nums)):
    idx = abs(nums[i]) - 1
    if nums[idx] < 0:
        # Found duplicate
    nums[idx] = -nums[idx]
```

## Interview Tips

1. **Always consider hash maps/sets first** - They solve most array problems optimally
2. **Clarify input constraints** - Can help optimize space (e.g., fixed character set)
3. **Think about trade-offs** - Hash maps trade space for time (O(n) space for O(1) lookup)
4. **Handle edge cases**:
   - Empty arrays
   - Single element
   - All duplicates
   - No duplicates
   - Negative numbers
   - Large numbers

## Time Complexity Goals

Most array & hashing problems can be solved in:
- **Time**: O(n) or O(n log n)
- **Space**: O(n) or O(1)

If your solution is O(n²), look for a hash map optimization.

## Common Mistakes

1. **Not checking if key exists** before accessing hash map
2. **Forgetting early termination** checks (e.g., length mismatch)
3. **Modifying array while iterating** without careful index management
4. **Not handling duplicates** properly in hash maps

## Study Order

1. Start with easy problems to master hash map/set basics
2. Progress to medium problems with multiple hash structures
3. Focus on time/space complexity analysis
4. Practice explaining your approach out loud

## Related Patterns

After mastering arrays & hashing, these patterns build on similar concepts:
- **Two Pointers** - Often combined with hash maps
- **Sliding Window** - Uses hash maps for substring problems
- **Graphs** - Hash maps for adjacency lists
- **Dynamic Programming** - Memoization uses hash maps
