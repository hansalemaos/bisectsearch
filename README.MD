# Functions for performing binary search on sorted lists

## pip install bisectsearch

#### Tested against Windows 10 / Python 3.10 / Anaconda 

	
```python
from bisectsearch import (
rightmost_value_equal_to,
leftmost_value_equal_to,
rightmost_value_less_than,
rightmost_value_less_than_or_equal,
leftmost_value_greater_than,
leftmost_value_greater_than_or_equal,
)
l = sorted(list(range(0, 5)) * 3)

print(f'{(h:=rightmost_value_equal_to(l, 4)), l[h]=}')
print(f'{(h:=rightmost_value_equal_to(l, 0)),l[h]=}')
print(f'{(h:=rightmost_value_equal_to(l, 1)),l[h]=}')
print(f'{(h:=leftmost_value_equal_to(l, 4)),l[h]=}')
print(f'{(h:=leftmost_value_equal_to(l, 0)),l[h]=}')
print(f'{(h:=leftmost_value_equal_to(l, 1)),l[h]=}')
print(f'{(h:=rightmost_value_less_than(l, 4)),l[h]=}')
print(f'{(h:=rightmost_value_less_than(l, 2)),l[h]=}')
print(f'{(h:=rightmost_value_less_than(l, 1)),l[h]=}')
print(f'{(h:=rightmost_value_less_than_or_equal(l, 40)),l[h]=}')
print(f'{(h:=rightmost_value_less_than_or_equal(l, 0)),l[h]=}')
print(f'{(h:=rightmost_value_less_than_or_equal(l, 1)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than(l, 2)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than(l, 3)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than(l, 0)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than(l, 1)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than_or_equal(l, 3)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than_or_equal(l, 0)),l[h]=}')
print(f'{(h:=leftmost_value_greater_than_or_equal(l, 1)),l[h]=}')

# output

# (h:=rightmost_value_equal_to(l, 4)), l[h]=(14, 4)
# (h:=rightmost_value_equal_to(l, 0)),l[h]=(2, 0)
# (h:=rightmost_value_equal_to(l, 1)),l[h]=(5, 1)
# (h:=leftmost_value_equal_to(l, 4)),l[h]=(12, 4)
# (h:=leftmost_value_equal_to(l, 0)),l[h]=(0, 0)
# (h:=leftmost_value_equal_to(l, 1)),l[h]=(3, 1)
# (h:=rightmost_value_less_than(l, 4)),l[h]=(11, 3)
# (h:=rightmost_value_less_than(l, 2)),l[h]=(5, 1)
# (h:=rightmost_value_less_than(l, 1)),l[h]=(2, 0)
# (h:=rightmost_value_less_than_or_equal(l, 40)),l[h]=(14, 4)
# (h:=rightmost_value_less_than_or_equal(l, 0)),l[h]=(2, 0)
# (h:=rightmost_value_less_than_or_equal(l, 1)),l[h]=(5, 1)
# (h:=leftmost_value_greater_than(l, 2)),l[h]=(9, 3)
# (h:=leftmost_value_greater_than(l, 3)),l[h]=(12, 4)
# (h:=leftmost_value_greater_than(l, 0)),l[h]=(3, 1)
# (h:=leftmost_value_greater_than(l, 1)),l[h]=(6, 2)
# (h:=leftmost_value_greater_than_or_equal(l, 3)),l[h]=(9, 3)
# (h:=leftmost_value_greater_than_or_equal(l, 0)),l[h]=(0, 0)
# (h:=leftmost_value_greater_than_or_equal(l, 1)),l[h]=(3, 1)
```