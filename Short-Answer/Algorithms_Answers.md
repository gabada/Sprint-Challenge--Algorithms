Add your answers to the Algorithms exercises here.

## Exercise I

```
a)  a = 0 # O(1)
    while (a < n * n * n): O(n)
      a = a + n * n O(1)
```
The Big O is O(n) because as N is increased it takes more time to complete. (Added big O analysis to code above)

```
b)  sum = 0 # O(1)
    for i in range(n): # O(n)
      i += 1 # O(1)
      for j in range(i + 1, n): # O(n)
        j += 1 # O(1)
        for k in range(j + 1, n): # O(n)
          k += 1 # O(1)
          for l in range(k + 1, 10 + k): # O(1)
            l += 1 # O(1)
            sum += 1 # O(1)
```
The Big O is O(n^3). This is because there are 3 loops that actually depend on the value of N. The fourth loop is a constant. To get O(n^3) I multiplied all of the loops `(O(n) * O(n) * O(n) * O(1))` (Added Big O analysis to code above)

```
c)  def bunnyEars(bunnies): O(1)
      if bunnies == 0: # O(1)
        return 0 # O(1)

      return 2 + bunnyEars(bunnies-1) O(n)
```
The Big O is O(n). This problem is trickier because it's recursion. In this case you can think of bunnies as N. It is O(n) because as the value on N increases it will take more time to complete.



## Exercise II

I would start out by going to the half way point of the floors (`f/2`). I would then drop an egg. If they egg breaks then I know that the egg will break on every floor above `f/2`. I would drop the next egg at the half way point of the lower floors (`(f/2)/2`). If the egg broke at that height I now know that the egg will break after being dropped from anything above that floor. Next I would go to half of that floor so (`((f/2)/2)/2`) If the egg still broke I would continue halving the floors until I got an egg that didn't break. I would then go up half as may floors. If it doesn't break I would go up half again but if it does break I would go down half again. Until the egg doesn't break.

The Big O of this method (Binary search) would is O(log n) because its dividing in half

