class Solution:
    def isPalindrome(self, x):
        if x < 0:
            return False
        if 0 <= x < 10:
            return True
        original = x
        reversed_num = 0
        while x > 0:
            reversed_num = reversed_num * 10 + x % 10
            x = x // 10
        return original == reversed_num

        
