# Laboratorio Análisis Estadístico De La Señal
# Parte A
1. Base de Datos Physionet
2. Importación y Gráfica de la Señal
<img width="1216" height="159" alt="image" src="https://github.com/user-attachments/assets/6333b1b1-abac-44fa-8045-08e8edad4ffc" />

<img width="737" height="560" alt="image" src="https://github.com/user-attachments/assets/d88298a5-cd4c-43b9-bd20-e232a83ad403" />

2.1 Gráfica en Dominio del Tiempo

<img width="726" height="557" alt="image" src="https://github.com/user-attachments/assets/14e3fbff-16b1-420d-979a-5f7e71effee0" />

3. Cálculos Estadíst6icos Descriptivos
   
   a) Media deb la señal

<img width="849" height="328" alt="image" src="https://github.com/user-attachments/assets/e4dcc61c-e69a-490a-a208-1f4dee4a6271" />

--- RESULTADOS DEL CÁLCULO DE LA MEDIA ---
Suma total de todos los valores: 176.590000
Número total de muestras: 5000
Media de la señal: 0.035318

Luego se calculó nuevamente la media de la señal mediante el uso de librerias o funciones.

<img width="523" height="67" alt="image" src="https://github.com/user-attachments/assets/8ff4cc3f-7be0-4f4b-97ac-baac40d84ff2" />

media de la señal:0.035318

   b) Desviación Estandar

   <img width="682" height="453" alt="image" src="https://github.com/user-attachments/assets/93c075b3-6004-4706-b580-ac2c927d4801" />

Suma de diferencias al cuadrado: 110.156394
Varianza: 0.022031
Desviación estándar: 0.148429

Cálculo con librerias

<img width="550" height="69" alt="image" src="https://github.com/user-attachments/assets/7808999d-c404-45c3-9a46-6cc785ea2f1e" />

Desviación estandar:0.148429

   c) Coeficiente de variación

   <img width="1073" height="312" alt="image" src="https://github.com/user-attachments/assets/3bbb2f38-1911-4617-a55f-85b86290edea" />

    Coeficiente de variación: 4.202655
 Coeficiente de variación (%): 420.27%

Cálculo con librerias

<img width="591" height="182" alt="image" src="https://github.com/user-attachments/assets/53ffb273-c6c7-4b68-8236-ffc4f4706d28" />


Coeficiente de variación: 420.27%
 
   d) Histograma



   Cálculo con librerias.

<img width="497" height="142" alt="image" src="https://github.com/user-attachments/assets/a2b399de-d615-4ac7-976b-a221182640c4" />


<img width="714" height="554" alt="image" src="https://github.com/user-attachments/assets/e9af1dbf-8a42-471f-899f-549cca2390eb" />

  
   e) Función de probabilidad

<img width="752" height="532" alt="image" src="https://github.com/user-attachments/assets/ef184044-7af9-4dd6-b6c5-8bdf40d98369" />


Cálculo con librerias

<img width="799" height="298" alt="image" src="https://github.com/user-attachments/assets/61c6260c-9bae-4df9-be53-fee5241cd418" />


<img width="682" height="563" alt="image" src="https://github.com/user-attachments/assets/9b50a839-5a9a-4414-be25-680665227090" />

   
   f) Curtosis

   <img width="813" height="598" alt="image" src="https://github.com/user-attachments/assets/51c8d9a1-f85e-4dae-aab5-2be6e29304b9" />


Valor de curtosis: 5.3752

Cálculo con librerias.

<img width="952" height="653" alt="image" src="https://github.com/user-attachments/assets/c83d72ae-0869-4a7a-b085-15be8cacd53a" />


<img width="1032" height="697" alt="image" src="https://github.com/user-attachments/assets/38b5755e-d2d3-4fa7-ba98-252a529be51f" />


# Parte B

4. Gráfica de la Señal Capturada utilizando el Generador de Señales Biológicas
   
Para la captura de la señal ECG  generada utilizando el generador de señales biológicas, se tuvo en cuenta una frecuencia de muestreo de 1000hz lo que quiere decir que por cada segundo se toman 1000 muestras. 
Es de importancia mencionar que para la adquisición de la señal, se utilizaron dos métodos, el primer método empleado hace referencia al uso de MATLAB en donde se capturo la señal, obteniendo la gráfica de la respectiva señal y un documento en excel en formato csv con los respectivos datos referentes a la señal, y el segundo método hace referencia al uso de librerias en python para adquirir la señal por medio del daq.

A continuación se muestra el código utilizado para obtener la gráfica de la señal adquirida, utilizando el documento en formato csv que se obtuvo por medio de la captura de la señal en MATLAB.

<img width="1281" height="537" alt="image" src="https://github.com/user-attachments/assets/486c0464-0ecd-4103-8f8e-e38ee8582471" />


Gráfica de la Señal Capturada

<img width="1073" height="479" alt="image" src="https://github.com/user-attachments/assets/55af60ea-aa79-47c2-b085-16f498023b17" />


5. Cálculos Estadísticos Descriptivos
   
6. Comparación de Resultados Obtenidos en la Parte A y Parte B
   
# Parte C

7. ¿ Qué es la Relación Señal Ruido (SNR)?
   
SE define como la razón entre la energía de una señal y la energía de ruido expresada en decibeles (dB), y brinda información sobre el nivel de ruido de fondo presente en una señal de habla u otra.

a)Ruido Gaussiano:

Es un tipo de señal aleatoria que tiene una función de densidad de probabilidad (PDF) igual a la de la distribución normal. En términos más simples, es un tipo de ruido que se caracteriza por su aleatoriedad e imprevisibilidad.

Una de las características clave del ruido gaussiano es que tiene una media de cero y una varianza constante. Esto significa que el ruido se distribuye uniformemente alrededor de cero, sin sesgo hacia valores positivos o negativos. Esto hace que el ruido gaussiano sea un modelo ideal para muchos fenómenos naturales, ya que refleja con precisión la variabilidad y la aleatoriedad presentes en los datos del mundo real.

En el campo del procesamiento de señales, el ruido gaussiano se utiliza a menudo como modelo de las fluctuaciones aleatorias que pueden producirse en las señales electrónicas. Al añadir ruido gaussiano a una señal, los investigadores pueden simular los efectos del ruido en el rendimiento de un sistema y desarrollar estrategias para mitigar su impacto.

Contaminación la señal con ruido gaussiano y medición del SNR

b) Ruido Impulso:

Un ruido de impulso es definido como un único ruido transitorio (o una serie de ellos) de extremadamente corta duración en el cual el nivel de presión sonora asciende rápidamente hasta un nivel pico de presión sonora, y a partir de allí desciende exponencialmente hasta el ruido ambiental. El ruido de impulso surge principalmente como resultado de una repentina liberación de energía en el medio, energía eléctrica en el caso de la ionización del aire, como en cortocircuitos, o energía química por la liberación súbita de gases, como en una descarga explosiva de un arma de fuego.

Contaminación la señal con ruido impulso y medición del SNR.

c)Ruido Tipo Artefacto

Contaminación la señal con ruido tipo artefacto y medición del SNR
9. Análisis de Resultados
10. Conclusiones
11. Referencias
