# Guía básica README

***
### Índice

1. [¿Qué es un archivo README?](#¿qué-es-un-archivo-readme)
2. [¿Qué debería contener un archivo README?](#¿qué-debería-contener-un-archivo-readme)
3. [Introducción a Markdown](#introducción-a-markdown)
   1. [Títulos](#títulos)
   2. [Texto común](#texto-común)
   3. [Texto en cursiva, negrita y tachado](#texto-en-cursiva-negrita-y-tachado)
   4. [Links](#links)
   5. [Imágenes](#imágenes)
   6. [Hipervínculos](#hipervínculos)
   7. [Listas](#listas)
   8. [Código](#código)
   9. [Tablas](#tablas)
   10. [Linea horizontal](#linea-horizontal)
4. [Plantilla README.md](#plantilla-readme.md)
5. [Últimas aclaraciones y recomendaciones](#últimas-aclaraciones-y-recomendaciones)

***
## ¿Qué es un archivo README?

Un archivo README debe contener **información importante** sobre el sistema, proyecto o software al que se esta refiriendo.

Por convención, es un archivo **.md** que hace referencia al lenguaje de marcado **Markdown.**

Se suele escribir *README* en mayúsculas, para que de este modo los sistemas que diferencian entre mayúsculas y minúsculas listarán el archivo antes que todos los demás.

## ¿Qué debería contener un archivo README?

Dependiendo del propósito del mismo pueden haber mas o menos secciones, pero en general es común encontrar las siguientes:

- Una descripción general del proyecto.
- Estado del proyecto, especialmente si este aun esta en desarrollo. Aquí se deben mencionar los cambios planeados y la dirección general del proyecto, y en el caso de que este ya este terminado también se debe especificar.
- Los requisitos del entorno de desarrollo para una correcta integración.
- Una guía par ala instalación y el correcto funcionamiento.
- Una lista con las tecnologías y/o módulos utilizados y, si es posible, links con mas información.
- Los proyectos de código abierto pueden incluir una sección donde se puedan aclarar ciertas dudas como, por ejemplo, *¿cómo solucionar ciertos problemas? ¿cómo pueden nuevos desarrolladores impulsar cambios en el código?*
- Bugs o errores conocidos.
- Una sección de preguntas frecuentes con todas las posibles preguntas planteadas hasta la fecha y sus respectivas respuestas.
- Información sobre derechos de autor y licencias.

## Introducción a Markdown

Markdown es un lenguaje de marcado que fue pensado como un lenguaje plano que se convierta facilmente en HTML con la ayuda de caracteres de formateo.

A continuación se van a explicar nociones básicas de este lenguaje de marcado, como aplicarlo y ejemplos del mismo. Al finalizar se dará un ejemplo general de un archivo README.md como plantilla.

### Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

    # Título 1 OR ========== (debajo del texto del título)
    ## Título 2 OR ---------- (debajo del texto del título)
    ### Título 3
    #### Título 4
    ##### Título 5
    ###### Título 6

### Texto común

Texto común

    Texto común

### Texto en cursiva, negrita y tachado

*Texto en cursiva*
**Texto en negrita**
***Texto en cursiva y negrita***
~~Texto tachado~~

    *Texto en cursiva* OR _Texto en cursiva_
    **Texto en negrita** OR __Texto en negrita__
    ***Texto en cursiva y negrita*** OR ___Texto en cursiva y negrita___
    ~~Texto tachado~~

### Links

[Nombre del link](https://www.google.com/ "Título opcional") OR https://www.google.com/ OR <https://www.google.com/>

    [Nombre del link](https://www.google.com/ "Título opcional") OR https://www.google.com/ OR <https://www.google.com/>

### Imágenes

![Nombre de la imagen](img-ejemplo.png "Título opcional")

    ![Nombre de la imagen](img-ejemplo.png "Título opcional")

### Hipervínculos

[Título del hipervínculo](#Títulos "Descripción opcional")

    [Título del hipervínculo](#Títulos "Descripción opcional")
    >>>ACLARACIÓN: En el caso de que luego del # hubiesen espacios en blanco, se deben reemplazar por un -

### Listas

- Lista desordenada
  - Sub-item
    - Segundo sub-item
- Segundo item 

~~~
    - Lista desordenada
      - Sub-item
        - Segundo sub-item
    - Segundo item
    OR
    * Lista desordenada
      * Sub-item
        * Segundo sub-item
    * Segundo item
~~~

1. Lista ordenada
   1. Sub-item
   2. Segundo sub-item
2. Cambio de número

~~~
    1. Lista ordenada
      1. Sub-item
      2. Segundo sub-item
    2. Cambio de número
~~~

- [ ] Tarea incompleta
  - [ ] Sub-tarea
- [X] Tarea completa

~~~
    - [ ] Tarea incompleta
      - [ ] Sub-tarea
    - [X] Tarea completa
~~~

### Código

`funcion()`

```python
    def funcion(a):
        for i in a:
            print(a)
```

    `funcion()`

    ```python
        def funcion(a):
            for i in a:
                print(a)
    ```

### Tablas

Tabla basica

| Columna 1 | Columna 2 |
| --------- | --------- |
| Celda 1   | Celda 2 |
| Celda 3   | Celda 4 |

Tabla alineada

| Alineado izquierda | Alineado centro | Alineado derecha |
| :--------------- | :-------------: | ---------------: |
| Celda 1 | Celda 2 | Celda 3 |
| Celda 4 | Celda 5 | Celda 6 |

    | Columna 1 | Columna 2 |
    | --------- | --------- |
    | Celda 1   | Celda 2 |
    | Celda 3   | Celda 4 |

    | Alineado izquierda | Alineado centro | Alineado derecha |
    | :--------------- | :-------------: | ---------------: |
    | Celda 1 | Celda 2 | Celda 3 |
    | Celda 4 | Celda 5 | Celda 6 |

### Linea horizontal

***

    ***

## Plantilla README.md

    ## Indice de contenidos
    1. [Información general](#Información-general)
    2. [Tecnologias](#Tecnologias)
    3. [Instalación](#Instalación)
    4. [Colaboraciones](#Colaboraciones)
    5. [FAQs](#faqs)
    ### Información general
    ***
    Aquí escribe una descripción general del proyecto. Es muy recomendable colocar el estado actual del proyecto en esta parte. 
    ### Captura de pantalla
    ![Texto de la imagen](url de la imagen)
    ## Tecnologias
    ***
    Colocar una lista de tecnologias utilizadas en este proyecto:
    * [Nobre de la tecnologia 1](https://ejemplo1.com): Version 12.3 
    * [Nobre de la tecnologia 2](https://ejemplo2.com): Version 2.34
    * [Modulo 1](https://ejemplo3.com): Version 1234
    ## Instalación
    ***
    Aquí colocar una pequeña introducción a la instalación. 
    ```
    $ git clone https://ejemplo1.com
    $ cd ../path/to/the/file
    $ npm install
    $ npm start
    ```
    Información adicional: Cualquier aclaración que valga la pena mencionar como puede ser variaciones en la instalación dependiendo del sistema operativo, etc.
    ## Colaboraciones
    ***
    Un pequeño intructivo de como poder aportar al proyecto si asi se desea.
    * Quizas alguna forma de contacto. 
    * O quizas como hacer llegar esas modificaciones.
    ## FAQs
    ***
    Una lista de las preguntas mas frecuentes sobre el proyecto
    1. **Pregunta 1 (en negrita)**
    Respuesta a la primer pregunta. 
    2. **Pregunta 2 (en negrita)** 
    Quizas alguna pregunta requiera de una lista para responderla:
    * Primer punto
    * Segundo punto
    * Tercer punto
    3. **Pregunta 3 (en negrita)**
    En las respuestas se pueden usar tanto palabras en *cursiva* como **negrita** para resaltar ciertos puntos.
    4. **Pregunta 4 (en negrita)**
    O quizas sea necesaria una tabla:
    | Columna 1 | Columna 2 | Columna 3 |
    |:--------------|:-------------:|--------------:|
    | Alineado izquierda | Alineado centro | Alineado derecha |

## Últimas aclaraciones y recomendaciones

Los archivos README suelen ser escritos en *Markdown*, como se fue explicando anteriormente y como es recomendable hacer, pero tambien se pueden escribir en otros formatos como pueden ser **.txt**, **.docs**, etc pero estos no son tan recomendables como el **.md**

Por ultimo tambien aclarar que siempre es preferible redactar el README en ingles por una cuestion de alcance y entendimiento de todo posible publico que lo lea, en este caso se dio una explicación en español para facilitar el entendimiento del mismo.
