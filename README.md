# Gererando bucles

## Punto #1

Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.

## Solución punto #1

``` python
a = 1 #Se asigna el primer valor
while(a <= 100): #Definimos el bucle
  print(str(a)+ " y su cuadrado es: " +str(a**2)) #Se imprime el valor actual y su cuadrado
  a += 1 #Se actualiza el valor para que el bucle se repita hasta que deje de cumplir la condición
```
### Código probado

[![Captura-de-pantalla-2023-03-27-193408.png](https://i.postimg.cc/br4Ff9bW/Captura-de-pantalla-2023-03-27-193408.png)](https://postimg.cc/V0BFjMKW)

### Diagrama de flujo
[![pako-e-Np-NUEt-Pwz-AM-it-WTt1op5-Vj-JYp-YO1-CRg-MO4-LTt-YSb-ZZ5-DFlq-RC0-e-k-LUL45-O-h-T7-Y7-Jpx-Ur-GBH7-T7-FGX2-A95pbi-PWwbyw.png](https://i.postimg.cc/5ykWYzzS/pako-e-Np-NUEt-Pwz-AM-it-WTt1op5-Vj-JYp-YO1-CRg-MO4-LTt-YSb-ZZ5-DFlq-RC0-e-k-LUL45-O-h-T7-Y7-Jpx-Ur-GBH7-T7-FGX2-A95pbi-PWwbyw.png)](https://postimg.cc/CnDQ9zmR)

## Punto #2

Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.

## Solución punto #2

``` python
i = 1 #asignamos la variable con valor de 1 (números impares)
print("a continuación tenemos los numeros impares de 1 hasta 999") #imprimimos el enunciado
while (i <= 999):#abrimos un bucle en el que 'i' debe ser menor o igual a 999
    if (i%2 > 0):#si el residuo de 'i'/2 es mayor a 0, 'i' es impar
        print(i)#imprimimos 'i'
    i = i + 2 #sumamos 2 a 'i' para continuar el bucle hasta que deje de cumplir la condición

a = 2 #asignamos la variable con valor de 2 (números impares)
print("a continuación tenemos los numeros pares de 2 hasta 1000")#imprimimos el enunciado
while (a <= 1000): #abrimos un bucle en el que 'n' debe ser menor o igual a 1000
    if (a%2 < 1): #si el residuo de 'n'/2 es menor a 1, 'n' es par
        print(a) #imprimimos 'n'
    a = a + 2 #sumamos 2 a 'n' para continuar con el bucle hasta que deje de cumplir la condición
```
### Código probado

[![h.png](https://i.postimg.cc/vTt8VZyZ/h.png)](https://postimg.cc/V05cy15x)

### Diagrama de flujo



## Punto #3

Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado

## Solución punto #3

``` python
x = int(input("Ingrese un número mayor a 2")) #Le solicitamos al usuario que ingrese un número
if x % 2 != 0: #Si el número no es par se le resta 1, para que se vuelva par
    x -= 1 
if x < 2 : #Se coloca una condición en caso de que el número no sea mayor a 2
    print ("El número ingresado no es válido")
while x >= 2: #Definimos el bucle donde se imprimirán los números hasta llegar a 2
    print(x)
    x -= 2 #Al restarle 2 a un número par, el resultado seguirá siendo par 
```
### Código probado

[![Captura-de-pantalla-2023-03-27-204346.png](https://i.postimg.cc/WpHXBwcS/Captura-de-pantalla-2023-03-27-204346.png)](https://postimg.cc/7bS3776T)

## Punto #4

En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18:9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para informar en que año la población del país B superará a la de A.


En este caso coloqué 2 posibles soluciones: 

1. La primera nos indica la lista de años hasta el momento en el que la población del país B supera a la del A
2. Y la segundo nos imprime el año exacto en el que la población del país B supera la del A

## Solución punto #4

#### Solución #1

Indica la lista de años hasta el momento en el que la población del país B supera a la del A

``` python
habitantesA = 25000000 #definimos la cantidad de habitantes del pais A
habitantesB = 18900000 #definimos la cantidad de habitantes del pais B
año = 2022#asignamos el año (2022)

while (habitantesB <=habitantesA):#iniciamos un bucle si los habitantes de B son menores a los habitantes de A
    crecimientoA = ((habitantesA*2)/100) #creamos la fórmula para saber el crecimiento de los habitantes de A
    crecimientoB = ((habitantesB*3)/100) #creamos la fórmula para saber el crecimiento de los habitantes de B
    habitantesA = habitantesA + crecimientoA #sumamos el crecimiento al valor inicial de los habitantes de A
    habitantesB = habitantesB + crecimientoB #sumamos el crecimiento al valor inicial de los habitantes de B
    año = año + 1 #sumamos un año al valor inicial
    print(año) #imprimimos los años en los que la población de A será mayor a la de B
```
### Código probado

[![Captura-de-pantalla-2023-03-27-204443.png](https://i.postimg.cc/W1CDjtbB/Captura-de-pantalla-2023-03-27-204443.png)](https://postimg.cc/QFgNJ87m)

#### Solución #2

Imprime el año exacto en el que la población del país B supera la del A

``` python
#definimos la variable
habitantesA= 25000000
habitantesB= 18900000
crecimientoA= 0.02
crecimientoB= 0.03
año =2022

while habitantesB < habitantesB :
    año += 1 #incrementar el año
    #calcular el nuevo tamaño de la población
    habitantesA += habitantesA*crecimientoA
    habitantesB += habitantesB*crecimientoB
    #Imprimir el resultado de la población
print("La población del país B supera a la población del país A en el año", año)

```
### Código probado

[![Captura-de-pantalla-2023-03-27-204527.png](https://i.postimg.cc/XJ0pGh5x/Captura-de-pantalla-2023-03-27-204527.png)](https://postimg.cc/WDX2x5XJ)

## Punto #5

Imprimir el factorial de un número natural n dado.

## Solución punto #5

``` python
a = float(input("Ingrese un número entero:")) #Se ingresa el número al que se le quiere sacar el factorial
x = a #El valor "x", será el que multiplicará a la variable "a", y comenzará teniendo el mismo valor que "a"

while x > 1: # El bucle va hasta que "x" llega 1, ya que si llega a 0, todo el bucle daria cero
    print(a) #Se imprimen todos los resultados hasta llegar, al factorial del número
    x -= 1 #Se resta 1 a la variable "x"
    a *= x # Se multiplica "a" por "x" ejm: Factorial de 3 = (3*3)*(3*2)*(3*1), siendo los números 3,2,1 la variable x, donde cada vez disminuye una unidad
    
print ("El factorial del número ingresado es: " +str(a) ) #Se imprime el último valor de a, que seria el valor factorial
```

### Código probado

[![Captura-de-pantalla-2023-03-27-204638.png](https://i.postimg.cc/ZKDnF03W/Captura-de-pantalla-2023-03-27-204638.png)](https://postimg.cc/qzyppJ1r)

## Punto #6

Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.

## Solución punto #6

``` python
x = input("Piensa un número del 1 al 100, y cuando estés listo presiona enter para comenzar: ") #Al presionar la tecla enter comienza el juego
a = 50 #Se inicia la variable en la mitad del rango,que en este caso es 50
print("Acaso el número es:" + str(a) + "?") #El código comienza preguntando si el numero que piensas es el 50, a partir de eso:

pregunta = input("El número que estás pensando es igual, poco menor , menor, mucho menor, poco mayor, mayor o mucho mayor al que dije?: ")

while pregunta != str("igual"): #Si se elige que es igual, el código se acaba e imprime que se adivinó el numero
    if pregunta == "poco menor": #Se resta 1 al valor actual, y se vuelve a preguntar
        a -= 1
    elif pregunta == "poco mayor": #Se suma 1 al valor actual, y se vuelve a preguntar
        a += 1
    elif pregunta == "menor": #Se resta 5 al valor actual, y se vuelve a preguntar
        a -= 5
    elif pregunta == "mayor": # Se resta 5 al valor actual, y se vuelve a preguntar
        a += 5
    elif pregunta == "mucho menor": #Se resta 10 al valor actual, y se vuelve a preguntar
        a -= 10
    elif pregunta == "mucho mayor": #Se suma 10 al valor actual, y se vuelve a preguntar
        a += 10
    
    print("Acaso el número es:" + str(a) + "?") #Por medio de este print se digita el nuevo número dependiendo de la respuesta del usuario
   
    #Por medio de este print se vuelve a preguntar
    pregunta = input("El número que estás pensando es igual, poco menor , menor, mucho menor, poco mayor, mayor o mucho mayor al que dije?: ") 

print("¡He adivinado el número!, el número es " +str (a)) #Fin del bucle cuando se digita que el numero es igual al pensado
```
### Código probado

[![Captura-de-pantalla-2023-03-27-204809.png](https://i.postimg.cc/bY4Ns4jn/Captura-de-pantalla-2023-03-27-204809.png)](https://postimg.cc/grqP7Sjc)

## Punto #7

Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.

## Solución punto #7

``` python
valor= int(input("Ingrese un número desde el 2 al 50:")) #Se le solicita al usuario que ingrese el valor inicial

if valor < 2 or valor > 50: #Colocamos un condicional que le permite identificar al programa si el número está en el rango
    print("El número no es válido ")
else:
   print("Los divisores de", valor, "son: ")

   divisor = 1 #se inicia con uno ya que el bloque while va a verficar todos los números desde ahí
   while divisor<= valor:#Se inicia el bucle siempre y cuando el divisor sean menor o igual al valor
       if valor% divisor == 0: #Si el residuo de la división es 0, entonces ese valor será un condicional
        print(divisor) #Se imprime el divisor

       divisor +=1 #Se le va sumando 1 hasta llegar al valor ingresado y así ir verificando sus divisores
```
### Código probado

[![Captura-de-pantalla-2023-03-27-205053.png](https://i.postimg.cc/nLQMRZZn/Captura-de-pantalla-2023-03-27-205053.png)](https://postimg.cc/R34MhkNY)

## Punto #8

Implementar el algoritmo que muestre los números primos del 1 al 100 usando funciones

## Solución punto #8

``` python
def numerosPrimos(a: int):
    i = int(2) # Se establece la variable desde 2 
    if a == 2 :
        print(a)
    while i < a : # mientras 'i' sea menor que 'a'
        if a%i ==0: # romper el bucle
            break
        elif i == a-1: # si 'i' es igual a 'a' - 1
            print(a)
        i += 1 #actualizar la variable sumando uno
 
if __name__ == "__main__":
    a = int(2) # declarar el límite mínimo de 'a'
    d = 100 #declarar el límite máximo 'd'
    while a < d : #mientras 'a' sea menor que 'd'
      Primos = numerosPrimos(a) #Declarar una variable d que expresa a los numero primos 'a' que estan entre el rango de 2 a 100
      a += 1 #Actualizar la variable de uno en uno teniendo en cuenta el rango
```
### Código probado

[![Captura-de-pantalla-2023-03-27-205922.png](https://i.postimg.cc/W4MqpjyX/Captura-de-pantalla-2023-03-27-205922.png)](https://postimg.cc/XZYYQM4C)
