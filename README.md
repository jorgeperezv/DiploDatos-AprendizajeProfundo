## DiploDatos-AprendizajeProfundo
Materia optativa "Aprendizaje Profundo" (Deep Learning) de la Diplomatura en Ciencias de Datos de la UNC

## Integrantes

* Ará Berberian
* Jorge Pérez
* Enzo Valverdi

# Informe

En primera instancia, comenzamos realizando pruebas con dos tipos de redes neuronales distintas, MLP y CNN en notebooks para poder entender en mayor detalle su funcionamiento. Luego de realizar dichas pruebas, desarrollamos un script llamado classifier_neural_network.py para poder correr ambos modelos de forma parametrizable incluyendo los hiperparametros.

## Resultados experimentos modelo MLP

Se probaron alterar los siguientes parametros:

* Dropuot: 0.3 y 0.7
* Batch Size: 128 y 256
* Freeze Embedings: True y False

<img src="images/MLflow MLP.png"
     alt="Experimentos MLP"
     style="float: center; margin-right: 10px;"
/>

Al poner en *False* el freeze embedings, obtenemos muchos mejores resultados que utilizando los mismos parámetros y seteandolo en *True*. Esto nos generó la duda, de que al realizar esta modificación estemos ante un caso de overfitting.

Con respecto al parametro dropout, verificamos que se obtienen mejores resultados cuando el valor es mas pequeño (0.3).

Por último, con un batch size de 256, obtenemos mejores resultados que uno de 128. Llegando a la conclusión, de que con batch size en 256 y dropout en 0.3, obtenemos el mejor resultado dejando del lado el parametro freeze embeding.

## Resultados experimentos modelo CNN

<img src="images/CNN-MLflow.png"
     alt="Experimentos CNN"
     style="float: center; margin-right: 10px;"
/>
