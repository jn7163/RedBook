# 运算次序

除了中缀运算优先于前缀调用外，表达式总是按从左到右的次序运算。

```
1 + 2 * 3                              ;-- (1 + 2) * 3 returns 9
1 + 2 * 3 = 9                          ;-- ((1 + 2) * 3) = 9 returns TRUE
9 = 1 + 2 * 3                          ;-- ((9 = 1) + 2) * 3 raises an error!

1 + (2 * 3)                            ;-- 1 + (2 * 3) returns 7

foo 1 + 2                              ;-- foo (1 + 2)
1 + foo 2 * 3                          ;-- 1 + (foo (2 * 3))
```
