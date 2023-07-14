---
author: Brayan Diaz C
pubDatetime: 2023-06-15T11:22:00Z
title: "Instala WSL a través de Microsoft Store 🐧"
postSlug: instalacion-wsl-desde-microsoft-store
featured: false
draft: true
tags:
  - Windows
  - WSL
  - Linux
  - DesarrolloSoftware
  - MicrosoftStore
ogImage: ""
description: Aprende a instalar y usar el Subsistema de Windows para Linux (WSL) a través de la Microsoft Store con este tutorial paso a paso.
---

# Instala WSL a través de Microsoft Store 🐧

Los desarrolladores de software a menudo prefieren Linux como su sistema operativo principal. Sin embargo, si usas Windows y quieres tener acceso a un entorno Linux sin tener que recurrir a una máquina virtual o a un arranque dual, **WSL** (Windows Subsystem for Linux) es tu solución.

## Table of Contents

## ¿Qué es WSL? 🤔

WSL es una capa de compatibilidad que permite ejecutar ejecutables binarios de Linux de manera nativa en Windows 10 y Windows 11. Esto significa que puedes usar Linux directamente en Windows, sin la necesidad de cambiar de sistema operativo o arrancar una máquina virtual.

## ¿Qué puedes hacer con WSL? 💡

WSL te permite ejecutar una amplia variedad de aplicaciones de Linux en Windows, desde aplicaciones de línea de comandos como Git, Node.js, Python, hasta aplicaciones de escritorio y web como Visual Studio Code, Atom, WordPress y Django.

## Versiones de WSL 🔄

Existen dos versiones de WSL:

1. **WSL 1** - Usa una máquina virtual para ejecutar aplicaciones de Linux, pero es compatible con más versiones de Linux.
2. **WSL 2** - Usa un núcleo de Linux real, lo que lo hace más rápido que WSL 1. Sin embargo, solo es compatible con algunas versiones de Linux.

## ¿Qué versiones de Windows son compatibles con WSL? 🖥️

WSL es compatible con Windows 10 (versión 2004 o posterior) y Windows 11. Para verificar tu versión de Windows, abre la configuración de Windows, haz clic en "Sistema" y luego en "Información". En la página "Información", puedes ver la versión de Windows que tienes instalada.

![Verificar versión de Windows](/assets/postContent/instalacion-wsl-desde-microsoft-store/verificar-version-windows.png)

## 1. Instalación de WSL 💾

Para instalar WSL, sigue estos pasos:

1. Abre la **Microsoft Store** en Windows y busca "WSL". Haz clic en el primer resultado y luego en "Instalar".
2. Reinicia tu computadora después de la instalación.

![Windows store instalar wsl](/assets/postContent/instalacion-wsl-desde-microsoft-store/windows-store-instalar-wsl.png)

## 2. Instalación de Linux en WSL 🐧

Para instalar un kernel de Linux en WSL, realiza los siguientes pasos:

1. Abre la **Microsoft Store** en Windows y busca la distribución de Linux de tu preferencia, por ejemplo, "Ubuntu". Haz clic en el primer resultado y luego en "Instalar".
2. Reinicia tu computadora después de la instalación.

![Windows store instalar ubuntu](/assets/postContent/instalacion-wsl-desde-microsoft-store/windows-store-instalar-ubuntu.png)

## 3. Configuración de Linux en WSL ⚙️

Para configurar Linux en WSL, abre la aplicación Linux que instalaste y sigue las instrucciones en pantalla. Se te pedirá que ingreses un **nombre de usuario** y una **contraseña**.

![Configuración inicial ubuntu](/assets/postContent/instalacion-wsl-desde-microsoft-store/configuracion-inicial-ubuntu.png)

## 4. Instalación de aplicaciones de Linux en Windows 📦

Ahora que ya tienes WSL y Linux instalados, puedes instalar aplicaciones de Linux en Windows. Para hacerlo, abre la aplicación Linux y ejecuta los siguientes comandos para actualizar el índice de paquetes e instalar la aplicación deseada:

```shell
sudo apt update
```

```shell
sudo apt install nombre_de_la_aplicación
```

Por ejemplo, para instalar Git, ejecutarías `sudo apt install git`.

## Conclusión

Con WSL, los desarrolladores de software que utilizan Windows como su sistema operativo principal pueden disfrutar de las ventajas de ejecutar aplicaciones de Linux sin necesidad de utilizar máquinas virtuales o particiones separadas. WSL brinda la flexibilidad y la facilidad de uso necesarias para llevar a cabo tareas de desarrollo y ejecutar aplicaciones de Linux en el entorno de Windows de manera eficiente.
