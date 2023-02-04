## Note
1. The gas savings given are based on the examples l've written and tested with foundry. 
2. They might not be accurate for your codebase and the best way to see how much gas you can save is by testing them yourself.

You can test them easily with the help of - https://github.com/0xKitsune/gas-lab


# Gas Optimizations Template

| Count | Explanation | Gas saved |
|:--:|:-------|:--:|
| G-01 | ++i costs less gas than i++, especially when it's used in for-loops (--i/i-- too) | 26 |
| G-02 | Cache array length outside of loop | 192 |
| G-03 | += costs more gas than = + for state variables | 38 |
| G-04 | i++ in for-loops should be unchecked, as overflow is impossible | 213 |

