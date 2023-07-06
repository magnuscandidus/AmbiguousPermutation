# AmbiguousPermutation
# cook your dish here
n=int(input())
while(n!=0):
    a=list(map(int,input().split()))
    b=a.copy()
    for i in range(n):
        b[a[i]-1]=i+1 
    if (a==b):
        print("ambiguous")
    else:
        print("not ambiguous")
    n=int(input())
