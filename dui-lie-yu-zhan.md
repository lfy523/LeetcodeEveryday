# 队列与栈

## 队列

队列，先进先出结构，有双端队列，优先队列等。这部分先总结一些经典题目。

{% tabs %}
{% tab title="387" %}
## **给定一个字符串 `s` ，找到 **_**它的第一个不重复的字符，并返回它的索引**_** 。如果不存在，则返回 `-1` 。**

利用两个set，第一个判断是否重复，若重复放入第二个set。

```cpp
#include <set>
class Solution {
public:
    int firstUniqChar(string s) {
        set<char> container, repeat;
        for(int i = 0; i < s.length(); i++){
            if (container.count(s[i]) == 0){
                container.insert(s[i]); // 判断是否重复
            }
            else{
                repeat.insert(s[i]); //若重复放入重复set
            }
        }
        for(int i = 0; i < s.length(); i++){
            if (repeat.count(s[i]) != 1){ // 判断该元素是否重复
                return i;
            }
        }        
        return -1;
    }
};
```
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}

{% tab title="Untitled" %}

{% endtab %}

{% tab title="Untitled" %}

{% endtab %}

{% tab title="Untitled" %}

{% endtab %}
{% endtabs %}



