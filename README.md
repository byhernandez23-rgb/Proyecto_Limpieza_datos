# Proyecto_Limpieza_datos
Automatizar un proceso de limpieza y preparación de archivos para la asignación de cuentas para agencias de cobranza


1. Objetivo del Proyecto

Automatizar el proceso limpieza y preparación de archivos para la asignación de cuentas para agencias de cobranza de acuerdo con las siguientes reglas.

Reglas de asignación:

 **Remesa normal (1-9) dentro y fuera.
 
1.- Se limpia cada pestaña el archivo AZUL_DENTRO, AZUL_FUERA: se cambia Bucket por su abreviación BK, fechas de cambios de Bucket, Fecha de retiro, Grupo no pueden estar vacías.
2.- AZUL_FUERA: se cambia la Remesa 300 por la misma que está en AZUL DENTRO
3.- Se juntan las dos pestañas en una.
4.- Se distribuye por agencias.
5.- Enviar correo.
 

**Remesa Trustonic (501-509).

 Solo una pestaña todas son Bucket 1

1.- Se limpia la pestaña REMESA_500: se cambia Bucket por su abreviación BK, fechas de cambios de Bk, fecha de retiro, grupo no pueden estar vacías.
2.- NO distribuye por agencias.
3.- Solo se gestionan internamente.
4.- Enviar correo.
 

**Remesa Bibani (801-809)
 
 Solo una hoja son pocas cuentas, es asignación de Bucket 3, que no recupero la agencia designada, se asigna a las 3 agencias.
 
1.- Se limpia la hoja se cambia Bucket por su abreviación BK, Fechas de cambios de Bucket, Fecha de retiro, grupo, no pueden estar vacías.
2.- Se distribuye entre las 3 agencias.
3.- Se manda por correo.


**Remesa Trustonic - Interna (701-709)
 
 Cuentas que se retiran de la agencia interna y se asignan a las 3 agencias, todas son Bucket 3.
 
1.- Se limpia la hoja se cambia Bucket por su abreviación BK, Fechas de cambios de Bucket, Fecha de retiro, Grupo no pueden estar vacías.
2.- Se distribuye por agencias.
3.- Se manda por correo.
 
**Remesa Especial (601-609)

Cuentas asignadas en una Agencia especifica que ya no se recuperaron en Bucket 1 y Bucket 2 al brincar a Bucket 3 se le retiran a la Agencia y se asignaron a las 3 agencias Externas.

1.- Realizar el retiro de las cuentas a Agencia especifica.
2.- Se limpia la hoja: se cambia Bucket por su abreviación BK, Fechas de cambios de Bucket, Fecha de retiro, Grupo no pueden estar vacías.
3.- Se distribuye por agencias.
4.- Se manda por correo.

________________________________________
2. Dataset

El dataset contiene la siguiente información:

•	Cuenta

•	Bucket

•	Remesa

•	Agencia

•	Cartera

•	Fechas de cambio de Bucket

•	Fecha de retiro

________________________________________
3. Librerías

Pandas

Pandas es una librería especializada en manipulación y análisis de datos estructurados. Proporciona estructuras de datos eficientes como DataFrame y Series, que permiten trabajar con información tabular de forma similar a una hoja de Excel o una tabla SQL.


Funciones principales:

•	Lectura y escritura de datos (CSV, Excel, SQL, JSON).

•	Limpieza y transformación de datos.

•	Filtrado, agrupaciones y agregaciones.

•	Análisis estadístico básico.


OS

La librería os permite interactuar con el sistema operativo desde Python. Se usa para manejar rutas, archivos, carpetas y variables del entorno.


Funciones principales:

•	Crear o eliminar directorios.

•	Obtener rutas de archivos.

•	Navegar entre carpetas.

•	Ejecutar operaciones del sistema.

Glob

La librería glob permite buscar archivos que coincidan con un patrón específico dentro de un directorio, usando comodines similares a los de la terminal.


Funciones principales:

•	Listar archivos por tipo o patrón.

•	Buscar archivos en múltiples carpetas.

•	Automatizar lectura de muchos archivos.


4. Código

<img width="1137" height="583" alt="image" src="https://github.com/user-attachments/assets/1d9a2896-ecf6-413e-890b-7e17fcd31b8f" />


<img width="1111" height="614" alt="image" src="https://github.com/user-attachments/assets/2cc7c6c2-cc98-4dc7-9c42-1079c12ae6c8" />


<img width="1119" height="612" alt="image" src="https://github.com/user-attachments/assets/29a77210-c180-4c41-bcda-b2ff5c281818" />


<img width="1094" height="588" alt="image" src="https://github.com/user-attachments/assets/fb007e9f-90ec-49ef-aedb-38a89aa7482a" />


________________________________________
👤 Autor
Miguel Ángel Hernández
Data Analyst | Business Intelligence | Pricing & Retail Analytics
