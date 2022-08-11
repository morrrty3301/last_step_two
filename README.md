
# last_step_two

from itertools import *
k = 0
a = []
for x in product('УКЫСМ', repeat=5):
    s = ''.join(x)
    k += 1
    if s.count('Ы') <= 1 and s.count('У') == 2 and s.count('С') == 0:
        a.append(k)

s = []        
for i in range(len(a)):
    s.append(a[i]+1)

print(s)
