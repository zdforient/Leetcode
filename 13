class Solution:
    def romanToInt(self, s: 'str') -> 'int':
        l1 = ['I','V','X','L','C','D','M']
        l2 = [1,5,10,50,100,500,1000]
        m={}
        for i in range(7):
            m[l1[i]] = l2[i]
        t = sum([m[i] for i in s])
        for i in range(len(s)-1):
            if m[s[i]] < m[s[i+1]]:
                t -= m[s[i]] * 2
        return t
