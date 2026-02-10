# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

A study repository for LeetCode Hot 100 problems. Content is written in Chinese. Solutions use Python.

## Structure

Problems are organized by algorithm category, each category being a top-level directory with a Chinese name:

- Each category has a `README.md` containing: core concepts, common patterns for that category, and a problem tracking table (checkbox-style)
- Each problem is a separate markdown file named after the problem in Chinese (e.g., `两数之和.md`)

### Categories (directory names)

哈希, 双指针, 滑动窗口, 子串, 普通数组, 矩阵, 链表, 二叉树, 图论, 回溯, 二分查找, 栈, 堆, 贪心算法, 动态规划, 多维动态规划, 技巧

## Problem File Format

Each problem markdown follows this structure:

1. **Title** (H1) + difficulty
2. **题目** - Problem statement
3. **示例** - Examples with input/output
4. **解法** - Solutions (brute force first, then optimal with ✓ mark)
5. **复杂度** - Time and space complexity
6. **要点** - Key takeaways

Code blocks use Python with type hints (e.g., `List[int]`), written as class methods (`self` parameter) matching LeetCode's submission format.

## Category README Format

Each category README contains:
1. **核心思想** - Core concept of the category
2. Relevant Python data structures/APIs table
3. **常见套路** - Common patterns
4. **本专题题目** - Problem tracking table with links, difficulty, and completion status (✅/⬜)

## Learning Workflow

When the user says "下一题" or specifies a problem name, follow this flow:

1. **出题**：描述题目和示例，然后问用户的思路
2. **引导**：让用户用自己的话描述解题思路，不要直接给答案
3. **纠正/补充**：对用户的思路给出反馈，指出问题或肯定方向，逐步引导到正确解法
4. **写代码**：让用户自己尝试写代码，review 用户写的代码，指出语法或逻辑错误
5. **追问优化**：如果有更优解法，引导用户思考（而不是直接告诉）
6. **记录**：用户理解后，将题解写入 markdown 文件并更新 category README

重点：这是学习仓库，目的是让用户主动思考，不是直接给答案。

## Conventions

- All prose in Chinese
- Problem difficulty labels: 简单 (Easy), 中等 (Medium), 困难 (Hard)
- When adding a new problem: create the problem `.md` file and update the category `README.md` tracking table (change ⬜ to ✅, add link)
- When creating a new category directory: include a `README.md` with the format described above before adding problems
