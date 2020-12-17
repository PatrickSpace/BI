# Divemotor-Analytics
Este trabajo inicia con la construcción de un modelo dimensional incluyendo todas sus fases previas.
1 Definición de requerimientos clave para medición de KPIs y datos escenciales para los procesos de Compra e Importación.
2 Diseño de modelos Starnet por cada requerimiento encontrado.
3 Diseño del Bus Matrix (Medidas x Procesos) de la solución.
4 Definir medidas y dimensiones a utilizar.
5 Construir el modelo dimensional lógico (Base de Datos)  

Requisitos para implementar la solución:
- Visual Studio 2015
- SQL Server Management Studio 
- Power BI

## Transformación de Datos (ETL)
En la carpeta ETL encontrarán una carpeta llamada **TP** la cual es una solución de Integration Services realizada en Visual Studio 2015.
Esta solución tiene 2 paquetes que extraen y transforman datos a partir de un excel. El primer paquete extrae los datos del excel y los formatea al tipo de datos de una base de datos SQL. El segundo paquete funciona como una confirmación de los datos generados en la base de datos inicial llevando los datos a una final con las relaciones correspondientes al modelo dimensional planteado.
*Para abrir la solución solo es necesario hacer doble click en el archivo TP.sln*

## Integración de una solución Analysis Services con SQL Server (Cubo)
Para realizar la integración es necesario realizar una conexión con Analysis Service dentro del SQL Server Management Studio.
En esta etapa del proyecto se integran las medidas y las dimensiones en una herramienta denominada Cubo Dimensional, una solución incluida dentro de Visual Studio. Para la integración se construyó un Data Source View definiendo las medidas y dimensiones acorde al modelo dimensional.
*Para abrir la solución solo es necesario hacer doble click en el archivo TF.sln en la carpeta Cubo/TF*

## Backup y Datos
Los datos iniciales se encuentran en la carpeta Datos.
El backup de la base de datos (modelo dimensional) se encuentra en la carpeta Cubo
