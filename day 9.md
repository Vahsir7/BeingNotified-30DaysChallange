Prime Reversal
You are given two binary strings 
A and B, each of length N. You can perform the following operation on string A any number of times:
Select a prime number X. Choose any substring of string A having length X and reverse the substring.
Determine whether you can make the string A equal to B using any (possibly zero) number of operations.
A substring is obtained by deleting some (possibly zero) elements from the beginning and some (possibly zero) elements from the end of the string.

------------------------------

testcase = int(input())
for i in range(testcase):
    l = int(input())
    s1=input()
    s2=input()
    o1=o2=0
    for i in range(l):
        if s1[i] == '1':
            o1+=1
        if s2[i] == '1':
            o2+=1
    #print(o1,o2)
    if (o1==o2):
        print("YES")
    else:
        print("NO")