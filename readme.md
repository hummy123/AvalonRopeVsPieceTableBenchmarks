# Piece Table vs Avalon Rope Benchmarks

## Introduction

This repository contains benchmarks for one component of a personal project, which involved implementing a Piece Table (a data structure used to allow efficient string insertion and deletion) in F# and a comparison with a data structure called a Rope (written in C#) used for the same purpose.

I won't bore with a discussion of the benchmark results - the .md files at the root of this repository do a good enough job at showing the performance differences. However, a few non-obvious remarks may be helpful to anyone viewing this repository.

1. These benchmarks shouldn't be taken as a definitive answer for the superior performance of one structure over the other.
  - This particular Rope is a mutable data structure while the Piece Table is immutable, and mutable/immutable structures often have difference performance characteristics.
2. This Rope may be regarded as slightly non-standard due to storing char values at each leaf rather than strings [unlike the diagram illustrating Ropes on Wikipedia](https://en.wikipedia.org/wiki/Rope_(data_structure)).
  - This Piece Table is somewhat non-standard as well. It is implemented as a linked list with a zipper, meaning that (like a splay tree) operations on nodes close to each other execute more quickly. 
3. The benchmark files numbered 4 and 5 illustrate two features of this particular Piece Table: Consolidation and Merging.
  - A Piece Table's worst case is when we have inserted into the middle of a string many times and subsequently have many pieces in the table. The Consolidation function rebuilds the table in O(n log n) time so that operations are fast again.
    - The Consolidate function was intended to be run in a multi-threaded manner after every appreciable keystroke delay, which is safe to do because of this Piece Table's immutability. This always keeps the structure's performance at the best case.
    - The Merge function "extends" a piece when we type contiguously rather than inserting a new piece into the table. This helps avoid the worst case when the table has many pieces.