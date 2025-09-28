# Leetcode-2798.-Number-of-Employees-Who-Met-the-Target
# Description
There are n employees in a company, numbered from 0 to n - 1. Each employee i has worked for hours[i] hours in the company.

The company requires each employee to work for at least target hours.

You are given a 0-indexed array of non-negative integers hours of length n and a non-negative integer target.

Return the integer denoting the number of employees who worked at least target hours.
# Algorithm
1. Create a variable count to keep track of emploees who have worked for atleast target number of hours.
2. Loop through hours
3. And for each ith element check if i>=target
4. If it is then increment count by 1 .
# Code
class Solution:

    def numberOfEmployeesWhoMetTarget(self, hours: List[int], target: int) -> int:
        count=0
        for h in hours:
            if h>=target:
                count+=1
        return count
