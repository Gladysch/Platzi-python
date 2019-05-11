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

stackoverflow => Paginas 

clase 5
--=======================================
-- trialapp.urls
from django.conf.urls import url
from apps.trialapp.views import root, hello, hello_name, hello_age

urlpatterns = [
    url(r'^$', root),
    url(r'^hello/$', hello),
    url(r'^hello/([a-z]{3,8})/$', hello_name),
    url(r'^hello/[a-z]{3,8}/([0-9]|[1-9]{1}[0-9]{1})/$', hello_age),
]
--=======================================
-- trialapp.views
from django.http import HttpResponse


def root(request):
    # assert False  # Sirve para romper el flujo
    return HttpResponse('Area 51 Training Center, desde Trial')


def hello(request):
    return HttpResponse('Hola estamos en Trial!')


def hello_name(request, name):
    message = '''
        Hola {}, estas en TrialApp
    '''.format(name)
    return HttpResponse(message)


def hello_age(request, age):
    message = '''
        Hola, tu edad es {}. <br\>
    '''.format(age)
    if int(age) > 17:
        message += 'Eres mayor de edad'
    else:
        message += 'Eres menor de edad'
    return HttpResponse(message)

-- TAREA
CREATE PARA COMPANY
