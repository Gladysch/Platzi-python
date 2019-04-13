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

#Celulares
string = '999999999 989898980 799999 99999999999 787890980'
list(filter(lambda x: len(x) == 9 and x[0] in ('9', '7'), string.split()))



# fibonacci al cubo

codingBat
