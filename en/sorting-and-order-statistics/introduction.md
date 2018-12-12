## Introduction

This part presents several algorithms that solve the following sorting problem:

Input: A sequence of n numbers [a1, a2, ..., an].  
Output: A permutation (reordering) [a'1, a'2, ..., a'n] of the input sequence such
that a'1 <= a'2 <= ... <= a'n.  
The input sequence is usually an n-element array, although it may be represented
in some other fashion, such as a linked list.

### The structure of the data

In practice, the numbers to be sorted are rarely isolated values. Each is usually part
of a collection of data called a record. Each record contains a key, which is the
value to be sorted. The remainder of the record consists of satellite data, which are
usually carried around with the key. In practice, when a sorting algorithm permutes
the keys, it must permute the satellite data as well. If each record includes a large
amount of satellite data, we often permute an array of pointers to the records rather
than the records themselves in order to minimize data movement.
