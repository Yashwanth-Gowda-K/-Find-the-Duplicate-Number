# -Find-the-Duplicate-Number


## 🚀 Problem Statement
Given an array `nums` containing `n + 1` integers where each integer is between `1` and `n` (inclusive), find:
- The duplicate number (guaranteed to exist)
- Without modifying the original array
- Using only constant extra space (O(1))
- With linear runtime complexity (O(n))

## 🧠 Algorithm Overview
### Floyd's Tortoise and Hare Approach
1. **Phase 1 (Cycle Detection):**
   - Slow pointer moves 1 step (`nums[slow]`)
   - Fast pointer moves 2 steps (`nums[nums[fast]]`)
   - They must meet inside the cycle

2. **Phase 2 (Duplicate Detection):**
   - Reset slow pointer to start
   - Move both pointers 1 step at a time
   - Next meeting point is the duplicate number

## ⚡ Complexity Analysis
| Metric       | Performance |
|--------------|-------------|
| Time         | O(n)        |
| Space        | O(1)        |
| Array Access | Read-only   |
