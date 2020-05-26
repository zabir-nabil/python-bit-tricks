# python-bit-tricks

source: https://graphics.stanford.edu/~seander/bithacks.html#ReverseParallel

Fastest bit manipulations, bit tricks, optimization code snippets in python

###### How many bits are different?

```
diff_bits = x ^ y
num_1s = bin(diff_bits).count('1')
```
