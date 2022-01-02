## Welcome to Septer's LeetCode Note

This GitHub page will be used to store the submission records and experience notes of chapter's learning and training on LeetCode. You can also visit [my GitHub home page](https://github.com/Septerxy).

## Easy

### No.1

**Title**
```
两数之和
给定一个整数数组 nums 和一个整数目标值 target，请你在该数组中找出 和为目标值 target 的那 两个 整数，并返回它们的数组下标。 
你可以假设每种输入只会对应一个答案。但是，数组中同一个元素在答案里不能重复出现。 
你可以按任意顺序返回答案。 

示例 1： 
输入：nums = [2,7,11,15], target = 9 
输出：[0,1] 
解释：因为 nums[0] + nums[1] == 9 ，返回 [0, 1] 。 

示例 2： 
输入：nums = [3,2,4], target = 6 
输出：[1,2] 

示例 3： 
输入：nums = [3,3], target = 6 
输出：[0,1] 

提示： 
2 &lt;= nums.length &lt;= 104 
-109 &lt;= nums[i] &lt;= 109 
-109 &lt;= target &lt;= 109 
只会存在一个有效答案 
进阶：你可以想出一个时间复杂度小于 O(n2) 的算法吗？

```
**Answer**
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
**Note**
```
NULL
```

## Medium

## Difficult


## MoreInfo
For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Septerxy/LeetCode.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
