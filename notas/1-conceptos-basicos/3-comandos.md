---
title: Comandos
author: Alan Yahir Juárez Rubio
type: Nota

aliases:
 - Comando
 - Alias

tags:
 - Comando
 - Alias
 - Flag
 - Argumento

creation date: 07-12-2023
last modification date: 08-12-2023
---

# Comandos

## Qué es un comando

Un **comando** en un _instrucción_ que enviamos a través de la _terminal_ hacia la _[shell](2-shells.md)_ para que el ordenador realice cierta acción. El _comando_ puede estar acompañado de _flags_, _parámetros_ y otros elementos

## Sintaxis

La sintaxis de un _comando_ puede variar según el tipo y su función, sin embargo existe una _sintaxis básica_ que todos, sino la mayoría de los comandos comparten:

```shell
Comando [flag(s)] [Argumento(s)]
```

> [!NOTE]
>
> Existen comandos que permiten escribir los _argumentos_ antes que los _flags_

1. **Nombre del comando:** La primera parte de un comando es el _nombre del comando_ a ejecutar
2. **Flags (opciones):** Puedes incluir _flags_ para modificar el comportamiento del comando
	1. **Cortas:** Letra de la _flag_. Le precede un guión medio `-`. Puedes incluir varias flags juntando las letras. p. ej: `ls -a -l` = `ls -al
	2. **Largas:** Nombre descriptivo de la _flag_. Le precede dos guiones medios `--`. P. ej: `ls --all --long`
3. **Argumento:** Dato de entrada sobre los que actúa el comando

> [!EXAMPLE]-
>
> > [!WARNING]
> >
> > Comando para remover/eliminar permanentemente la carpeta `archivos` en el directorio actual de manera recursiva (`-r` flag) e interactiva (`-i` flag), es decir, navegará por toda la carpeta y por cada archivo te preguntará si quieres removerlo (y/n).
> >
> > ```shell
> > rm -ri archivos
> > ```


## Tipos de comandos

> [!NOTE]
>
> El comando `type` recibe como parámetro el _nombre del comando_ y devuelve información sobre el comando para determinar de qué tipo es.

- **Programa ejecutable:** Un archivo binario generado al compilar un código, capaz de ser ejecutado.

> [!EXAMPLE]-
>
> ```bash
> type mkdir
> ```
>
> Este comando devuelve la ruta del _ejecutable_ asociado al comando `mkdir`.
>
> ```shell
> mkdir is /usr/bin/mkdir
> ```

- **Comando de utilidad del shell:** Una función o comando predeterminado que está integrado en la _shell_.

> [!EXAMPLE]-
>
> ```bash
> type cd
> ```
>
> Este comando devuelve el tipo de comando `cd`, indicando que es una utilidad integrada en la _shell_.
>
> ```shell
> cd is a shell builtin
> ```

- **Función de shell:** Una función o comando que no es parte predeterminada de la _shell_, pero que puede ser definido y utilizado.

> [!EXAMPLE]-
>
> Suponiendo que has creado la siguiente función:
>
> ```bash
> function myfunc() {
> 	echo "Hola, soy una función de shell."
> }
>
> type myfunc
> ```
>
> La salida sería:
>
> ```shell
> myfunc is a function
> myfunc ()
> {
> 	echo "Hola, soy una función de shell."
> }
> ```

- **Alias:** Un comando que, al ser creado, establece un nombre alternativo para un comando existente. Esencialmente, crea un sinónimo para el comando original.

> [!EXAMPLE]-
>
> ```bash
> type ll
> ```
>
> Este comando devuelve información sobre el alias `ll`, mostrando que está asociado al comando `ls -al`.
>
> ```shell
> ll is aliased to 'ls -al'
> ```

## Cómo crear un alias

Existen dos tipos de alias:

- **Temporal:** Solo funciona en la sesión de la terminal que fue creada
- **Permanente:** Funcionará en todo momento

### Alias Temporales

La sintaxis para crear un alias es la siguiente

```shell
alias [nombre-del-alias]="comando"
```

> [!EXAMPLE]-
>
> ```shell
> alias la="ls -A"
> ```

### Alias Permanentes

> [!NOTE]
>
> Utilizaré la _shell_ `bash` como ejemplo, sin embargo estas instrucciones también funcionan para `zsh` (remplazar `bash` por `zsh`).

En el directorio `home` encontrarás los archivos de configuración de `bash`, ahí encontrarás un archivo llamado `.bashrc`

1. Abrir el archivo `.bashrc` en tu editor de texto favorito.
2. Escribir en una línea en blanco la misma sintaxis para crear un _alias_ en la terminal, pero con comillas simples en vez de dobles.

> [!EXAMPLE]-
> ```shell
> alias ll='ls -l'
> ```

3. Guarda el archivo y reinicia tu terminal o ejecuta el comando `bash` para aplicar los cambios.

<div style="page-break-after: always;"></div>

## Referencias

- Trailhead (s. f.). _Explore la estructura de comandos y la navegación_. Consultado el 07 de diciembre de 2023 de https://trailhead.salesforce.com/es-MX/content/learn/modules/cli-basics/cli-2

- UofABioinformaticsHub (s. f.). _Linux Command Structure_. Consultado el 07 de diciembre de 2023 de https://uofabioinformaticshub.github.io/BASH-Intro/notes/extra_command_syntax.html

- Devars E. (s. f.). _Cómo configurar variables de entorno_. Consultado el 07 de diciembre de 2023 de https://platzi.com/new-home/clases/2292-terminal/37350-variables-de-entorno/