![map](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg/473px-Hash_table_3_1_1_0_1_0_0_SP.svg.png)

Load factor
A load factor is a critical statistic of a hash table, and is defined as follows:


where alpha = n/k

n is the number of entries occupied in the hash table.

k is the number of buckets.(size)

The performance of the hash table deteriorates in relation to the load factor alpha.

Therefore a hash table is resized or rehashed if the load factor approaches 1.

A table is also resized if the load factor drops below alpha_max/4

Acceptable figures of load factor include 0.6 and 0.75.


Hash function

h(k) = M mod n


Collision resolution

**Separate chaining**

![chaining](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Hash_table_5_0_1_1_1_1_1_LL.svg/675px-Hash_table_5_0_1_1_1_1_1_LL.svg.png)



**Open addressing**

![addressing](https://upload.wikimedia.org/wikipedia/commons/thumb/b/bf/Hash_table_5_0_1_1_1_1_0_SP.svg/570px-Hash_table_5_0_1_1_1_1_0_SP.svg.png)

Open addressing is another collision resolution technique in which every entry records are stored in the bucket array itself, and the hash resolution is performed through probing.


Well-known probe sequences include:

Linear probing, in which the interval between probes is fixed (1,2,3,4) (2,4,6,8)

Quadratic probing, in which the interval between probes is increased by adding the successive outputs of a quadratic polynomial to the value given by the original hash computation.
(1,2,4,8,16)

Double hashing, in which the interval between probes is computed by a *secondary hash function*.


https://en.wikipedia.org/wiki/Hash_table

https://www.geeksforgeeks.org/hashing-data-structure/?ref=lbp


1. Two Sum

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.
```
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        hashmap = {}
        for i in range(len(nums)):
            complement = target - nums[i]
            if complement in hashmap:
                return [i, hashmap[complement]]
            hashmap[nums[i]] = i
```
https://leetcode.com/problems/two-sum/solution/
