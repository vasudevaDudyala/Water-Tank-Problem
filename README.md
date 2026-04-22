# Water-Tank-Problem
Interactive Trapping Rain Water visualization using Vanilla JavaScript implementing O(n) prefix-suffix optimization with real-time UI rendering and dynamic water level display.

📌 Problem Statement

Given an array of non-negative integers representing the height of blocks, compute how much rainwater can be trapped after rainfall.

Each element represents the height of a bar, and water is trapped between taller bars.

🧠 Intuition

At any index, water trapped depends on:

Maximum height to the left
Maximum height to the right

Water level is determined by the smaller boundary.

📌 Core Formula
Water[i] = min(leftMax[i], rightMax[i]) - height[i]

🚀 Approach

This project uses an O(n) Prefix-Suffix Optimization approach.

Step 1: Input Processing
Accept comma-separated values from user input
Step 2: Precompute Boundaries
Compute leftMax[] → maximum height from left
Compute rightMax[] → maximum height from right
Step 3: Water Calculation
For each index, calculate trapped water using formula
Sum all contributions
Step 4: Visualization
Render bars using HTML/CSS
Overlay water using dynamic div heights


Input:

<img width="902" height="277" alt="image" src="https://github.com/user-attachments/assets/c73a0198-f837-471b-8911-b3bcf818b503" />

Output:

<img width="787" height="623" alt="image" src="https://github.com/user-attachments/assets/61b1b224-ffbf-4c3e-b9a9-1c9e0c6cbb32" />


