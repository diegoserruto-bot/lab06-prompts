# Bitacora de prompts

Laboratorio 06: Fundamentos de Ingenieria de Prompts. Herramienta de IA usada: (ChatGPT)

## Ejercicio 2: Tokens y ventana de contexto

| Texto                              | Tokens | Caracteres |
| ---------------------------------- | -----: | ---------: |
| Los estudiantes programan en Java. |      8 |         36 |
| The students program in Java.      |      7 |         30 |
| desafortunadamente                 |      4 |         18 |

```
La cantidad de tokens no siempre coincide con la cantidad de palabras. Una palabra larga como “desafortunadamente” puede dividirse en varios tokens. También se puede observar que las dos frases tienen diferente cantidad de tokens aunque expresan una idea similar.
```

### ¿Qué paso en los pasos 4 y 5?

En el paso 4, le di a la IA el contexto para que supiera que la aplicación era TiendaTec y que utilizaba Java Swing.

En el paso 5, La IA respondió correctamente, por lo que me da a entender que la memoria de ChatGPT puede conservar información entre chats.

## Ejercicio 3: Temperatura

### Resultados

| Temperatura | BiblioTec | LibroYa | PrestaLibro | LectoGo | PaginaLibre | NubeDeTinta |
| ----------: | --------: | ------: | ----------: | ------: | ----------: | ----------: |
|           0 |    100.0% |    0.0% |        0.0% |    0.0% |        0.0% |        0.0% |
|         0.5 |     65.3% |   24.0% |        8.8% |    1.2% |        0.4% |        0.2% |
|           1 |     44.5% |   27.0% |       16.4% |    6.0% |        3.7% |        2.4% |
|         1.8 |     32.2% |   24.4% |       18.5% |   10.6% |        8.0% |        6.4% |

### Observacion

Cuando sube la temperatura, los nombres se vuelven más variados y tienen probabilidades más parejas.
El simulador no crea nombres nuevos porque solo puede escoger de la lista que ya tiene.

## Ejercicio 4: Prompt vago vs estructurado

| Criterio                            | Prompt vago | Prompt estructurado |
| ----------------------------------- | ----------- | ------------------- |
| Menciona el objetivo del sistema    | Si          | Si                  |
| Menciona a los usuarios principales | No          | Si                  |
| Tiene exactamente 3 funcionalidades | No          | Si                  |
| Esta en 3 parrafos                  | No          | Si                  |
| Lo usaria en un informe real        | No          | Si                  |

El prompt estructurado dio una respuesta más específica y ordenada porque indicaba qué debía incluir. En cambio, el prompt vago dio una respuesta más general y sin tantos detalles.

## Ejercicio 5: Anatomia de un prompt

| Componente  | Texto de mi prompt                                                          |
| ----------- | --------------------------------------------------------------------------- |
| Rol         | Actua como desarrollador Java.                                              |
| Instruccion | Crea un programa en Java para gestionar los productos de una tienda.        |
| Contexto    | Usando una clase Producto con los atributos codigo, nombre, precio y stock. |
| Ejemplo     | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio).    |
| Formato     | Explica primero la estructura de la clase y luego presenta el codigo Java.  |

### Cambios por nivel

**Nivel 1:** Se indico el rol y la tarea, por lo que la respuesta dejo de ser general y se enfoco en Java.

**Nivel 2:** Se agrego el contexto de la tienda y la clase Producto, haciendo que la respuesta sea mas especifica.

**Nivel 3:** Se indicaron los atributos que debia tener la clase, por lo que el codigo tuvo una estructura mas definida.

**Nivel 4:** Se pidio explicar primero la estructura y despues mostrar el codigo, haciendo que la respuesta sea mas ordenada.

**Nivel 5:** Se agrego un ejemplo del estilo de los metodos, por lo que la respuesta siguio una forma mas especifica al escribir getters y setters.

## Ejercicio 6: Del prompt basico al profesional

| Qué revisar                                            | Cumple (Sí / No) |
| ------------------------------------------------------ | ---------------- |
| ¿Está escrito en Java y usa Swing?                     | Sí               |
| ¿Pide correo y contraseña?                             | Sí               |
| ¿Explica el funcionamiento antes o después del código? | Sí               |
| ¿El código está organizado en clases?                  | Sí               |
| ¿Valida los datos que ingresa el usuario?              | Sí               |

```
Actua como desarrollador Java. Crea un ejemplo de login para una aplicacion de escritorio utilizando Swing. El usuario debe ingresar correo y contrasena. Explica brevemente el funcionamiento y presenta el codigo organizado por clases
restricciones: no uses librerias externas, valida que el correo contenga @ y que la contrasena tenga al menos 8 caracteres, y muestra los mensajes con JOptionPane.
```
