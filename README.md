# What is the purpose of the library
This libary is the result of an implementation for solving the equivalence problem for linear tree-to-word transducers from the field of automaton theory. However, on the way to the solution a lot of interesting algorithm were implemented. Some basic algorithm such as the equivalence test for finite deterministic word automaton and more complex algorithms for example a fast equivalence test for SLP-compressed words. The goal of the project was to implement an algorithm with polynomial time complexity for testing the equivalence of linear tree-to-word transducers. 

## Equivalence test for SLP-compressed words
To achieve this goal it was necessary to implement a fast equivalence test for straight line programs (SLPs). These SLPs are special context-free grammars generating only one word. They are used to compress text. The implementation is based on the paper [Faster fully compressed pattern matching by recompression](https://arxiv.org/abs/1111.3244).

## The Morphism Equivalence Problem for Context-free Languages
The next step was to solve the morphism equivalence problem for context free languages which is decribed in the [Ph.D. thesis](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.36.8729&rep=rep1&type=pdf) of Wojciech Plandowski. However, we accelerate the equivalence test of SLPs by using the algorithm introduced by Arthur Jez. 

## The Equivalence Problem for Sequential Tree-to-word Transducers
It is possible to reduce the equivalence problem of sequential tree-to-word transdsequential tree-to-word transducersucers to the morphism equivalence test of context-free grammars which is decribed by in this [paper](http://www.grappa.univ-lille3.fr/~staworko/papers/staworko-fct09.pdf).

## Equivalence test for Linear Tree-to-Word Transducers
The last step was to reduce the orignal problem to the equivalence problem. This reduction is described in [Deciding Equivalence of Linear Tree-to-Word Transducers in Polynomial Time](https://arxiv.org/abs/1606.03758). 
