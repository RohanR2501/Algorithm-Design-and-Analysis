# SC2001-Lab-Projects
## SC2001 Project 1 — Hybrid Mergesort + Insertion Sort

### Introduction
In Mergesort, when the sizes of subarrays are small, the overhead of many recursive
calls makes the algorithm rather inefficient. Therefore in real use cases, we often combine
Mergesort with Insertion Sort to come up with a hybrid sorting algorithm for better efficiency.

The idea is to set a small integer **S** as a threshold for the size of subarrays.
Once the size of a subarray in a recursive call of Mergesort is less than or equal to S,
the algorithm will switch to Insertion Sort, which is efficient for smaller-sized inputs.

This project implements and analyzes such a hybrid algorithm, and compares it with
the original Mergesort.
