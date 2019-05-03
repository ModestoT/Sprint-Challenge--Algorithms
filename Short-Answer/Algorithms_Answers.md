Add your answers to the Algorithms exercises here.

## Exercise 1

a)  a = 0                     O(1)
    while (a < n * n * n):    O(n)
      a = a + n * n           O(1)
  
  answer O(n)

b)  sum = 0    O(1)
    for i in range(n):   O(n)
      i += 1          O(1)
      for j in range(i + 1, n): O(n)
        j += 1    O(1) 
        for k in range(j + 1, n): O(n)
          k += 1 O(1)
          for l in range(k + 1, 10 + k): O(n)
            l += 1
            sum += 1

    answer O(n^4)

c)  def bunnyEars(bunnies):
      if bunnies == 0: O(1)
        return 0

      return 2 + bunnyEars(bunnies-1) O(n)

    answer O(n)

## Exercise 2


def CheckBreakingPoint(nStories, eggs):
  for story in nStories:     
    drop egg from story starting from first story
    check if egg breaks or not
    if it does break return that story
    else
    go to the next story 
    then check if an egg breaks at this story

time complexity of this possible solution would be an O(n) since it is dependent on however many stories the build has