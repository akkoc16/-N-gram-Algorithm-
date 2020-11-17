
# N-gram-Algorithm
## n-gram Algorithm Implementation in Intel x86 Assembly

In this project, we implemented n-gram algorithm using Intel assembly. N-gram defines a
contagious sequence of n items (characters or samples) from any given information. It is commonly used
in natural language processing (NLP) to derive probabilistic models. 

N-gram function will take two strings and value of n as its main inputs parameters and will measure the similarity
of the given strings.

##### int n_gram(char* str_1, int size_1, char* str_2, int size_2, int n);

The function will first determine the sequence sets of given string, listing the n-grams they contain.
Let us use 𝑆′ and 𝑆′′ to specify sets beloning to the first and second input strings respectively. 
Lastly, our function use the similarity parameters calculated as its return value and conclude its
execution. It is important that you notice the return parameter of the function is declared as an
integer.

![N-gram](https://github.com/akkoc16/-N-gram-Algorithm-/blob/main/example.PNG)


## Implementation

``` 
nasm -f elf32 assembly.asm -o assembly.o
gcc -c last_main_asm.c -o last_main_asm.o
gcc assembly.o last_main_asm.o -o ngram
./ngram
```

