---
author: Brayan Diaz C
pubDatetime: 2023-06-15T14:22:00Z
title: Guía de Instalación y Configuración de Git 🚀
postSlug: instalacion-configuracion-git
featured: false
draft: true
tags:
  - Git
  - Instalación
  - Configuración
  - ControlDeVersiones
  - desarrollosoftware
ogImage: ""
description: Instala y configura Git en tu sistema Ubuntu. Obten la última versión de Git y configurar tus credenciales y ajustes básicos.
---

# Guía de Instalación y Configuración de Git 🚀

Aprende cómo instalar y configurar Git en tu sistema Ubuntu. Esta guía te mostrará los pasos necesarios para obtener la última versión de Git y configurar tus credenciales y ajustes básicos.

## Table of Contents

## Paso 1: Agregar el repositorio PPA de Git

Para obtener la última versión estable de Git, agrega el repositorio PPA ejecutando el siguiente comando:

```bash
sudo add-apt-repository ppa:git-core/ppa -y
```

## Paso 2: Actualizar dependencias

Asegúrate de tener las dependencias actualizadas ejecutando el siguiente comando:

```bash
sudo apt-get update
```

## Paso 3: Instalar Git

Instala Git en tu sistema con el siguiente comando:

```bash
sudo apt-get install git -y
```

## Paso 4: Verificar la versión de Git

Confirma que Git se ha instalado correctamente verificando su versión con el siguiente comando:

```bash
git --version
```

## Paso 5: Configurar colores en los comandos de Git

Habilita el uso de colores en los comandos de Git para una mejor legibilidad ejecutando el siguiente comando:

```bash
git config --global color.ui true
```

## Paso 6: Configurar nombre de usuario

Configura tu nombre de usuario de Git con el siguiente comando:

```bash
git config --global user.name "Tu Nombre"
```

## Paso 7: Configurar dirección de correo electrónico

Configura tu dirección de correo electrónico asociada a Git con el siguiente comando:

```bash
git config --global user.email "tucorreo@example.com"
```

## Paso 8: Configurar la rama principal predeterminada

Establece la rama principal predeterminada para los nuevos repositorios con el siguiente comando:

```bash
git config --global init.defaultBranch main
```

## Paso 9: Configurar una plantilla de mensaje de commit

Crea un archivo para utilizarlo como plantilla de mensaje de commit con el siguiente comando:

```bash
git config --global commit.template ~/.gitmessage
```

## Paso 10: Generar una clave SSH

Genera una nueva clave SSH para autenticarte en servicios como GitHub y GitLab con el siguiente comando:

```bash
ssh-keygen -t rsa -b 4096 -C "tucorreo@example.com"
```

Presiona 'Enter' cuatro veces para aceptar los valores predeterminados.

## Paso 11: Agregar clave SSH a tu cuenta de GitHub

Copia el contenido de la clave SSH recién generada con el siguiente comando:

```bash
cat ~/.ssh/id_rsa.pub
```

Luego, ve a tu cuenta de GitHub y pega el contenido de la clave en la sección de [configuración de SSH](https://github.com/settings/ssh).

## Paso 12: Verificar la autenticación SSH

Verifica que la autenticación SSH esté funcionando correctamente ejecutando los siguientes comandos:

```bash
ssh -T git@github.com
```

Deberías recibir un mensaje similar a:

```
Hi excid3! You've successfully authenticated, but GitHub does not provide shell access.
```

## Conclusión

¡Felicidades! Has instalado y configurado Git en tu sistema Ubuntu. Ahora estás listo para comenzar a utilizar Git en tus proyectos. Asegúrate de personalizar los ajustes de usuario y mantener tus claves SSH seguras.

Recuerda consultar la documentación oficial de Git para obtener más información sobre cómo utilizar Git de manera efectiva en tu flujo de trabajo de desarrollo.

## Información adicional

- Git es una herramienta poderosa para el control de versiones y colaboración en proyectos de desarrollo de software.
- Puedes explorar diferentes comandos y funcionalidades de Git para aprovechar al máximo esta herramienta.
- Mantén tus claves SSH privadas y no las compartas con nadie para garantizar la seguridad de tus repositorios remotos.
