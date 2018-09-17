## mcj-fibonacci
使用Java實作費式數列。
### 費式數列
```
1, 1, 2, 3, 5 ...
第一個及第二個的值為1，後續接為前兩個值的總和，依此類推。
F(1) = 1
F(2) = 1
F(3) = F(1) + F(2) = 2
F(4) = F(2) + F(3) = 3
...
```
### Sample1
使用遞迴實作，但可以發現效能上有嚴重的問題。
基本F(n)消耗的時間會接近F(n - 2) + F(n - 1)的消耗時間，且會無限遞增下去！
### Sample2
改用單一迴圈實作，解決效能上的問題。
一併調整memory leak的問題。
