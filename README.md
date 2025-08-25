# Laboratorio Análisis Estadístico De La Señal
# Parte A
1. Base de Datos Physionet
 La muestra tomada de la base de datos Physionet, seleccionando una señal ECG (electrocardiograma) de la duración correcta para sus posteriores cálculos estadísticos, con 200 muestras por segundo esto se evidencia en la frecuencia de muestreo de 200Hz. Este ECG se tomó de un subconjunto de electrocardiograma de diagnóstico.
   Se utilizo la muestra 40689238 deGow, B., Pollard, T., Nathanson, LA, Johnson, A., Moody, B., Fernandes, C., Greenbaum, N., Waks, JW, Eslami, P., Carbonati, T., Chaudhari, A., Herbst, E., Moukheiber, D., Berkowitz, S., Mark, R. y Horng, S. (2023). MIMIC-IV-ECG: Subconjunto coincidente de electrocardiograma de diagnóstico (versión 1.0). FisioNet . RRID: SCR_007345. https://doi.org/10.13026/4nqg-sb35
   
3. Importación y Gráfica de la Señal
   
Para esta parte del laboratorio se importó la señal en Python mediante los archivos .dat y .hea, y se hizo uso de la librería matplotlib para su visualización, en la gráfica se observan características típicas de un ECG como la onda P, el complejo QRS y las ondas T.

<img width="1216" height="159" alt="image" src="https://github.com/user-attachments/assets/6333b1b1-abac-44fa-8045-08e8edad4ffc" />

<img width="737" height="560" alt="image" src="https://github.com/user-attachments/assets/d88298a5-cd4c-43b9-bd20-e232a83ad403" />

2.1 Gráfica en Dominio del Tiempo

<img width="726" height="557" alt="image" src="https://github.com/user-attachments/assets/14e3fbff-16b1-420d-979a-5f7e71effee0" />

3. Cálculos Estadísticos Descriptivos
   
   Se calcularon de dos maneras distintas (con librerías y sin ellas) la media, la desviación estándar, coeficiente de variación, histograma, función de probabilidad y curtosis, primeramente se evidencia el programa sin el uso de las librerías y continuamente se verá las mismas medidas calculadas mediante librerías predefinidas de Python. 
   
   a) Media de la señal
 La media es un valor estadístico que representa el promedio de la señal, permitiéndonos establecer referencias de una actividad normal cardiaca para poder así detectar patrones anormales

<img width="849" height="328" alt="image" src="https://github.com/user-attachments/assets/e4dcc61c-e69a-490a-a208-1f4dee4a6271" />

--- RESULTADOS DEL CÁLCULO DE LA MEDIA ---
Suma total de todos los valores: 176.590000
Número total de muestras: 5000
Media de la señal: 0.035318

Luego se calculó nuevamente la media de la señal mediante el uso de librerias o funciones.

<img width="523" height="67" alt="image" src="https://github.com/user-attachments/assets/8ff4cc3f-7be0-4f4b-97ac-baac40d84ff2" />

media de la señal:0.035318

   b) Desviación Estandar
Este valor estadístico nos indica el grado de variabilidad de la señal con respecto a la media, este nos ayuda a identificar y analizar el comportamiento del corazón, ejemplo cuando se ve un valor elevado refleja fluctuaciones pronunciadas 

   <img width="682" height="453" alt="image" src="https://github.com/user-attachments/assets/93c075b3-6004-4706-b580-ac2c927d4801" />

Suma de diferencias al cuadrado: 110.156394
Varianza: 0.022031
Desviación estándar: 0.148429

Cálculo con librerias

<img width="550" height="69" alt="image" src="https://github.com/user-attachments/assets/7808999d-c404-45c3-9a46-6cc785ea2f1e" />

Desviación estandar:0.148429

   c) Coeficiente de variación
Este es una medida relativa ya que relaciona la desviación estándar con la media de la señal, por esto nos ayuda a comparar distintos registros cardiacos para identificar irregularidades del ritmo cardiaco.


   <img width="1073" height="312" alt="image" src="https://github.com/user-attachments/assets/3bbb2f38-1911-4617-a55f-85b86290edea" />

    Coeficiente de variación: 4.202655
 Coeficiente de variación (%): 420.27%

Cálculo con librerias

<img width="591" height="182" alt="image" src="https://github.com/user-attachments/assets/53ffb273-c6c7-4b68-8236-ffc4f4706d28" />


