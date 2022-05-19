## Check a integer whether it is a prime number
```python
def is_prime(x):
    if (x==0) or (x==1):
        return False
    i=2
    while i*i<=x: 
        if x%i==0:
            return False
        i+=1
    return True
```
## Create a prime list
```python
def is_prime(x):
    if (x==0) or (x==1):
        return False
    i=2
    while i*i<=x:
        if x%i==0:
            return False
        i+=1
    return True

n=int(input("N= "))

prime_n=[x for x in range(n) if is_prime(x) ]
print(prime_n)
print('Number of prime between 1 to',n,':',len(prime_n),'\n')

n_prime=[]
current=0
j=1
while current<n:
    if is_prime(j):
        n_prime.append(j)
        current+=1            
    j+=1
print("First",n,"prime number:",n_prime)
```
