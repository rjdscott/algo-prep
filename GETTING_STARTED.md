# Getting Started with Algorithm Interview Prep

Welcome! This guide will help you get started with your coding interview preparation.

## Quick Start

### 1. Set Up Your Environment

```bash
# Clone/navigate to the repository
cd algo-prep

# Create virtual environment
python -m venv venv

# Activate it
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Lab
jupyter lab
```

### 2. Start with the Right Category

**If you're new to coding interviews**, start here:
1. `problems/arrays_and_hashing/` - Foundation for everything else
2. `problems/two_pointers/` - Essential pattern
3. `problems/sliding_window/` - Common in interviews

**If you have limited time** (< 2 weeks), focus on:
- Arrays & Hashing (top 10 problems)
- Two Pointers (top 5 problems)
- Binary Search (top 5 problems)
- Trees (DFS/BFS basics)

**If you're targeting specific companies**:
- FAANG: Focus on Medium problems across all categories
- Startups: Focus on Easy/Medium, emphasize practical solutions
- Trading Firms: Add Math & Geometry, Bit Manipulation

### 3. Your First Problem

Open `problems/arrays_and_hashing/217_contains_duplicate.ipynb`

This is a perfect first problem because:
- Simple to understand
- Multiple approaches (sorting vs hash set)
- Teaches fundamental trade-offs (time vs space)
- Common interview question

## Study Strategy

### Week-by-Week Plan (8 weeks)

**Week 1-2: Foundations**
- Arrays & Hashing (Easy problems)
- Goal: 10-15 problems

**Week 3: Core Patterns**
- Two Pointers
- Sliding Window
- Goal: 10-15 problems

**Week 4: Search & Stack**
- Binary Search
- Stack
- Goal: 10-15 problems

**Week 5: Data Structures**
- Linked List
- Trees (focus on DFS/BFS)
- Goal: 10-15 problems

**Week 6: Advanced Patterns**
- Backtracking
- Heap/Priority Queue
- Goal: 8-12 problems

**Week 7: Dynamic Programming**
- 1D DP
- Start 2D DP
- Goal: 8-12 problems

**Week 8: Review & Mock Interviews**
- Redo problems you struggled with
- Practice explaining solutions out loud
- Time yourself (45 min per problem)

## Daily Study Routine

### Recommended: 2-3 hours/day

**Hour 1: New Problem**
1. Read problem (5 min)
2. Think about approach without coding (10 min)
3. Code brute force solution (15 min)
4. Optimize and code better solution (30 min)

**Hour 2: Understanding**
1. Compare with notebook solutions
2. Study different approaches
3. Understand time/space complexity
4. Run through edge cases

**Hour 3 (Optional): Related Work**
1. Solve a related problem
2. Review previous problems
3. Write notes on patterns you learned

## How to Use the Notebooks

### 1. First Attempt (Before Looking at Solutions)
- Read the problem statement
- Think about approaches (write notes)
- Try to code a solution in a new cell
- Test your solution

### 2. Learn from Solutions
- Compare your approach with the notebook
- Understand why each approach works
- Study the complexity analysis
- Run the verbose walkthroughs

### 3. Practice Explaining
- Pretend you're in an interview
- Explain the problem out loud
- Walk through your approach step-by-step
- Discuss trade-offs

### 4. Test Your Understanding
- Close the notebook
- Try to solve again from memory
- Explain it to someone else
- Write your own test cases

## Tracking Your Progress

Create a simple spreadsheet or markdown file:

```markdown
| Problem | Date | First Attempt | Optimal? | Review Date |
|---------|------|---------------|----------|-------------|
| Two Sum | 1/15 | Hash map ✓    | Yes      | 1/22        |
| Contains Duplicate | 1/15 | Sort | No (should use set) | 1/22 |
```

Mark problems for review if you:
- Couldn't solve it within 45 minutes
- Didn't get optimal solution
- Struggled with edge cases
- Need to review the pattern

## Red Flags & How to Fix Them

**🚩 You can't explain your solution clearly**
→ Practice talking through problems out loud

**🚩 You get the brute force but can't optimize**
→ Study the "Key Patterns" sections in each category README

**🚩 You make lots of syntax errors**
→ Practice coding by hand, then type it out

**🚩 You forget edge cases**
→ Create a checklist: empty input, single element, duplicates, negatives, max values

**🚩 You can't estimate time complexity**
→ Review the complexity analysis sections, count loops and operations

## Mock Interview Practice

After completing 40-50 problems, start mock interviews:

1. **Self-Timed**: Pick a random medium problem, give yourself 45 min
2. **With a Friend**: Take turns being interviewer
3. **Platforms**: Use Pramp, interviewing.io, or similar
4. **Record Yourself**: Watch to improve communication

## Key Success Metrics

You're ready for interviews when you can:

✓ Solve most Easy problems in < 20 minutes
✓ Solve most Medium problems in < 45 minutes
✓ Clearly explain your approach before coding
✓ Identify time/space complexity immediately
✓ Generate edge cases quickly
✓ Recognize which pattern to apply within 5 minutes

## Resources Beyond This Repo

- **NeetCode.io**: Video explanations for all problems
- **LeetCode Discuss**: Community solutions and patterns
- **AlgoExpert**: Additional problems and explanations (paid)
- **Cracking the Coding Interview**: Classic book with more context

## Common Questions

**Q: Should I memorize solutions?**
A: No. Focus on understanding patterns. You should be able to derive solutions.

**Q: How many problems do I need to solve?**
A: Quality > Quantity. 100-150 problems understood deeply beats 300 done superficially.

**Q: What if I can't solve a problem?**
A: That's normal! Give yourself 30-45 min, then look at hints/solutions. The learning happens when you study the solution.

**Q: Should I do all problems in each category?**
A: No. Focus on variety. Do 10-15 per category to learn patterns, then move on.

**Q: How do I know which approach to use?**
A: Pattern recognition comes with practice. The category READMEs list common patterns.

## Getting Help

If you're stuck:
1. Read the problem constraints carefully (they hint at the approach)
2. Check the pattern hints in the category README
3. Look at the "Initial Observations" section
4. Try the brute force approach first
5. Study the notebook's explanations

## Final Tips

- **Consistency beats intensity**: 1-2 hours daily beats 10 hours on weekends
- **Understand, don't memorize**: Focus on why, not what
- **Practice explaining**: Communication matters as much as coding
- **Review regularly**: Spaced repetition is key
- **Stay positive**: Everyone struggles at first

Good luck with your interview prep! 🚀