Coeficiente de variación: 420.27%
 
   d) Histograma
   Este es una representación gráfica donde se ve la distribución de los valores de la señal, nos permite visualizar los rangos más amplios y frecuentes de los datos.
   

<img width="572" height="679" alt="Captura de pantalla 2025-08-23 181744" src="https://github.com/user-attachments/assets/27260808-7e11-4cab-8982-98c58c7c44a9" />
<img width="1090" height="607" alt="Captura de pantalla 2025-08-23 210313" src="https://github.com/user-attachments/assets/4a7a467c-71a5-4681-a6fa-a0b2bd3bcb2b" />
<img width="1310" height="779" alt="Captura de pantalla 2025-08-23 211428" src="https://github.com/user-attachments/assets/3d57be6d-0fd8-4923-a0aa-f55ecb5c371b" />
<img width="1036" height="644" alt="Captura de pantalla 2025-08-23 210433" src="https://github.com/user-attachments/assets/64832e49-a5ba-4fff-a8c6-4d82ff63e089" />
<img width="696" height="538" alt="Captura de pantalla 2025-08-23 210521" src="https://github.com/user-attachments/assets/dea73d6a-b898-4c28-8550-74274234f37a" />
<img width="1310" height="781" alt="Captura de pantalla 2025-08-23 211509" src="https://github.com/user-attachments/assets/79c5c3ae-4f24-4dcf-b6d7-15932d64a274" />


   Cálculo con librerias.

<img width="497" height="142" alt="image" src="https://github.com/user-attachments/assets/a2b399de-d615-4ac7-976b-a221182640c4" />


<img width="714" height="554" alt="image" src="https://github.com/user-attachments/assets/e9af1dbf-8a42-471f-899f-549cca2390eb" />

  
   e) Función de probabilidad
Se usa para modelar el comportamiento de la señal y poder analizar sus tendencias permitiendo así analizar si tiene tendencias atípicas o normales.
   
<img width="699" height="650" alt="Captura de pantalla 2025-08-23 212151" src="https://github.com/user-attachments/assets/a6b7cede-c4aa-4a60-8396-89b95af00bac" />
<img width="788" height="561" alt="Captura de pantalla 2025-08-23 212452" src="https://github.com/user-attachments/assets/c061b33a-69c9-4739-9d7b-f5a4a6042595" />

<img width="752" height="532" alt="image" src="https://github.com/user-attachments/assets/ef184044-7af9-4dd6-b6c5-8bdf40d98369" />


Cálculo con librerias

<img width="799" height="298" alt="image" src="https://github.com/user-attachments/assets/61c6260c-9bae-4df9-be53-fee5241cd418" />


<img width="682" height="563" alt="image" src="https://github.com/user-attachments/assets/9b50a839-5a9a-4414-be25-680665227090" />

   
   f) Curtosis
   La curtosis nos permite describir el grado de concentración de la señal alrededor de la media. Nos ayuda a poder analizar si hay presencia de picos pronunciados o una distribución normal.
   <img width="958" height="698" alt="image" src="https://github.com/user-attachments/assets/630cae51-4cd3-4cb8-a225-7b76036a2f94" />
   <img width="841" height="743" alt="image" src="https://github.com/user-attachments/assets/3879537b-37bf-4d2a-b5b7-355b72a8805e" />


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


Gráfica de la Señal Capturada en mathlab

<img width="1073" height="479" alt="image" src="https://github.com/user-attachments/assets/55af60ea-aa79-47c2-b085-16f498023b17" />

Para el proceso de captura de la señal por medio del daq se toma la base de la importacion "nidaqmx" y con ello poder realizar la captura usando el hardware de la daq logrando guardar los datos en una variable gracias a la funcion "data=task.read", y configurar la frecuencia de muestreo con la funcion "task.timing.cfg_samp_clk_timing"

<img width="914" height="433" alt="image" src="https://github.com/user-attachments/assets/92be5712-f6b8-4be0-bcfc-52761e167881" />

y grafocando los datos con las funciones de mathplotlib tenemos la siguiente grafica 

<img width="552" height="411" alt="image" src="https://github.com/user-attachments/assets/c6f37c41-66ac-491d-b963-acd68559b983" />

