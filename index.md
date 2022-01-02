## Welcome to Septer's LeetCode Note

This GitHub page will be used to store the submission records and experience notes of chapter's learning and training on LeetCode. You can also visit [my GitHub home page](https://github.com/Septerxy).

### Easy

## No.1

#Title
```
**两数之和**
```
#Answer
```
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        vector<int> res;
        for(int i=0;i<nums.size();i++)
        {
            for(int j=i+1;(j<nums.size())&&(j!=i);j++)
                if(nums[i]+nums[j]==target)
                {
                    res.push_back(i);
                    res.push_back(j);
                    break;
                }
        }
        return res;
    }
};
```
#Note
```
test
```

### Medium

### Difficult


### MoreInfo
For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Septerxy/LeetCode.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
