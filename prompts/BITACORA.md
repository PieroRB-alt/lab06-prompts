# Bitacora de prompts 
  
## Laboratorio 06: Fundamentos de Ingenieria de Prompts. 
  
## Herramienta de IA usada: Chat gpt
  
## Ejercicio 2: Tokens y ventana de contexto 
| Texto | Caracteres | Tokens |
|---|---|---|
| Los estudiantes programan en Java. | 35 | 8 |
| The students program in Java. | 29 | 6 |
| desafortunadamente | 18 | 44 |

#### Durante la primera conversación la IA dio la respuesta correcta de acuerdo al marco de contexto. Durante la nueva conversación la IA también pudo dar una respuesta correcta porque ChatGPT usa la función de "Memoria" la cual almacena la información a través de las sesiones eliminando el problema del marco de contexto vacío.


## Ejercicio 3: Temperatura 

  | Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|---|---|---|
| 0 | 100.0% | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3% | BiblioTec, BiblioTec, BiblioTec, BiblioPrestamo, BiblioTec |
| 1.0 | 44.5% | BiblioTec, BiblioPrestamo, BiblioTec, UniBook, BiblioTec |
| 1.8 | 32.2% | BiblioPrestamo, LectioUni, BiblioPrestamo, UniBook, Librolink |

####  A temperaturas más altas los porcentajes se equilibran y empiezan a crear nombres menos comunes.No es posible que el simulador genere nuevos nombres ya que un aumento de la temperatura sólo afecta la probabilidad de seleccionar nombres sin aportar ninguna información nueva.

## Ejercicio 4: Prompt vago vs estructurado 
  
  | Criterio | Prompt vago | Prompt estructurado |
|---|---|---|
| Menciona el objetivo del sistema | No | Si |
| Menciona a los usuarios principales | No | Si |
| Tiene exactamente 3 funcionalidades | No | Si |
| Esta en 3 parrafos | No | Si |
| Lo usaria en un informe real | No | Si |

## Ejercicio 5: Anatomia de un prompt 

| Componente | Texto de mi prompt |
|---|---|
| Rol | Actua como desarrollador Java. |
| Instruccion | Crea un programa en Java... usando una clase Producto con los atributos codigo, nombre, precio y stock. |
| Contexto | ...para gestionar los productos de una tienda. |
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio (double precio). |
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java. |

### Nivel 1: En lugar de generar algún código la IA me pidió más aclaraciones sobre mi solicitud ya que no era lo suficientemente clara.

### Nivel 2: La IA asumió un rol técnico así como el de un interrogador ya que no sabía qué tipo de programa necesitaba.

### Nivel 3: Después de darle a la IA el contexto necesario creó el programa pero desarrolló sus atributos y métodos por su propia iniciativa.

### Nivel 4: El código generado ya tenía todos los atributos requeridos (código,nombre,precio y stock).

### Nivel 5: Ejemplos (Final):Me dio el código estructurado,introdució la clase y luego mostró el código de acuerdo al formato de los métodos que necesitaba.