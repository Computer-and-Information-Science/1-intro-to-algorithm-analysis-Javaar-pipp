# CISC230 - Javaar Pippinger

## factorial2.cpp

- input/parameter impacting number of calls:

The variable "num" which is then passed as "n" to factorial function.
The number inputted + 1 will determine the number of calls.

- 3 specific examples of input/parameter and number of calls:

input 2 = -> called 3 times.

input 3 = -> called 4 times.

input 4 = -> called 5 times.

- number of recursive calls when input/parameter is *n*:

n = number inputted.

f(n) = n + 1 = number of recursive calls

## ireverse2.cpp

- input/parameter impacting number of calls:

The variable "num" which is then passed as "n" to the ireverse function.
The number of integers inputted will determine the number of calls + one.

- 3 specific examples of input/parameter and number of calls:

input 12 = -> called 3 times.

input 123 = -> called 4 times.

input 1234 = -> called 5 times.

- number of recursive calls when input/parameter is *n*:

n = amount of integers inputted(123 = 3 integers).

f(n) = n + 1 = Total calls

## sreverse2.cpp

- input/parameter impacting number of calls:

The variable "str" which is then passed as "s" to the sreverse function.
The length of the string will determine how many calls are made.

- 3 specific examples of input/parameter and number of calls:

input "to" = -> called 2 times.

input "hello" = -> called 5 times.

input "sky" = -> called 3 times.

- number of recursive calls when input/parameter is *n*:

n = length of the string.

f(n) = n = Total calls

## permute.cpp

- input/parameter impacting number of calls:

The variable "s" which is then passed as "str" to the permute function. The length of the string will determine how many times the function permute is called.

- 3 specific examples of input/parameter and number of calls:

input "ab" = -> called 5 times.

input "abc" = -> called 16 times.

input "abcd" = -> called 65 times.

input "abcde" = -> called 326 times.

- number of recursive calls when input/parameter is *n*:

n = length of string

f(n) = n*f(n-1) + 1 

## tower.cpp

- input/parameter impacting number of calls:

The variable "n" which is then passed as "n_disks" to the tower function. The larger the value of "n_disk" the more calls to the fucntion are made.

- 3 specific examples of input/parameter and number of calls:

input 1 = -> called 3 times.

input 3 = -> called 15 times.

input 10 = -> called 2047 times.

- number of recursive calls when input/parameter is *n*:

I used a global variable to tally the number of calls as the call stack grew too fast to tally by hand. I then created a table with all the inputs between 1-10 and looked for the pattern.

n = number of disk entered.

f(n) = 2^(n+1) - 1 = Total calls

## fibonacci2.cpp (presented in video lesson)

- input/parameter impacting number of calls:

The global variable "N" and the "i" variable control how many times the function is called. The i variable loops and counts up to N, each loop calls the fib function. 

- 3 specific examples of input/parameter and number of calls:

parameter (const unsigned int N) 3 = -> called 5 times.

parameter (const unsigned int N) 4 = -> called 8 times.

parameter (const unsigned int N) 5 = -> called 11 times.

Note: This function is hard to map how many calls will be made at any number; but it appears to about double. Every sequence of 10 however produces a distinct formula below the main one.

parameter (const unsigned int N) 20 = -> called 56 times.

parameter (const unsigned int N) 30 = -> called 86 times.

parameter (const unsigned int N) 80 = -> called 236 times.

- number of recursive calls when input/parameter is *n*:

n = global "n" variable.

f(n) = n * 2 = Total calls

f(n) = (n * 3) - 4 = Total number of calls/(formula for sequence of 10s)
