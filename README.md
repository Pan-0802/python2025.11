#求素数
n=eval(input())
l = []
for i in range(2,n+1):
    l.append(i)
print(l)
for i in l.copy():
    for j in range(i+1,n+1,) :
        if j % i == 0 and j in l :
            l.remove(j)
print(l)
