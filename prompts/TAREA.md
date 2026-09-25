# Tarea: Mi prompt profesional

## Funcionalidad elegida

La funcionalidad elegida es un programa para calcular el promedio de tres notas de un estudiante y determinar si aprobo o desaprobo.

## Version 1: prompt basico

```
Crea un programa en Java que calcule el promedio de tres notas y muestre si el estudiante aprobo o desaprobo.
```

### Que cambie

En esta primera version escribi una instruccion sencilla indicando solamente lo que queria que hiciera el programa.

### Por que lo cambie

Queria comenzar con un prompt basico para observar que informacion podia faltar y que cosas podia mejorar en las siguientes versiones.

### Que mejoro en la respuesta

La IA entendio la funcion principal del programa, pero la respuesta podia ser diferente a lo que necesitaba porque no habia especificado detalles como el uso de Scanner, la nota minima o la forma de presentar la respuesta.

## Version 2

```
Crea un programa sencillo en Java que permita ingresar tres notas de un estudiante usando Scanner. Calcula el promedio de las tres notas y muestra si el estudiante aprobo o desaprobo. La nota minima para aprobar es 11. Explica brevemente como funciona el programa.
```

### Que cambie

Agregue el uso de Scanner, la cantidad de notas, la nota minima para aprobar y una explicacion breve del programa.

### Por que lo cambie

La primera version era muy general, por lo que agregue informacion para que la IA tuviera una idea mas clara de lo que necesitaba.

### Que mejoro en la respuesta

La respuesta fue mas especifica porque la IA ya conocia el lenguaje que debia utilizar, como ingresar las notas y cual era la condicion para aprobar.

## Version 3: prompt final

```
Actua como un profesor de programacion en Java que explica de manera sencilla a un estudiante que esta aprendiendo programacion. Crea un programa en Java que permita ingresar tres notas de un estudiante usando Scanner, calcule su promedio y muestre si aprobo o desaprobo, considerando que la nota minima para aprobar es 11. Como ejemplo, si las notas ingresadas son 14, 12 y 16, el promedio debe ser 14.0 y el resultado debe mostrar "Aprobado". Entrega primero el codigo Java dentro de un bloque de codigo y luego explica brevemente las partes principales del programa. No utilices librerias externas, no agregues funcionalidades que no fueron solicitadas y manten el programa sencillo.
```

### Que cambie

Agregue un rol, un contexto mas completo, un ejemplo, un formato para la respuesta y restricciones.

### Por que lo cambie

Queria que el prompt fuera mas preciso y que la IA tuviera toda la informacion necesaria para generar una respuesta cercana a lo que necesitaba.

### Que mejoro en la respuesta

La respuesta fue mas controlada y clara, ya que la IA conoce el tipo de explicacion que debe dar, los datos que debe utilizar y la forma en que debe presentar el resultado.

## Componentes del prompt final

| Componente  | Parte del prompt                                                                                                        |
| ----------- | ----------------------------------------------------------------------------------------------------------------------- |
| Rol         | Profesor de programacion en Java que explica de manera sencilla a un estudiante.                                        |
| Instruccion | Crear un programa que permita ingresar tres notas, calcular el promedio y mostrar si aprobo o desaprobo.                |
| Contexto    | El programa esta dirigido a un estudiante que esta aprendiendo los conceptos basicos de Java y debe utilizar `Scanner`. |
| Ejemplos    | Se proporcionan las notas 14, 12 y 16, con un promedio de 14.0 y resultado "Aprobado".                                  |
| Formato     | Primero mostrar el codigo Java dentro de un bloque de codigo y luego explicar brevemente sus partes principales.        |
| Restriccion | No utilizar librerias externas ni agregar funcionalidades que no fueron solicitadas.                                    |

## Evaluacion del resultado

| Criterio                                    | Resultado |
| ------------------------------------------- | --------- |
| El programa esta desarrollado en Java       | Si        |
| Permite ingresar tres notas                 | Si        |
| Utiliza `Scanner`                           | Si        |
| Calcula el promedio correctamente           | Si        |
| Indica si el estudiante aprobo o desaprobo  | Si        |
| Considera 11 como nota minima para aprobar  | Si        |
| Explica las partes principales del programa | Si        |
| No utiliza librerias externas               | Si        |

## Errores que evite

- **Ser demasiado general:** En la primera version solo indique que queria calcular el promedio de tres notas. Para evitar este error, en las siguientes versiones agregue informacion como el lenguaje Java, el uso de `Scanner`, la nota minima para aprobar y el resultado esperado.

- **No indicar el formato:** En las primeras versiones no especifique como queria recibir la respuesta. Para evitar este error, en la version final indique que primero se debe mostrar el codigo dentro de un bloque de codigo y despues una explicacion breve.
