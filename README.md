# The Hamming difference

Write a program that can calculate the Hamming difference between two DNA strands.

A mutation is simply a mistake that occurs during the creation or copying of a nucleic acid, in particular DNA. Because nucleic acids are vital to cellular functions, mutations tend to cause a ripple effect throughout the cell. Although mutations are technically mistakes, a very rare mutation may equip the cell with a beneficial attribute. In fact, the macro effects of evolution are attributable by the accumulated result of beneficial microscopic mutations over many generations.
The simplest and most common type of nucleic acid mutation is a point mutation, which replaces one base with another at a single nucleotide.
By counting the number of differences between two homologous DNA strands taken from different genomes with a common ancestor, we get a measure of the minimum number of point mutations that could have occurred on the evolutionary path between the two strands.
This is called the 'Hamming distance'.

It is found by comparing two DNA strands and counting how many of the nucleotides are different from their equivalent in the other string.
```
1 GAGCCTACTAACGGGAT
2 CATCGTAATGACGGCCT
3 ^ ^ ^  ^ ^    ^^
The Hamming distance between these two DNA strands is 7.
```

adenine (A)
guanine (G)
thymine (T)
cytosine (C)

## Your job

1/ Install PHPUnit

2/ Create in the `src/` folder the `Hamming` class composed of a `distance()` method which will take as parameters the two DNA strands to be compared and will return the difference.

3/ Create in the `tests/` folder the `HammingTest` class allowing to perform the following tests:

```
test1  
strand A : GAGCCTACTAACGGGAT  
strand B : CATCGTAATGACGGCCT  
result : 7

test2  
strand A: CCGCAAATACTAACGCG  
strand B: CATCGTAATGACGGCCT  
result: 13

test3  
strand A: ACCTTGAAGTCAGCGCT  
strand B: CATCGTAATGACGGCCT  
result: 12

test4    
strand A: AGCCTTGAATCAGCGCT  
strand B: CATCGTAATGACGGCCT  
result : 11
```

4/ Write the logic of the `distance()` method
