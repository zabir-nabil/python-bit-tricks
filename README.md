# python-bit-tricks

source: https://graphics.stanford.edu/~seander/bithacks.html#ReverseParallel

Fastest bit manipulations, bit tricks, optimization code snippets in python

###### How many bits are different?

```
diff_bits = x ^ y
num_1s = bin(diff_bits).count('1')
```

##### Turning on bit, getting the status of bitmask at position `i`

```
bitmask = bitmask | (1 << i) # initially, bitmask is 0
```

```
status = bitmask & (1 << i) # if status is 0, the bit is unset, else [value of status can be 1, 2, 4, 8, ...] the bit is set
```
