# G1-Algoritmos
Integrantes:
  -Juan Eduardo Bedoya
  -Luis Alfonso Diaz 
  -Juliette Lizarazo
  -Valentina Colmenares
  -Juan Pablo Caicedo
  
  Laboratorio #6: En el presente laboratorio se implementó de un perceptrón simple mostrado en clase para un clasificador binario utilizando el dataset "data_banknote_authentication.cvs" obtenido de: https://archive.ics.uci.edu/ml/datasets/banknote+authentication, utilizando los atributos "Skewness of Wavelet Transformed image" y "Kurtosis of Wavelet Transformed image".
  
  Análisis de resultados:
  De las dos características seleccionadas se pudo apreciar que los datos no son linealmente separables (como se puede apreciar en el siguiente gráfico), por lo que la capacidad del perceptrón para el discernimiento de las dos clases (Authentic/Inauthentic) es mucho menor.
  
  ![image](https://user-images.githubusercontent.com/95059566/173982110-7b7c9dc5-4ef9-4ece-be8d-138281ae3579.png)
  
  Es por esto, que al realizar el entrenamiento y evaluar los resultados del mismo, se calcula un 55.5393% de error, generando un comportamiento inestable, como se puede observar en la gráfica a continuación.
  
  ![image](https://user-images.githubusercontent.com/95059566/173982453-e49b3638-9a13-4627-b213-00afa4e05cf5.png)

  Finalmente, se puede concluir que es necesario el uso de algoritmos y estructuras más sofisticadas para una clasificación adecuada del dataset escogido.
