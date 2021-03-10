# Leetcode 344 Reverse String
###### tags: `Leetcode`
![](https://i.imgur.com/pmNVO70.png)

Solution1:
```
public class Solution {
    public void ReverseString(char[] s) {
       
        int left = 0,right = s.Length-1;
        while(left<right){
            char tmp=s[left];
            s[left++]=s[right];
            s[right--] = tmp;
        }
    
    }
}
```
Solution2:
```
public class Solution {
    public void ReverseString(char[] s) {
       
       Array.Reverse(s);
    
    }
}
```
Mark:These two solutions get almost the same runtime and memory

hint:
![](https://i.imgur.com/XXnrp3z.png)
* ref : https://leetcode.com/problems/reverse-string/