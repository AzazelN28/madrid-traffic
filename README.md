# Madrid Traffic

## Instalar Docker

[Docker](https://www.docker.com/) es una plataforma abierta para desarrolladores y
sysadmins para construir, entregar y ejecutar aplicaciones distribuidas, ya sea en
portátiles, centros de datos o la nube.

Madrid Traffic hace uso tanto de `docker` como de `docker-compose`.

Docker está disponible tanto para [Linux](https://docs.docker.com/engine/installation/linux) como para [Windows](https://docs.docker.com/docker-for-windows/) o [Mac](https://docs.docker.com/docker-for-mac/) (Madrid Traffic
sólo se ha probado en versiones Linux y Mac de Docker).

Para instalarlo puedes seguir los diferentes pasos en sus guías de instalación:

- [Guía de instalación para Linux](https://docs.docker.com/engine/installation/linux)
- [Guía de instalación para Mac](https://docs.docker.com/docker-for-mac/)
- [Guía de instalación para Windows](https://docs.docker.com/docker-for-windows/)

## Arrancar el entorno en Mac o Linux

Primero clona este repositorio usando git:

```sh
git clone https://github.com/rojo2/madrid-traffic.git
```

Una vez clonado el repositorio, podrás descargarte el resto del entorno a través del comando:

```sh
git submodule update --init --recursive
```

Cuando estén todos los submodulos descargados entonces podemos arrancar el entorno usando `docker-compose`:

```sh
cd docker && docker-compose up
```

Para la gente con prisa, copia y pega este código y ejecútalo con un terminal (necesitarás tener Docker for Mac arrancado en caso de usarlo desde Mac)

```sh
git clone https://github.com/rojo2/madrid-traffic.git madrid-traffic
cd madrid-traffic && git submodule update --init --recursive
cd docker && docker-compose up
```

## Arrancar el entorno en Windows (con PowerShell)

Necesitarás tener instalado `git` en PowerShell para ello instala [posh-git](https://github.com/dahlbyk/posh-git), siguiendo [esta guía](https://git-scm.com/book/es/v2/Git-in-Other-Environments-Git-in-Powershell) de `git`
es fácil.

Hecho con :heart: por ROJO 2 (http://rojo2.com)
