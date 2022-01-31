Proyecto Final Grupo 1

Desarrollado por:

José Javier Olalla - Óliver García - Luis Miguel Señor

Presentación del ejercicio:

Se implementarán las tareas necesarias para llevar los datos desde la fuente hasta la capa de consumo dentro del datalake, para su posterior explotación. Con ello, se cubre un amplio espectro de proyectos Big Data y tecnologías usadas diariamente

Carga de los datasets:
Cargar los datasets en el lago y crear las tablas necesarias para poder acceder por consultas SQL.

Tratamiento de datos:
Se puede hacer una aproximación con consultas SQL, después se tiene que programar en un proyecto Spark con Maven multi módulo, o varios proyectos Maven, separando cada tipo de proceso en módulos/proyectos diferentes. Incluir las dependencias necesarias para cada módulo (Scala, Spark, etc.) y configurar los plugins necesarios y las fases de construcción del proyecto

El cliente quiere tener los siguientes puntos: 

 - Tabla maestra con el horóscopo y con países por continente. 
 - El equipo de desarrollo de negocio quiere implementar una funcionalidad para agrupar los usuarios por su horóscopo fijándose en la fecha de registro.  
 - Necesitan saber a qué continente pertenece cada usuario.
 - Se necesita saber cuántos usuarios por país pertenecen a cada signo del horóscopo, y cuál es el signo que tiene más usuarios a nivel mundial y cuál es el grupo que más escucha ese signo. 
 - ¿En qué continente deberían publicitar más la aplicación? ¿Hay algún continente que falte?  
 - Estas tablas tienen que estar disponibles en HIVE y en MySQL.
 - Saltarse la capa de registrar los resultados en Hive y registrarlo todo directamente en MySQL.
 - No usar las librerías de Spark para guardarlos los datos en el lago y luego acceder con Hive disponiendo tablas externas.

Las soluciones se crean en la nube de Azure, utilizando las siguientes herramientas:

Azure Data Lake Storage Gen2 - Clúster de HDInsight - Azure Data Factory - PySpark - Hive - Jupyter Notebooks - Azure Database for MySql
