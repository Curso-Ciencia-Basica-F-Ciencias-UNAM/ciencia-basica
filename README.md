# Ciencia Básica

Este repositorio aloja el código de la página del curso Ciencia Básica. Esta página usa [hugo](https://gohugo.io/) y el tema [hugo-book](https://github.com/alex-shpak/hugo-book).

## Requisitos

Instalar hugo:

``` 
sudo apt install hugo
```

## Crear contenido

Por ejemplo para crear un template (usando el arquetipo `práctica.md`) para la "Práctica 9" usar:

```
hugo new prácticas/práctica-09.md
```

## Desplegar a github pages

1. Borrar carpeta `/public`: `rm -fr /public`
2. Crear carpeta `/public`: `hugo`
3. Subir cambios a repo en Github. La actualización de la página se hace [automáticamente con Github Actions](https://gohugo.io/hosting-and-deployment/hosting-on-github/).
