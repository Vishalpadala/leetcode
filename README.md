# leetcode
class Solution:     def countPrimes(self, n):         count=0         isPrime=[True for _ in range(n)]         for i in range(2,n):             if isPrime[i]:                 count+=1                 j=2                 while(i*j &lt; n):                     isPrime[i*j]=False                     j+=1         return count
