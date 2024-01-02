# Decoding-the-relations-between-Genes

## Introduction

In this report I provide the implementation of the longest common subsequence problem in decoding the relationships between gene sequences. The goal is to recover the genealogy tree for a given set of strings represeting the gene sequences including the parent gene and the resulting genes from the replication of that gene and its children.

## Key Functionalities

1. **Gene Relationship Analysis**: Identifies relationships between different genes based on the given DNA sequences.
2. **Visualization**: Provides visualizations of the relationships between genes.

## Approaches Used

1. **Dynamic Programming**: Used to find the longest common subsequence later used as a similarity metric between the genes.
2. **Greedy approach**: Used as the local strategy to build the genealogy binary tree based on the optimal LCS for each step.
3. **Brute Force**: Used as the global strategy to find build the tree.

## Data Structures Used

1. **Max Heap**: Used to store the DNA sequences and heapify them maintainting the max heap property.
2. **Binary Trees**: Created as a dictionary where each key is a node and the value corresponds to its children.

## Usage

Input the DNA Sequences to the Set_string as lists of 2 elemnts "the DNA sequence and its corresponding representative character".

call the function `generate_lcs_proportion_matrix2(set_strings)` with the set_string as input.

store the function's output in a variable say `lcs_proportion_matrix`

Call the function `build_tree_heap_all_nodes(lcs_proportion_matrix, set_strings)` to generate the genealogy binary tree.
