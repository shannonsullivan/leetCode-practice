## 350. Intersection of Two Arrays II

Given two integer arrays nums1 and nums2, return an array of their intersection. Each element in the result must appear as many times as it shows in both arrays and you may return the result in any order.

### Example 1:

Input: nums1 = [1,2,2,1], nums2 = [2,2]\
Output: [2,2]

### Example 2:

Input: nums1 = [4,9,5], nums2 = [9,4,9,8,4]\
Output: [4,9]\
Explanation: [9,4] is also accepted.


### Constraints:

- 1 <= nums1.length, nums2.length <= 1000
- 0 <= nums1[i], nums2[i] <= 1000

### Pseudocode:

1. Initialize length of 1st input array
2. Initialize length of 2nd input array
3. Initialize pointer 1, 2 and 3
4. Sort both input arrays
5. While fist pointer is less than length of 1st input array
6. And 2nd pointer is less than length of 2nd input array
7. If 1st input array index at 1st pointer is less than 2nd input array index at 2nd pointer
8. Increment 1st pointer
9. Else if 1st input array index at 1st pointer is greater than 2nd input array index at 2nd pointer
10. Increment 2nd pointer
11. Else set 3rd pointer incremented to index of 1st input array index of 1sst pointer incremented
12. Increment 2nd pointer
13. Return the range of 1st input array from index 0 to third pointer