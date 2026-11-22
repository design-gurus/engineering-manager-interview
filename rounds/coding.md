# The Coding Round for Engineering Managers

Some companies ask engineering manager candidates to write code, and some do not. Where the round exists, it is usually one 45-minute session with one or two problems of easy to medium difficulty. The interviewer is not looking for the fastest solution. The round checks that the manager can still reason about code, because a manager who cannot will struggle to review designs, judge estimates, or earn the trust of the team.

## Who gets a coding round

The table describes commonly reported practice. Always confirm with the recruiter.

| Situation | Coding round |
|---|---|
| First-line manager at a large technology company | Likely, one round |
| Manager expected to contribute code part of the time | Very likely, sometimes two rounds |
| Senior manager with managers reporting to them | Sometimes, often replaced by a second design round |
| Director and above | Rare |
| Small startup hiring its first manager | Likely, sometimes as a take-home exercise |

Ask the recruiter three questions: whether there is a coding round, which language is allowed, and whether the difficulty matches the engineer loop.

## What is graded

| Signal | Weight for a manager |
|---|---|
| Asks about inputs, limits, and edge cases before coding | High |
| Explains the approach before writing it | High |
| Produces working, readable code | High |
| States time and space complexity correctly | Medium |
| Finds the optimal solution | Lower than in an engineer loop |
| Tests the code with an example | High |

A manager who communicates well and delivers a correct, simple solution usually passes. A manager who is silent for 20 minutes usually does not, even with an optimal answer.

## What to study

Managers rarely have time to solve several hundred problems. Studying by pattern is more efficient. A pattern is a reusable approach that solves a family of problems, such as two pointers or breadth-first search.

| Priority | Topics | Suggested problems |
|---|---|---|
| 1 | Arrays, strings, hash maps, two pointers, sliding window | 15 |
| 2 | Trees and graphs with breadth-first and depth-first search | 12 |
| 3 | Stacks, queues, heaps, intervals, binary search | 10 |
| 4 | Basic dynamic programming and backtracking | 5 |

About 40 problems over four weeks, with every solution explained aloud, is a realistic target for a working manager.

## A 45-minute plan

| Minutes | Step |
|---|---|
| 0 to 5 | Restate the problem and ask about input size and edge cases |
| 5 to 10 | Describe a simple approach and its complexity, then a better one if you see it |
| 10 to 30 | Write the code while explaining each block |
| 30 to 38 | Walk through one normal example and one edge case |
| 38 to 45 | Discuss complexity and how you would test it in production |

## Common mistakes

- Assuming there is no coding round and learning otherwise two days before the onsite.
- Practicing silently. The explanation is half of the grade.
- Choosing a language you have not written in for years.
- Saying "I would delegate this" during the round.

## Go deeper

- [Grokking the Engineering Manager Coding Interview](https://www.designgurus.io/course/grokking-the-engineering-manager-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-coding) is a pattern-based problem set sized for the manager loop.
- Lesson: [Subarray Sum Equals K (medium)](https://www.designgurus.io/course-play/grokking-the-engineering-manager-coding-interview/doc/subarray-sum-equals-k-medium?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-coding), in Grokking the Engineering Manager Coding Interview
- Lesson: [Technical Skills for Engineering Managers](https://www.designgurus.io/course-play/grokking-the-engineering-manager-interview/doc/technical-skills-for-engineering-managers?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-coding), in Grokking the Engineering Manager Interview
- [Grokking the Engineering Manager Interview](https://www.designgurus.io/course/grokking-the-engineering-manager-interview?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-coding) covers the technical skills a manager is expected to keep.
- Related page: [System design for managers](system-design-for-managers.md).
