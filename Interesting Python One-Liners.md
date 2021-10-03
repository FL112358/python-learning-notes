## Most frequent element
~~~
test_list = [3, 2, 5, 6, 4, 3, 2, 5, 3, 7, 4]
most_frequent_element = max(set(test_list), key=test_list.count)
print(most_frequent_element)
~~~
> 3

## Merge sets
~~~
s1 = {1, 3, 5}
s2 = {2, 4, 6}
s1.update(s2)
print(s1)
~~~
> {1, 2, 3, 4, 5, 6}

## Anagram
~~~
from collections import Counter
s1 = 'silent'
s2 = 'listen'
print('anagram') if Counter(s1) == Counter(s2) else print('not an anagtam')
~~~
> anagram
