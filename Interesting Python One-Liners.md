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

## Binary to decimal
~~~
d = int('1010', 2)
print(d)
~~~
> 10

## Quick sort
~~~
qsort = lambda lis: lis if len(lis) <= 1 else qsort([x for x in lis[1:] if x < lis[0]]) + [lis[0]] + qsort([x for x in lis[1:] if x >= lis[0]])
print(qsort([17, 29, 11, 97, 103, 5]))
~~~
> [5, 11, 17, 29, 97, 103]

## Sum of n consecutive numbers
~~~
n = 5
print(sum(range(1, n+1)))
~~~
> 15

## Ceiling division
~~~
a, b = 11, 4
print(-(-a // b))
~~~
> 3

## Use "for" in list comprehensions
~~~
print([number for number in [1, 2, 3, 4] if number % 2 == 0])
~~~
> [2, 4]

~~~
# numbers of elements that smaller than x in a m*n Multiplication Table
m = 4
n = 3
x = 5
print(sum(min(x // i, n) for i in range(1, m+1)))
~~~
> 7

