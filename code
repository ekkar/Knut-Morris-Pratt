t = raw_input('Enter the string ')
s = raw_input('Enter the substring ')
import OurPrefix
    
def kmp(s,t):
    index = -1
    f = OurPrefix.prefix(s)
    k = 0
    for i in xrange(len(t)):
        while k > 0 and s[k] <> t[i]:
            k = f[k-1]
        if s[k] == t[i]:
            k = k + 1
        if k == len(s):
            index = i - len(s) + 1
            break
    return index
    
print(kmp(s,t))    
if kmp(s,t) == -1:
print('Substring not found')
else:
print'Substring in the string starts with a number {0} '.format(kmp(s,t))
