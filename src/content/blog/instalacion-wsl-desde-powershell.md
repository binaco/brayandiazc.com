---
author: Brayan Diaz C
pubDatetime: 2023-06-15T12:22:00Z
title: "Instala WSL a través de PowerShell 🐧"
postSlug: instalacion-wsl-desde-powershell
featured: false
draft: false
tags:
  - Windows
  - WSL
  - Linux
  - DesarrolloSoftware
  - PowerShell
ogImage: ""
description: Aprende a instalar y usar el Subsistema de Windows para Linux (WSL) a través de PowerShell con este tutorial paso a paso.
---

# Instala WSL a través de PowerShell 🐧

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

![Verificar versión de Windows](/assets/postContent/instalacion-wsl-desde-powershell/verificar-version-windows.png)

## 1. Instalación de WSL 💾

La instalación de WSL es sencilla. Sigue estos pasos:

1. Abre PowerShell como administrador.

![Abrir PowerShell](/assets/postContent/instalacion-wsl-desde-powershell/powershell.png)

2. Ejecuta el siguiente comando:

```powershell
wsl --install
```

![Instalar WSL](/assets/postContent/instalacion-wsl-desde-powershell/instalacion-wsl.png)

3. Tu PC te pedirá que reinicies. Una vez reiniciado, WSL estará instalado.

## 2. Configuración de Linux en WSL ⚙️

Para configurar Linux en WSL, abre la aplicación Linux que instalaste y sigue las instrucciones en pantalla. Se te pedirá que ingreses un **nombre de usuario** y una **contraseña**.

![Configuración inicial ubuntu](/assets/postContent/instalacion-wsl-desde-powershell/configuracion-inicial-ubuntu.png)

## 3. Instalación de aplicaciones de Linux en Windows 📦

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

## Recursos adicionales

- [Documentación oficial de Microsoft sobre WSL](https://docs.microsoft.com/es-es/windows/wsl/)
- [Guía de instalación de WSL](https://docs.microsoft.com/es-es/windows/wsl/install-win10)
- [Guía de instalación de WSL 2](https://docs.microsoft.com/es-es/windows/wsl/install-win10#update-to-wsl-2)
