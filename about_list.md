# About Python List

```
In [1]: a = ['a', 'b', 'c']

In [2]: a.append('d')

In [3]: # добавление

In [4]: a
Out[4]: ['a', 'b', 'c', 'd']

In [5]: a.clear()

In [6]: a
Out[6]: []

In [7]: # очищаем список

In [8]: a = ['a', 'b', 'c']

In [9]: b = a

In [10]: b
Out[10]: ['a', 'b', 'c']

In [11]: a.append('d')

In [12]: a
Out[12]: ['a', 'b', 'c', 'd']

In [13]: b
Out[13]: ['a', 'b', 'c', 'd']

In [14]: c = a.copy()

In [15]: a.append('e')

In [16]: c
Out[16]: ['a', 'b', 'c', 'd']

In [17]: a
Out[17]: ['a', 'b', 'c', 'd', 'e']

In [18]: # copy

In [19]: a.append('e')

In [20]: a
Out[20]: ['a', 'b', 'c', 'd', 'e', 'e']

In [21]: a.count('e')
Out[21]: 2

In [22]: # count - количество определенных элементов

In [23]: a
Out[23]: ['a', 'b', 'c', 'd', 'e', 'e']

In [24]: d = ['f', 'g']

In [25]: a.extend(d)

In [26]: a
Out[26]: ['a', 'b', 'c', 'd', 'e', 'e', 'f', 'g']

In [27]: a += d

In [28]: a
Out[28]: ['a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g']

In [29]: # extend тоже, что += - расширяем список

In [30]: a.index('c')
Out[30]: 2

In [31]: # находим индекс нужного элемента

In [32]: a.index('f')
Out[32]: 6

In [33]: # если несколько одинаковых, то слева направо первый элемент

In [34]: a.index('h')
---------------------------------------------------------------------------
ValueError                                Traceback (most recent call last)
<ipython-input-34-cf73d789a52c> in <module>()
----> 1 a.index('h')

ValueError: 'h' is not in list

In [35]: a
Out[35]: ['a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g']

In [36]: a.insert(10, 'h')

In [37]: a
Out[37]: ['a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g', 'h']

In [38]: a.insert(0, '-a')

In [39]: a
Out[39]: ['-a', 'a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g', 'h']

In [40]: # вставка в нужное место

In [41]: a
Out[41]: ['-a', 'a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g', 'h']

In [42]: a.pop()
Out[42]: 'h'

In [43]: a
Out[43]: ['-a', 'a', 'b', 'c', 'd', 'e', 'e', 'f', 'g', 'f', 'g']

In [44]: a.remove('e')

In [45]: a
Out[45]: ['-a', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'f', 'g']

In [46]: del a[0]

In [47]: a
Out[47]: ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'f', 'g']

In [48]: a.reverse()

In [49]: a
Out[49]: ['g', 'f', 'g', 'f', 'e', 'd', 'c', 'b', 'a']

In [50]: a.sort()

In [51]: a
Out[51]: ['a', 'b', 'c', 'd', 'e', 'f', 'f', 'g', 'g']
```