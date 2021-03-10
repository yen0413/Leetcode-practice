# Leetcode 509 Fibonacci Number
###### tags: `Leetcode`
![](https://i.imgur.com/NKYV77D.png)

Solution1:
```
public class Solution {
    public int Fib(int n) 
    {
        if(n<=1){return n;}
    
        int first = 0;
        int second = 1;
        for(int i =2;i<=n;i++)
        {
            int sum = first+second;
            first = second;
            second = sum;
        }
        return second;
    }
}
```
Solution2(遞迴Recursion):
```
public class Solution {
    public int fib(int N) {
        if (N <= 1) {
            return N;
        }
        return fib(N-1) + fib(N-2);
    }
}
```
hint:
![](https://i.imgur.com/31riEOO.png)
* ref : https://leetcode.com/problems/fibonacci-number/