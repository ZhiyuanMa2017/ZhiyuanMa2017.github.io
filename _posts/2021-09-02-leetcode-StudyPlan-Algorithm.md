---
layout: post
title: LeetCode Study Plan Algorithm
tags:
  - LeetCode
  - Algorithm
---
#  Binary Search

#  Two Pointers

# Depth-First Search, DFS

#  Breadth-First Search, BFS

#  Dynamic Programming, DP

#  Backtracking

#  Bit Manipulation

1. &：

   ```mathematica
   0 & 0 = 0
   
   0 & 1 = 0
   
   1 & 0 = 0
   
   1 & 1 = 1
   ```

2. XOR:

   ```mathematica
   0 ^ 0 = 0 
   0 ^ 1 = 1 
   1 ^ 0 = 1 
   1 ^ 1 = 0
   ```

   ```mathematica
       0101 (decimal 5)
   XOR 0011 (decimal 3)
     = 0110 (decimal 6)
   ```

   ```mathematica
       0010 (decimal 2)
   XOR 1010 (decimal 10)
     = 1000 (decimal 8)
   ```

3. \|:

   ```mathematica
   0 | 0 = 0 
   
   0 | 1 = 1 
   
   1 | 0 = 1 
   
   1 | 1 = 1
   ```

4. &：

   ```mathematica
   0 & 0 = 0 
   0 & 1 = 0 
   1 & 0 = 0 
   1 & 1 = 1
   ```

5. ~：

   ```mathematica
   ~1 = 0 
   ~0 = 1
   ```

6. \<<：

   shifts a bit pattern to the left

   左边的二进制位丢弃，右边补0
   
   ```mathematica
   -1 = 11111111111111111111111111111111
   
   -1 << 31 = 10000000000000000000000000000000 = -2147483648
   
   -2147483648 << 1 = 0
   
   -1 << 32 = 11111111111111111111111111111111 = -1
   31 mod 32 = 0
   so, -1 << 32 = -1 << 0 = -1
   
   -1 << 31 << 1 = 0
   ```

7. \>>：

   shifts a bit pattern to the right, the bit pattern is given by the left-hand operand

   正数左补0，负数左补1，右边丢弃

8. \>>>：

   shifts a zero into the leftmost position

   忽略符号位，空位都以0补齐
