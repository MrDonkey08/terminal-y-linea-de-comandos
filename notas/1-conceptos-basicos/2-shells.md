---
title: Shell
author: Alan Yahir Juárez Rubio
type: Nota

aliases:
 - Shell
 - Línea de Comandos

tags:
 - Terminal
 - Comandos
 - Shell
 - CLI
 - Consola
 - PowerShell
 - CMD
 - Bash
 - Zsh

creation date: 04-12-2023
last modification date: 08-12-2023
---

# Shell

Las _shells_ son el medio de comunicación entre el usuario y el computador. Mientras que la **[terminal](1-terminal-y-linea-de-comandos.md)** es el programa que permite introducir comandos, la **shell** es la encargada de convertir los comandos en instrucciones con las que el computador pueda trabajar y, en base a ello, recibe una salida la cual manda como respuesta a la _terminal_

## Windows

### Predeterminadas

- **CMD (Command Prompt) o Símbolo del Sistema:** CMD es el terminal predeterminado en versiones antiguas de Windows. Aunque ha sido superado en funcionalidad por PowerShell, todavía está presente por razones de compatibilidad.

- **PowerShell:** El shell más avanzado y potente en el entorno Windows. Proporciona capacidades de scripting y administración del sistema más amplias que CMD. Es compatible con todos, sino la mayoría de los comandos de **CMD**. Además, **PowerShell** admite ciertos comandos de **Bash**.

> [!NOTE]- Versiones de PowerShell
>
> - **_Windows PowerShell_ (Powershell 5.1):** Versión que viene instalada por defecto en _Windows 10_ y _Windows 11_ debido a su estabilidad.
>
> - **PowerShell Core (PowerShell 6.0):** Diseñado para ser compatible con Windows, Linux y macOS. Continuó evolucionando, y la última versión estable es PowerShell 7.x, que es compatible con múltiples plataformas.
>
> - **PowerShell (PowerShell 7.0 y posteriores):** A partir de la versión 7.0, Microsoft cambió el nombre de PowerShell Core a simplemente PowerShell para reflejar la compatibilidad y la igualdad de características en todas las plataformas.

> [!IMPORTANT]
>
> Debido a las deficiencias de CMD, Microsoft convirtió a **PowerShell** en su terminal predeterminado en Windows. A pesar de esto, Microsoft no ha removido **CMD** de Windows ya que diversos programas antiguos dependen de él para su correcto funcionamiento. No obstante, se recomienda utilizar **PowerShell** en lugar de **CMD** siempre que sea posible.

### Alternativas

- **WSL (Windows Subsystem for Linux):** No es un shell por sí mismo, pero proporciona acceso a varios shells de Linux, como Bash, dentro de un entorno Windows.

- **Git Bash:** Proporciona una interfaz de línea de comandos para Git, y también incluye un entorno Bash que permite ejecutar comandos Bash y utilizar herramientas de Unix en Windows.

- **Cygwin:** Proporciona un entorno similar al de Unix en Windows, incluyendo un shell Bash.

- **Fish Shell:** Es un shell que se centra en la facilidad de uso y la interactividad.

<div style="page-break-after: always;"></div>

## Linux y macOS

### Predeterminadas

- **BASH (Bourne Again Shell):** BASH es el shell predeterminado en muchos sistemas Unix, incluyendo Linux y macOS. Ofrece una amplia gama de características y es ampliamente utilizado.

- **Zsh (Z shell):** Zsh es otro shell popular que mejora y amplía las características de BASH. Es conocido por su potencia y flexibilidad.

### Alternativas

- **PowerShell Core:** Es una versión multiplataforma de PowerShell que se ejecuta en SO's como Windows, Linux y macOS.

- **Fish Shell:** Es un shell que se centra en la facilidad de uso y la interactividad.

- **Ksh (Korn Shell):** Ofrece características combinadas de shells como Bash y Csh. Es utilizado en algunos entornos empresariales.

- **Csh (C Shell):** Un shell que proporciona una sintaxis diferente y algunas características adicionales.

- **Tcsh:** Es una versión mejorada de Csh y se utiliza en algunos entornos, especialmente por usuarios que prefieren ciertas características adicionales, como la capacidad de autocompletar utilizando la tecla Tab.

<div style="page-break-after: always;"></div>

## Referencias


- ThioJoe (julio 25, 2020). _Windows Powershell vs Command Prompt: What's The Difference Anyway?_. Consultado el 04 de diciembre de 2023 de https://www.youtube.com/watch?v=H0gwnFV_SFs

- TioJoe (septiembre 07, 2022). _Windows PowerShell vs PowerShell Core - What Is It?_. Consultado el 04 de diciembre de 2023 de https://www.youtube.com/watch?v=PqHfuaF2EiY

- Microsoft (junio 28, 2023). _What is PowerShell?_. Consultado el 04 de diciembre de 2023 de https://learn.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7.4

- Microsoft (noviembre 06, 2023). _What is Windows PowerShell?_. Consultado el 04 de diciembre de 2023 de https://learn.microsoft.com/en-us/powershell/scripting/windows-powershell/overview?view=powershell-7.4

- DavidOchoBits (marzo 25, 2019). _Las 5 mejores shell para GNU/Linux_. Consultado el 04 de diciembre de 2023 de https://www.ochobitshacenunbyte.com/2019/03/25/las-5-mejores-shell-para-gnu-linux/

- Mcfarlin T. (mayo 01, 2018). _A Quick Guide to Shells in macOS_. Consultado el 04 de diciembre de 2023 de https://tommcfarlin.com/shells-in-macos/
