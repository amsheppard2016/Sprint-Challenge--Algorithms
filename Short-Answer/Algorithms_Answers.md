#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

```python
a)  a = 0 #O(1)
    while (a < n * n * n): #O(n)
      a = a + n * n #O(n)
```
The runtime complexity is O(n). Since each line above would equal O(1+2n). Once you remove the constants O(n) is what you are left  with.


```
b)  sum = 0 #O(1)
    for i in range(n): #O(n)
      j = 1 #O(1)
      while j < n: #O(n^2)
        j *= 2 O(n*2)
        sum += 1 #O(1)
```
The runtime complexity is O(n). Each line equals O(1+n+1+n+2n+1). After you remove constans ends up being O(n^2)

```
c)  def bunnyEars(bunnies):
      if bunnies == 0: #O(n)
        return 0 #O(1)

      return 2 + bunnyEars(bunnies-1) #O(n)
```
This runtime complexity is O(n). All together they  equal O(1 + 2n), which comes out to O(n). The function being recursive causes it to be O (n).

## Exercise II

I would start with a recursive binary search. The floors of the building are like an array so I would start by testing the middle floor. If the egg breaks then run the same search on the lower array. Else run the same search on the upper array. Until you are left with a floor that the egg doesnt break and the following floor breaks. Then the function would return that number. The runtime complexity is O(log n), because the number of floors you start with this will change the amount of searches needed to complete the function.