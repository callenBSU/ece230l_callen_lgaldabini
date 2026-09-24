# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

For this lab, we optimized circuits by using boolean equations derived from truth tables and KMaps. We first 
implemeted the truth table into a KMap to visualize the minterms and maxterms. We then group together both
sets and layed out a boolean equation. Once we created our equations, we implemented them into all
3 code files. Once done, we booted up Vivado and ran a successful simulation and board test. This lab showed
us the process of going from a truth table -> KMap -> Boolean -> Code -> Board. 

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
The groups of 1's or 0's were able to go over the edge because those edges have the same variables. For example,
a 4-variable KMap edges share that B/D is 0. Assuming F(A,B,C,D).

### Why are the names Sum of Products and Products of Sums?
Sum of products are named because they are represented multiple sets of products (AND gates) and adding them
together with OR gates (the +). The opposite is true for Products of Sums. In POS, the products (AND) is taken
from a combination of sums (OR gates).

### Open the test.v file – how are we able to check that the signals match using XOR?
It is able to check if the signals math using XOR because each LED specified in the file refers to the maxterm, 
minterm, or naive. If we're gonna use the XOR command to see if an LED is lighting up and the other isn't, we'll
be able to determine that there is a bug in the code.

