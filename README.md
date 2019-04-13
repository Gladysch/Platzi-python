# Platzi-python
Clases de Python
Clase n°3

# FIBONACCI
def fibo(n):
    if n == 0 or n == 1:
        return n
    return fibo(n-1) + fibo(n-2)

def print_fibo(n):
    for i in range(n):
        print(fibo(i), end=', ')
        
n = int(input())
print_fibo(n)

#t3chfest2018

# fibonacci al cubo

codingBat
