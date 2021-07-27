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

## 二分搜索相关题目笔记

- [Leetcode 34. Find the first and last postion of Element in Sorted Array](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/34.%20Find%20First%20and%20Last%20Position%20of%20Element%20in%20Sorted%20Array.md)
- [Leetcode 162. Find Peak Element](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/162.%20Find%20Peak%20Element.md)
- [Leetcode 153. Find Minimum in Rotated Sorted Array](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/153.%20Find%20Minimum%20in%20Rotated%20Sorted%20Array.md)
- [Leetcode 275. H-Index II](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/275.%20H-Index%20II)
- [Leetcode 81. Search in Rotated Sorted Array II.md](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/81.%20Search%20in%20Rotated%20Sorted%20Array%20II.md)
- [Leetcode 33. Search in Rotated Sorted Array](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/33.%20Search%20in%20Rotated%20Sorted%20Array.md)
- [154. Find Minimum in Rotated Sorted Array II [H]](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/154.%20Find%20Minimum%20in%20Rotated%20Sorted%20Array%20II%20%5BH%5D.md)
- [540. Single Element in a Sorted Array](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/540.%20Single%20Element%20in%20a%20Sorted%20Array.md)
- [240. Search a 2D Matrix II](https://github.com/wruochao19/Leetcode-Note/blob/main/Binary_Search/540.%20Single%20Element%20in%20a%20Sorted%20Array.md)
