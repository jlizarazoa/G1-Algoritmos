# G1-Algoritmos
Integrantes:
  -Juan Eduardo Bedoya
  -Luis Alfonso Diaz 
  -Juliette Lizarazo
  -Valentina Colmenares
  -Juan Pablo Caicedo


Laboratorio #4: El presente laboratorio busca desarrollar dos funciones que hallen las raíces de una función dada en clase, por dos métodos distintos: el de fuerza bruta (probar valor por valor hasta encontrar la raíz) y el método de la bisección, y se compara la complejidad de ambos algoritmos, es decir su tiempo de ejecución. Al lado de cada línea de código se coloca un comentario en el que se especifica el orden de complejidad de dicha línea.

Fuerza bruta:

    import numpy as np #O(1)
    
    def f(x): #O(1) + O(1) + O(1) -->  O(1)
        y=(x**5)-(59*(x**4))+(35*(x**3))-(250*(x**2))+(x)-70  #O(1)
        return y  #O(1)

    for i in np.arange(-1000,1000-0.0001,0.0001).round(4): #O(n)   
        if((f(i)*f(i+0.0001))<0 or f(i)==0): #O(1)   
            print(i) #O(1)    


Algoritmo voraz por bisección:

    def f(x): #O(1)
        y=(x**5)-(59*(x**4))+(35*(x**3))-(250*(x**2))+(x)-70 #O(1)
        return y #O(1)


     def biseccion(inicio,fin): # O(Log n)

         limInferior = inicio #O(1)
         limSuperior = fin #O(1)

         while (abs(limInferior-limSuperior) > (0.0001)): #O(Log n)
             limInferior=limSuperior  #O(1)
             limSuperior=(inicio+fin)/2  #O(1) #Produce el log n (base 2) en el while

            if (f(inicio)*f(limSuperior)<0): #O(1)
                 fin=limSuperior #O(1)

            if (f(limSuperior)*f(fin)<0): #O(1)
                 inicio=limSuperior #O(1)

         limSuperior=round(limSuperior,4) #O(1)
         print(limSuperior) #O(1)

     biseccion(-1000,1000) #O(Log n)
