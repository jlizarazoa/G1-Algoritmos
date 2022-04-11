# G1-Algoritmos
Integrantes:
  -Juan Eduardo Bedoya
  -Luis Alfonso Diaz 
  -Juliette Lizarazo
  -Valentina Colmenares
  -Juan Pablo Caicedo
 
 Laboratorio #3:
 El correspondiente laboratorio consistió en la construcción grupal de un algoritmo de búsqueda de una secuencia de caracteres en una cadena usando el tipo de algoritmo 'Fuerza bruta'.

Complejidad y aclaraciones del Código:



      def genFinder(secuence,gen): # O(n) * [O(n) + O(n)] --> O(n) * O(n) --> O(n^2)
  
         for i in range(len(secuence)-len(gen)): #O(n)
         
         temp = secuence[i:i+len(gen)] #O(n)
      
         if(temp == gen):  #O(n)
          
                print(str(i)+" - "+str(i+len(gen))) #O(1)
              
                #break  #O(1)
              
                    """
                    Si se quita el break de comentarios, se devuelven todas las coincidencias en el texto
                    Si se deja el break de comentarios, se devuelve solo la primera coincidencia en el texto 
                   """

      gen = 'TAATAGCTTCTTAGGAGAATGACAAAA' # Grupo 1  #O(1)

      genFinder(secuence,gen)  #O(n^2)
  
