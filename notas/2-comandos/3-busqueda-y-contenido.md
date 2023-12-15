---
title: Búsqueda y Contenido
author: Alan Yahir Juárez Rubio
type: Nota

aliases:
tags:

creation date: 11-12-2023
last modification date: 14-12-2023
---

## Búsqueda

|          Comando           | Nombre | Descripción                                                                 |           Flags            |      Argumento      | Ejemplo            |
|:--------------------------:|:------:|:--------------------------------------------------------------------------- |:--------------------------:|:-------------------:| ------------------ |
|           `find`           | Buscar | Busca archivos en una jerarquía de directorios en base a una expresión dada | `-name `, `-type`, `-size` | Ruta del directorio | `find ./ -name "main.cpp"`, `find ~/Documents/ -name "" |
|    `grep <regex> file`     |        |                                                                             |       `i`, `c`, `v`        |       Archivo       |                    |
| `grep -i hola mensaje.txt` |        |                                                                             |                            |                     |                    |

<br>

| Comando | Nombre | Descripción                                                                    |  Flags   | Argumento | Ejemplo |
|:-------:|:------:|:------------------------------------------------------------------------------ |:--------:|:---------:| ------- |
| `which` |  Cuál  | Muestra la ruta del binario de un comando. Busca en todas las rutas del _path_ | `a`, `v` |  Comando  |         |
|         |        |                                                                                |          |           |         |

### Exploración de Contenido

| Comando | Descripción                                                                                          |                      Flags                       | Argumento  | Ejemplo |
|:-------:|:---------------------------------------------------------------------------------------------------- |:------------------------------------------------:|:----------:| ------- |
| `head`  | Imprime las primeras 20 líneas del archivo                                                           |                    `n <num>`                     |  Archivo   |         |
| `tails` | Imprime las últimas 20 líneas del archivo                                                            |                    `n <num>`                     |  Archivo   |         |
| `more`  | Imprime el contenido de un archivo                                                                   |        `c`, `d`, `f`, `l`, `p`, `s`, `u`         |  Archivo   |         |
| `less`  | Imprime el contenido de un archivo como `more`, pero con más funciones. Está basado en `more` y `vi` |                  `N`. `X`, `+F`                  |  Archivo   |         |
|  `cat`  | Concatena el contenido de archivos para imprimirlo                                                   | `A`, `b`, `e`, `E`, `n`, `s`, `t`, `T`, `u`, `v` | Archivo(s) |         |

<div style="page-break-after: always;"></div>

## Referencias

- https://platzi.com/new-home/clases/2292-terminal/37345-explorando-el-contenido-de-nuestros-archivos/