# 二分搜索笔记

时间复杂度一般为O(logn),一般适用于有序数组

二分搜索一般有二种目的：

- 判断一个特定的值是否在数组中存在
- 在数组中寻找满足条件的值

一般二分搜索的模板(用于判断target在数组中是否存在)

```java
class Solution{
  pubilc int binarySearch(int[] nums, int target){
    int l = 0, r = nums.length - 1;
    while(l <= r){
      int mid = l + (r-l) / 2;
      if(nums[mid] == target){
        return true;
      }
      if(nums[mid] < target){
        l = mid + 1;
      }
      else{
        r = mid - 1;
      }
      return false;
    }  
  }
}

```

## 二分搜索题目笔记

> Leetcode 153. Find Minimum in Rotated Sorted Array.

> Suppose an array of length n sorted in ascending order is rotated between 1 and n times. For example, the array nums = [0,1,2,4,5,6,7] might become: 
> - [4,5,6,7,0,1,2] if it was rotated 4 times.
> - [0,1,2,4,5,6,7] if it was rotated 7 times. 

> Notice that rotating an array [a[0], a[1], a[2], ..., a[n-1]] 1 time results in the array [a[n-1], a[0], a[1], a[2], ..., a[n-2]]. 

> Given the sorted rotated array nums of unique elements, return the minimum element of this array. 

> You must write an algorithm that runs in O(log n) time.
