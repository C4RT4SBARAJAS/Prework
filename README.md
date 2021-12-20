# Prework: Configuración de Entorno de Desarrollo en windows

La idea de este curso es que tu termines preparad@ para poder comenzar a aprender Desarrollo Web desde Cero.

Aquí vamos a configurar nuestro navegador, vamos a conocer que opciones de navegadores tenemos, también vamos a preparar nuestro editor de código, lo ideal es que aquí te estamos dejando list@ para tu camino como desarrollador@ web. Luego de esto nos vamos a pasar a ver algo super interesante que esl el Windows Subsystem for Linux, que basicamente te permite instalar un sistema operativo Linux dentro de tu Windows, que va a correr super rápido, super eficiente y eso te va a permitir ejecutar todas las herramientas de desarrollo, y no vas a tener un bloqueo para desarrollar nada, todo va a ir fluyendo. Vamos a dejar bien configurado nuestro WSL. Luego de esto hablaremos brevemente de Git y GitHub.

En caso de que tu no tengas una computadora con windows 10, no importa, pues puedes aprender a montar una maquina virtual de linux. Utilizando el sistema operativo Ubuntu.

Si no quieres usar WSL o una maquina virtual, entonces tendríamos una situación grave, porque vas a sufrir muchísimo en todo tu flujo de desarrollo, vas a tener muchísimos bloqueos, vas a perder muchísmo tiempo buscando adaptar las cosas a Windows. Yo te invito a que si eres de este último grupo que no quiere poner ni una maquina virtual o no quiere instalr el WSL, lo reconsideres, porque vas a sufrir muchísimo.

Este curso es bien importante que lo vallas haciendo paso a paso conmigo, también que sigas las instrucciones al pie de la letra.

## Editor de texto: instalando el tuyo
La mayoría de las personas hoy en día están utilizando Visual Studio Code y es el que vamos a estar utilizando en nuestros cursos, así que es el que vamos a instalar.

Visual Studio Code es un Editor de Código free, están construido encima de Open source y se ejecuta y corre en Windows, Linux o Mac. Te sirve para todo tipo de funcionalidades, para Web, para Apps moviles, para Ciencia de Datos y desarrollo de videojuegos, Visual Studio Code es muy versatil y te sirve para programar todo tipo de aplicaciones. Tiene un enfoque modular ya que puedes instalar solo lo que necesites para programar.

Para descargar el instalador haz clic [aquí](https://visualstudio.microsoft.com/es/free-developer-offers/ "aquí"). Elegimos **Visual Studio Code** > Descarga gratuita > Windows x64.

## Extensiones y personalización de Visual Studio Code
Vamos a agregar una serie de extenciones que te van a ayudar muchísimo con todo nuestro código.

1. **Abrimos** Visual Studio Code.
2. Nos dirigimos a **Extensions**.
3. Clik en **Search Extensions in ...**

Las Extenciones a instalr son las siguientes:

- Prettier - Code formatter
- Color Highlight
- Live Server
- Path Intellisense
- Auto Rename Tag
- Material Icon Theme

## ¿Qué es Windows Subsystem for Linux?
Esto es lo que Microsoft biene desarrollando para poder volver a windows 10 una plataforma competitiva para poder desarrollar. Ya que Windows no servía para desarrollo de aplicaciones web. Hoy en día con día con Windows Subsystem for Linux, todo lo puedes hacer desde una terminal de Linux dentro de tu sistema operativo windows. Esto es posible gracias a que microsoft esta desarrollando esta tecnología y esta en su versión 2. Lo que tiene es un nucleo de linux que además, combina tecnologías de virtualización que le permiten ejecutarse super rápido en windows. Con esto te quiero decir que, es de buen rendimiento y es basntante útil.

Si tu no tienes instalado windows 10, primero esfuerzate por tenerlo, vale mucho la pena. Es un gran sistema operativo y se esta volviendo una muy buena herramienta de trabajo para desarrollar.

**Para actualizar a WSL 2**, ***debe ejecutar Windows 10. Para sistemas x64: La versión 1903 o posterior, con la compilación 18362 o posterior. Para sistemas ARM64: La versión 2004 o posterior, con la compilación 19041 o posterior.***

Para comprobar la versión de mi windows 10 utilizamos el Ejecutador de tareas y escribimos el comando `winver`. Si tu no tienes esta versión lo que puedes hacer es **Buscar actualizaciones** en windows update.

## Instalación de Windows Subsystem for Linux
Ya podemos instalar WSL. ¡Hagamoslo!

1. Habilite el subsistema de Windows para Linux. Abra PowerShell como administrador (menú Inicio> PowerShell> haga clic con el botón derecho> Ejecutar como administrador) e ingrese este comando:

```shell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