posteriormente cargamos los datos en csv capturados a un google drive compartido donde empezamos a trabajarlos para sacar sus estadisticos no sin antes graficarlos ahí para asegurarnos de la ausencia de cualquier corrupcion en el archivo 

<img width="908" height="264" alt="image" src="https://github.com/user-attachments/assets/000ff4fc-8075-4744-93f6-a0c0804ef5e5" />

<img width="621" height="459" alt="image" src="https://github.com/user-attachments/assets/542e367c-6139-46af-ab1a-9a9000ddb387" />

usamos las librerias para repetir el proceso de la parte A ahora con nuestra propia señal

5. Calculos descriptivos
   
A) Media.

<img width="480" height="152" alt="image" src="https://github.com/user-attachments/assets/a808251b-5edf-4a3e-85c0-d625d793be50" />

B) desviacion estandar

<img width="536" height="164" alt="image" src="https://github.com/user-attachments/assets/568e7812-93f6-4f49-8a06-35f42d1ad759" />

C) coeficiente de variacion

<img width="640" height="96" alt="image" src="https://github.com/user-attachments/assets/04a89e43-eed3-4216-9380-e5fc5363041e" />

D) Histograma

   
<img width="496" height="122" alt="image" src="https://github.com/user-attachments/assets/5dfdfeea-2dc0-4cb9-82d3-cf6bd603bb03" />


<img width="592" height="452" alt="image" src="https://github.com/user-attachments/assets/93c04750-ae8f-42bd-b662-712e4da05cb9" />

E) funcion de probabilidad


<img width="773" height="212" alt="image" src="https://github.com/user-attachments/assets/c51e9142-d192-4967-9ad2-91745f077bf8" />


<img width="576" height="459" alt="image" src="https://github.com/user-attachments/assets/68f2cc29-e411-44f9-8ddc-be36dae76421" />

F) Curtosis


<img width="547" height="101" alt="image" src="https://github.com/user-attachments/assets/a0147b3a-a8ee-4352-87be-adc1156c6c53" />

G) Sintesis


<img width="928" height="360" alt="image" src="https://github.com/user-attachments/assets/289b481a-f853-41ea-8c2e-536cfdca346f" />

<img width="555" height="475" alt="image" src="https://github.com/user-attachments/assets/15d31fb2-ed84-4e89-adc9-99eaef67635f" />



   
   
7. Comparación de Resultados Obtenidos en la Parte A y Parte B

   Análisis de Resultados
   
   En este momento veremos las diferencias e igualdades entra la parte A (Señal sacada de physionet, y la parte B (Señal capturada en el generador), para iniciar veremos la frecuencia de muestreo ya que en los dos casos se usó una distinta la primer parte la señal fue registrada a 200 Hz mientras la de la segunda parte se capturo con una frecuencia de 1000Hz, esto se hizo con el objetivo de que la segunda parte tuviera más detalle temporal. como ya se había mencionado los datos se obtuvieron de manera distinta lo que también sería una diferencia entre señales. 
 
   Seguidamente compararemos las medidas estadísticas calculadas en ambas partes, empezaremos con la media en ambas partes el valor nos dio muy cercano a cero (0 ) lo que nos muestra la estabilidad en la línea base de los ECG, continuamos con la desviación estándar en este ambos nos dio la magnitud esperada sin embargo en la señal de la parte B se evidencio un valor más predecible que el de la parte A, y por último el coeficiente de variación este se mantuvo alto en ambos caso demostrando así que efectivamente un ECG es una señal oscilatoria.

   Para finalizar la comparación hablaremos de la curtosis y el histograma, en el caso de la curtosis en ambas partes se mostraron valores altos por los picos pronunciados aunque en la parte A se nota una mayor irregularidad por ser una señal de un paciente real, en el caso del histograma vemos que se concentran en los valores centrales además de ver una cola alargada en cada gráfica demostrando así que tiene una naturaleza periódica
 
   
# Parte C

8. ¿ Qué es la Relación Señal Ruido (SNR)?
   
SE define como la razón entre la energía de una señal y la energía de ruido expresada en decibeles (dB), y brinda información sobre el nivel de ruido de fondo presente en una señal de habla u otra.

a)Ruido Gaussiano:

Es un tipo de señal aleatoria que tiene una función de densidad de probabilidad (PDF) igual a la de la distribución normal. En términos más simples, es un tipo de ruido que se caracteriza por su aleatoriedad e imprevisibilidad.

