---
author: Brayan Diaz C
pubDatetime: 2023-06-15T15:22:00Z
title: Instalación de Ruby en Ubuntu usando rbenv 🚀
postSlug: instalacion-configuracion-ruby-ubuntu-rbenv
featured: false
draft: false
tags:
  - WSL
  - Ubuntu
  - instalación
  - configuración
  - desarrollo
  - programación
ogImage: ""
description: Instala Ruby en tu sistema Ubuntu utilizando rbenv. Esta guía te mostrará los pasos necesarios para configurar rbenv y obtener la versión deseada de Ruby.
---

# Instalación de Ruby en Ubuntu usando rbenv 🚀

Aprende cómo instalar Ruby en tu sistema Ubuntu utilizando rbenv. Esta guía te mostrará los pasos necesarios para configurar rbenv y obtener la versión deseada de Ruby.

## Table of Contents

## Paso 1: Instalar dependencias

Antes de comenzar, asegúrate de tener las dependencias necesarias instaladas en tu sistema. El siguiente comando instalará varias bibliotecas y paquetes requeridos para compilar Ruby y sus gemas:

```bash
sudo apt install git-core build-essential curl wget openssl libssl-dev libreadline-dev dirmngr zlib1g-dev libmagickwand-dev imagemagick-6.q16 libffi-dev libpq-dev cmake libwebp-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev software-properties-common libcurl4-openssl-dev
```

## Paso 2: Instalar rbenv

rbenv es una herramienta que te permite instalar y manejar múltiples versiones de Ruby en tu sistema. Clona el repositorio de rbenv ejecutando el siguiente comando:

```bash
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
```

## Paso 3: Configurar rbenv

Configura rbenv agregando las siguientes líneas al archivo `~/.bashrc`. Estas líneas añaden rbenv al PATH de tu shell y habilitan la inicialización automática de rbenv cuando abras una nueva terminal:

```bash
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
source ~/.bashrc
```

## Paso 4: Instalar ruby-build

ruby-build es un plugin para rbenv que te permite instalar diferentes versiones de Ruby. Clona el repositorio de ruby-build dentro del directorio de rbenv ejecutando el siguiente comando:

```bash
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
```

## Paso 5: Configurar ruby-build

Configura ruby-build agregando la siguiente línea al archivo `~/.bashrc`. Esto añade ruby-build al PATH de tu shell:

```bash
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Paso 6: Verificar versiones disponibles de Ruby

Antes de instalar una versión específica de Ruby, puedes verificar las versiones disponibles ejecutando el siguiente comando:

```bash
rbenv install --list-all
```

Puedes verificar las versiones estables de Ruby ejecutando el siguiente comando:

```bash
rbenv install --list
```

## Paso 7: Instalar una versión de Ruby

Elige una versión de Ruby e instálala. Reemplaza `3.2.2` en el siguiente comando con la versión deseada:

```bash
rbenv install 3.2.2
```

## Paso 8: Establecer la versión global de Ruby

Establece la versión de Ruby recién instalada como la versión global. Esto significa que será la versión utilizada por defecto en tu sistema. Ejecuta el siguiente comando:

```bash
rbenv global 3.2.2
```

## Paso 9: Verificar la versión de Ruby

Verifica que la instalación de Ruby se haya realizado correctamente ejecutando el siguiente comando:

```bash
ruby -v
```

## Paso 10: Instalar Bundler

Bundler es una herramienta de manejo de gemas en Ruby. Facilita la gestión de dependencias en tus proyectos. Para instalar Bundler, ejecuta el siguiente comando:

```bash
gem install bundler
```

## Paso 11: Configurar Bundler para GitHub

Configura Bundler para que utilice HTTPS al clonar repositorios de GitHub. Esto ayuda a resolver problemas de conexión en entornos con firewalls restrictivos. Ejecuta el siguiente comando:

```bash
bundle config github.https true
```

¡Felicidades! Has instalado y configurado Ruby en tu sistema Ubuntu utilizando rbenv. Ahora puedes comenzar a desarrollar proyectos con Ruby.

Recuerda que puedes personalizar la versión de Ruby que deseas instalar y utilizar Bundler para administrar las dependencias de tus proyectos Ruby.

## Información adicional

- rbenv te permite tener múltiples versiones de Ruby en tu sistema y seleccionar la versión activa según tus necesidades.
- Ruby-build es un complemento de rbenv que facilita la instalación de diferentes versiones de Ruby.
- Bundler es una herramienta fundamental para administrar dependencias en proyectos Ruby.
- Puedes explorar más sobre Ruby y rbenv para aprovechar al máximo su potencial en el desarrollo de aplicaciones y proyectos.
