# LC-26
Remove Duplicates from Sorted Array
```ruby
class Solution {
public:
    int removeDuplicates(vector<int>& v) {
        int n = 1;
        for(int i=1;i<v.size();i++)
        {
            if(v[i-1]!=v[i])
            {
               v[n] = v[i];
               n++;
            }
        }
        return n;
    }
};
```