Una de las características clave del ruido gaussiano es que tiene una media de cero y una varianza constante. Esto significa que el ruido se distribuye uniformemente alrededor de cero, sin sesgo hacia valores positivos o negativos. Esto hace que el ruido gaussiano sea un modelo ideal para muchos fenómenos naturales, ya que refleja con precisión la variabilidad y la aleatoriedad presentes en los datos del mundo real.

En el campo del procesamiento de señales, el ruido gaussiano se utiliza a menudo como modelo de las fluctuaciones aleatorias que pueden producirse en las señales electrónicas. Al añadir ruido gaussiano a una señal, los investigadores pueden simular los efectos del ruido en el rendimiento de un sistema y desarrollar estrategias para mitigar su impacto.

<img width="810" height="386" alt="image" src="https://github.com/user-attachments/assets/efbdc97a-319b-4462-a838-cc9d9fb728e4" />

<img width="625" height="141" alt="image" src="https://github.com/user-attachments/assets/62f718ac-907a-4803-9d51-48d24b607100" />

Contaminación la señal con ruido gaussiano y medición del SNR

b) Ruido Impulso:

Un ruido de impulso es definido como un único ruido transitorio (o una serie de ellos) de extremadamente corta duración en el cual el nivel de presión sonora asciende rápidamente hasta un nivel pico de presión sonora, y a partir de allí desciende exponencialmente hasta el ruido ambiental. El ruido de impulso surge principalmente como resultado de una repentina liberación de energía en el medio, energía eléctrica en el caso de la ionización del aire, como en cortocircuitos, o energía química por la liberación súbita de gases, como en una descarga explosiva de un arma de fuego.

<img width="773" height="487" alt="image" src="https://github.com/user-attachments/assets/5cf78127-0cfb-4872-a2eb-2efbe970c260" />
<img width="623" height="150" alt="image" src="https://github.com/user-attachments/assets/15851932-aab8-4e40-ae8b-566545b49d20" />

Contaminación la señal con ruido impulso y medición del SNR.

c)Ruido Tipo Artefacto
<img width="816" height="453" alt="image" src="https://github.com/user-attachments/assets/af01510a-f9a5-446d-8fb5-7cf60610637b" />
<img width="1494" height="270" alt="image" src="https://github.com/user-attachments/assets/3d55e69d-5e06-4869-98d0-67a29938b92d" />

Contaminación la señal con ruido tipo artefacto y medición del SNR

09. Conclusiones
    
    En la parte A y B el análisis estadístico nos permitió comprobar que las señales generadas tanto por un paciente como por el generador comparten patrones con unas mínimas diferencias en cuanto a su regularidad y su dispersión

    Este laboratorio resalta la importancia de trabajar tanto con señales humanas como señales controladas ya que la primera seria usada para el estudio de señales auténticas mientras la generadas nos permite controlar métodos usados y un más certero análisis en condiciones predecibles

      
10. Referencias
    [1]. Gow, B., Pollard, T., Nathanson, L. A., Johnson, A., Moody, B., Fernandes, C., Greenbaum, N., Waks, J. W., Eslami, P., Carbonati, T., Chaudhari, A., Herbst, E., Moukheiber, D., Berkowitz, S., Mark, R., & Horng, S. (2023). MIMIC-IV-ECG: Diagnostic Electrocardiogram Matched Subset (version 1.0). PhysioNet. RRID:SCR_007345. https://doi.org/10.13026/4nqg-sb35

    [2]. Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C., Mark, R., ... & Stanley, H. E. (2000). PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation [Online]. 101 (23), pp. e215–e220. RRID:SCR_007345.
    [3]. MIMIC-IV-ECG: Diagnostic Electrocardiogram Matched Subset V1.0. (2023, 15 septiembre). https://physionet.org/content/mimic-iv-ecg/1.0/files/p1000/p10000032/s40689238/#files-panel
    [4]. Ruido gaussiano. (2025, 25 febrero). Wray Castle. https://wraycastle.com/es/blogs/glossary/gaussian-noise?srsltid=AfmBOoqh1igHvyUVctINCbA7JnQFLbgd82Pktf1aZJt6aFsWKpQMKrb4
    [5]. Vidal, D. (2021). Estudio del ruido impulsivo. www.academia.edu. https://www.academia.edu/61954308/Estudio_del_Ruido_Impulsivo
