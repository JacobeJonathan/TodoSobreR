# Curso fundamento con R
![postgre_instal_](src/1.webp)
- [Instalando nuestras herramientas](#Instalandonuestrasherramientas)
- [Importarachivos](#Importarachivos)
- [Tipos de datos](#Tiposdedatos)
- [Estructura del dataset del proyecto](#Estructuradeldatasetdelproyecto)
- [Vectores](#Vectores)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)
- [Primero calculos](#PrimerosCalculos)


## Instalandonuestrasherramientas
- ¿Qué es la economía naranja?
  - Es donde se mezclan las industrias culturales con las áreas de soporte como el desarrollo de aplicaciones o software.

  - Buscaremos responder a la pregunta:
  - Si tienes un startup que hace software, ¿en qué país abrirías una oficina?

  - El dataset de economía naranja fue creado por la profesora con las siguientes variables:

    - Aporte de servicios a PIB.
    - Aporte de economía naranja a PIB.
    - Penetración de internet.
    - Inflación.
    - Tasa de desempleo.
    - Población debajo de la línea de pobreza.
    - Edad mediana de la población.
    - Porcentaje de la población entre 25-54 años.
    - Inversión en educación %PIB.
  - Instalando: 
    - R: https://cran.r-project.org/
    - RStudio: https://www.rstudio.com/products/rstudio/download/
    - OrangeEconomiGithub: https://github.com/sap0408/Orange-Economy

  - ![Instaladores](src/1.png)
  - ![R y Rstudio instalado corectamente](src/2.png)
## Importarachivos
- Primero importar bien los archivos en Rstudio
  - ![Instaladores](src/3.png)
## PrimerosCalculos
- En esta clase vamos a hacer unos cuantos cálculos dentro de R Studio para ir acostumbrándonos a su sintaxis y comandos útiles.

- Dos comandos que utilizaras muy seguidos son:

  - (Ctrl + L): Se encarga de borrar la consola.
  - (Ctrl + Enter): Realiza la operación que selecciones.
  - Asignar un valor a una variable dentro de R se hace mediante el par de signos <- quedando, por ejemplo:

  - x <- 10
  - La función View nos muestra nuestro dataset en forma de tabla.
 - Comandos:
  - View(Orangec) = Vemos la tabla llamada Orangec
  - cotrl + l = se limpia la consola
  - ctrl + enter = para ejecutar 
  - <-  es el signo igual(=) en R
  - Tabien podemos utilizar el = que es el mismo
  - ![Instaladores](src/4.png)
## Tiposdedatos
- str(mtcars)   str = estructura
- ![Instaladores](src/5.png)
- Para conocer la estructura de un dataset, utilizamos la función str() (que significa structure o estructura), pasandole como parámetro el nombre del dataset en cuestión.
­
- En la información arrojada podemos visualizar los tipos de datos:
- (se recomienda comprender los fundamentos de la programación)
- int: Enteros. Números “redondos” como 1, 2, 3, 10, 100.
- num: Numérico. Números flotantes (o de coma flotante, decimales), como 1.5, 2.3, 3.2, 0.01.
- logi: Booleanos. Valores de true o false
­
- Vale la pena aclarar que en los datasets, los valores booleanos pueden estar representados con los enteros (int) 1 y 0, true o false respectivamente.
Para cambiar el tipo de dato, podemos llamar al dataset, situarnos en la variable, y utilizar el método as.logical().
dataset$var = as.logical(dataset$var)
­
- También vimos la variable Factor, se usa para clasificar los datos según su grupo o categoría.
­
- Hubo dos términos claves, observaciones y variables.
Observaciones: Filas.
  - Variables: Columnas.
  - Donde fila y columna tienen el mismo significado que tienen en una tabla convencional; fila y observación son sinónimos, y variables y columnas también.

##  Estructuradeldatasetdelproyecto
- summary: función que nos va a mostrar un resumen del dataset que le mandemos.
- transform: función para modificar los valores de un dataset.
- View(orangeec)
- str(orangeec)
- ojo: desactivar el heading sino no vamos poder hacer el summary al momento de importar el archivo
- summary(orangeec) nos muestra minimo macimo mediana
- tranformar de libras a kilos:
  - mtcars.new <- transform(mtcard,wt=wt*1000/2)
  - mtcars.new
  - summary(mtcars.new)
## Vectores
- Un vector es un ente matemático que se usa para guardar información de un mismo tipo, dentro de R se crean los vectores con la función c.

  - sum es una función que como su nombre lo indica,retorna la suma de los valores que le indiquemos.
- ![Instaladores](src/6.png)
- [Utilizar vectores profesionalmente](/comousarvectoresenR.pdf)