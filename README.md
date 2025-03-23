# Estadistica Inferencial

Practica de conceptos de estadistica inferencial utilizando la libreria scipy

Simulacion y visualiza una distribución Poisson con parámetro lambda = 2.5 y una muestra de 1000. Esto significa que, en promedio, ocurren 2.5 terremotos de magnitud mayor a 8.5 en la escala de Richter durante un año.

Cargamos librerías y módulos necesarios
<br>![image](https://github.com/user-attachments/assets/88453e58-b344-49c4-9580-8d4633834054)


Realizamos la simulación y distribucion con los parametros definidos
<br>![image](https://github.com/user-attachments/assets/c14b78c5-b852-489c-ae2c-cc49403c0702)
<br>![image](https://github.com/user-attachments/assets/fa1b7d8f-f9c6-4c93-b221-7134b5e1142a)

Con esta simulación, modelamos el número de terremotos que pueden ocurrir por año durante los siguientes 1000 años.

Realizamos la simulación con los nuevos parametros
<br>![image](https://github.com/user-attachments/assets/cadf15ea-c1d6-469c-bbb4-707fec7c1184)
<br>![image](https://github.com/user-attachments/assets/efeca9a1-32f9-4b50-8771-3336b7693c1e)

Podemos seguir observando que con estos nuevos parámetros la mayor ocurrencia de eventos ocurridos en 1000 años es de 2500

---

Usando el set de datos marketing_campaign.csv, realizamos una prueba de hipótesis para contrastar si el número de compras en línea (NumWebPurchases) tiene alguna relevancia con el número de visitas a la página web (NumWebVisitsMonth).
<br>![image](https://github.com/user-attachments/assets/1b53bc15-1ac8-49b2-8990-bf41a0217a5f)

Definimos hipótesis
<br>![image](https://github.com/user-attachments/assets/14ef06a9-1704-41f0-978b-ce4a1ce4d04e)

Realizamos una visualización entre las dos variables para obtener una idea de cómo se comporta la información
<br>![image](https://github.com/user-attachments/assets/92178c11-bdd5-40ad-b3fc-5b3b637c9e87)
<br>La información aunque no es completamente clara, muestra una correlación linear con algunos outliers

Agrupamos la información en dos categorías: clientes con alto número de visitas (> 5) y bajo número de visitas (≤ 5) para realizar una prueba ANOVA
<br>![image](https://github.com/user-attachments/assets/e48a05ab-f3c5-4755-88de-9fe74295fbf9)

Realizamos la prueba estadística
<br>![image](https://github.com/user-attachments/assets/96e82104-8eb3-4506-9204-4b3a9238452f)

Se muestra por los resultados obtenidos que se rechaza la hipótesis nula, lo que significa que las variables sí están relacionadas.
<br>Por haber obtenido un f-stat muy alto y un p-value de 0 se realiza otra prueba alterna para comprobar los resultados
<br>![image](https://github.com/user-attachments/assets/fcfe50a3-c552-4b60-b4c9-5ccf41408aba)

La prueba de Pearson nos muestra unos resultados similares y de igual manera rechaza la hipótesis.
