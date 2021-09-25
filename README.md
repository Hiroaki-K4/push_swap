# push_swap
This project will make you sort data on a stack, with a limited set of instructions, using the lowest possible number of actions. To succeed you’ll have to manipulate various types of algorithms and choose the one (of many) most appropriate solution for an optimized data sorting. While using the two stacks A and B, perform the following operations to sort.

- sa : swap a - swap the first 2 elements at the top of stack a. Do nothing if there is only one or no elements).
- sb : swap b - swap the first 2 elements at the top of stack b. Do nothing if there is only one or no elements).
- ss : sa and sb at the same time.
- pa : push a - take the first element at the top of b and put it at the top of a. Do nothing if b is empty.
- pb : push b - take the first element at the top of a and put it at the top of b. Do nothing if a is empty.
- ra : rotate a - shift up all elements of stack a by 1. The first element becomes the last one.
- rb : rotate b - shift up all elements of stack b by 1. The first element becomes the last one.
- rr : ra and rb at the same time.
- rra : reverse rotate a - shift down all elements of stack a by 1. The last element becomes the first one.
- rrb : reverse rotate b - shift down all elements of stack b by 1. The last element becomes the first one.
- rrr : rra and rrb at the same time.

<br>

# My score
![push_swap](https://user-images.githubusercontent.com/51109408/128590165-3d7ef78e-5ba0-4273-b318-c583bde2c0d9.png)

<br>

# Sort algorithm(Quick sort)
I used [quicksort](https://www.geeksforgeeks.org/quick-sort/) as the sorting algorithm.

<br>

# How to build
Build the files.

```
make
```
Rebuild
```
make re
```
Clean .o files
```
make clean
```
Clean all files
```
make fclean
```

# How to run
Executing the command below will output the operation used to sort.
```
ARG="4 67 3 87 23"; ./push_swap $ARG
```
The command below prints the number of operations used to sort.
```
ARG="4 67 3 87 23"; ./push_swap $ARG | wc -l
```
Run the command below to check if the operation used to sort is correct. If the answer is correct, OK is output, and if it is incorrect, KO is output. The checker file is for Mac. Use checker_linux in Linux environment.
```
ARG="4 67 3 87 23"; ./push_swap $ARG | ./checker $ARG
```
