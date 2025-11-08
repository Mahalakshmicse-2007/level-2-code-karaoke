
<img width="5400" height="2383" alt="Code Karaoke-min" src="https://github.com/user-attachments/assets/b93e02e6-6468-4a00-9a9e-a00bc0e4cb0f" />



# level-2-code-karaoke
Level 2 questions for code karaoke event, there are 2 questions write the program and test it with examples in those questions and upload in fork 
# Question 1:
1.Tow Sum:
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.
 
# Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

# Example 2:
Input: nums = [3,2,4], target = 6
Output: [1,2]

# Example 3:
Input: nums = [3,3], target = 6
Output: [0,1]

# CODE:def two_sum(nums, target):
    seen = {}  

    for i, num in enumerate(nums):
        diff = target - num
        if diff in seen:
            return [seen[diff], i]  
        seen[num] = i
        print(two_sum([3,3],6))

    return []

# OUTPUT:![WhatsApp Image 2025-11-08 at 10 53 55_3dd2f906](https://github.com/user-attachments/assets/12d2feed-6d96-4b0e-9d8a-eed767ce5cc1)



# Question 2:
1. Palindrome Number:

Given an integer x, return true if x is a palindrome, and false otherwise.
 
# Example 1:
Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
# Example 2:
Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
# Example 3:
Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.


# CODE:
def is_palindrome(x):

    return str(x) == str(x)[::-1]


x = int(input("Enter an integer: "))

if is_palindrome(x):
    print("True — It's a palindrome!")
else:
    print("False — Not a palindrome.")
# OUTPUT:![WhatsApp Image 2025-11-08 at 11 12 19_a0e742e9](https://github.com/user-attachments/assets/72067f81-bf6c-43e4-898c-fcaf3105fc77)

