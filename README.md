# This note is writen by @[Neptune_EX](https://github.com/Neptune-EX)

## DATA_LAB 数字的表示 20260817

1. 针对负数表示的数字的计算方法:

$$
\text{Value} = sign \times (-2^{31}) + \sum_{i=0}^{30} b_i \times 2^i
$$

2. 补码和相反数的等效性:

$$
    x+(\sim x)=\text{0xFFFFFFFF}=-1 \\
    x+(\sim x)+1=0 \\
$$

3. n位最多表示的数字：

- howManyBits(12) = 5
- howManyBits(298) = 10
- howManyBits(-5) = 4
- howManyBits(0)  = 1
- howManyBits(-1) = 1
- howManyBits(0x80000000) = 32
$$
    - (2^{(n-1)}) \to 2^{(n-1)} 共计2^n个数字
$$

其中：
- 最小负数：1000_0000_0000_0000_0000_0000_0000_0000
- 最大负数：1111_1111_1111_1111_1111_1111_1111_1111

同时，针对某个负数$x$，用于表示该数所需的最少的位数与$\sim x$相同，及其相反数-1.




