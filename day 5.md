<h1>Mask Policy</h1>
<a href="https://www.codechef.com/practice/course/1-star-difficulty-problems/DIFF1200/problems/MASKPOL">Question link</a>

<div>
A city has been infected by a contagious virus.
  
In a survey, it was found that A out of the N people living in the city are currently infected. It has been observed that the only way for a person to get infected is if he comes in contact with an already infected person, and both of them are NOT wearing a mask.

The mayor of the city wants to make a new Mask Policy and find out the minimum number of people that will be required to wear a mask to avoid the further spread of the virus. Help the mayor in finding this number.
Note: The only aim of the mayor is to stop virus spread, not to mask every infected person.
</div>

<hr>

```
testcase = int(input())
for i in range(testcase):
    n,a = map(int,input().split())
    b=n-a
    print(min(a,b))
```
