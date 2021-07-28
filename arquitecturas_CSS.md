# Arquitecturas de CSS

## Objetivos

* **Predecible** > Escribir reglas claras
* **Reutilizable** > No escribir codigo redundante
* **Mantenible** > Que sea facil de leer y adaptarnos a los estandares
* **Escalable** > Que pueda crecer facilmente sin afectar el rendimiento

## Buenas practicas

* Establecer reglas para que el equipo se entienda
* Explicar la estructura base o dar los fundamentos del proyecto a un nuevo integrante
* Evitar hojas de estilo muy extensas
* Tener una buena documentacion explicando algunos aspectos del codigo

---

# OOCSS (Object Oriented CSS)

Se separa el diseno del contenido. Lo cual permite reutilizar mucho mejor el codigo. Por ejemplo, si el header y el footer ambos tienen un width de 100%, entonces se crea una clase general que se llame fullWidth (en vez de especificar ese width en la clase de cada uno de ellos)

# BEM (Block Element Modifier)

Se separan los bloques, los elementos y los modificadores. Por ejemplo si tenemos un header con 2 botones de colores: La clase del header se llamaria `header`, la del primer boton seria `header__button--red`, el segundo boton seria `header__button--yellow`.

Como puedes ver, se escriben las clases asi `bloque__elemento--modificador`

# SMACSS (Scalable and Modular Architecture CSS)

En esta metodologia se siguen los siguientes 5 pasos:

1. Definir los componentes base. (por ejemplo los botones)
2. Definir el layout, que son elementos que se utilizan una sola vez en nuestra pagina. (por ejemplo el header y el footer)
3. Definir el modulo, que son componentes que se van a utilizar en la aplicacion mas de una vez
4. Definir el estado de los componentes. Por ejemplo, un boton que al ser activado pase a verde, y al ser desactivado a rojo
5. Definir el tema de nuestra aplicacion

# ITCSS (Inverted Triangle CSS)

La idea de esta metodologia es dividir nuestros archivos de CSS en ciertas partes para que no se combinen entre si.

El triangulo se refiere a:

* Magnitud
* Especificidad
* Claridad

# Atomic Design

En esta metodologia se busca separar los elementos de forma jerarquica de la siguiente manera:

Atomos - Moleculas - Organismos - Templates - Paginas