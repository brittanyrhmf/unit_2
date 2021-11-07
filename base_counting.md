Define the function as base_count with input b (base)

Create n in range(0,101) - to do the 100 numbers

Create empty string - to store answer

org_numb = n (to include that number in the output)

If n is 0 just add “0” to answer string

While n is more than 0:
Concatenate to string the remainder of n / b (using modulus: %)

n has new value of itself floor divide by the base

Print the concatenated string but inverted using slicing (because we read bottom to top) in a line like “f’{org_num} in decimal, with a base {b} is {n}’”

code:
