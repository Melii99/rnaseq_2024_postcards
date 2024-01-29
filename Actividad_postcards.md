Postcards
================

rnaseq_LCG-UNAM_2024

Curso introductorio de RNA-seq para LCG-UNAM Feb 2024

Actividad postcards

30/01/2024

## Create Beautiful, Simple Personal Websites

A collection of R Markdown templates for creating simple and easy to
personalize single page websites.

“El objetivo del paquete es facilitar que cualquier persona pueda crear
un sitio web personal de una sola página con un documento R Markdown.”

- Autor: Sean Kross \[aut, cre\]

- Maintainer: Sean Kross \<sean at seankross.com\>

- [Page:
  https://CRAN.R-project.org/package=postcards](https://CRAN.R-project.org/package=postcards)

- [GitHub:
  https://github.com/seankross/postcards](https://github.com/seankross/postcards)

## Instalación

``` r
## Puedes instalar Postcards con el siguiente comando:
install.packages("postcards")

## O puedes instalar la última versión en desarrollo:
remotes::install_github("seankross/postcards@main")
```

## Plantillas

Postcards incluye cinco plantillas: Jolla, Jolla Blue, Trestles, Onofre
y Solana. Cada sitio está optimizado para ser visualizado tanto en
computadoras de escritorio como en dispositivos móviles. El objetivo del
paquete es facilitar que cualquier persona pueda crear un sitio web
personal de una sola página con un documento R Markdown

Para comenzar a personalizar una de estas plantillas, debes crear un
nuevo proyecto.

## Crear un nuevo proyecto en RStudio (selección interactiva)

Si usas RStudio:

- selecciona “File”, “New Project”…
- Elige “New Directory”, “Postcards Website”
- Ingresar un nombre de directorio para tu proyecto en RStudio
  (“Tu_Usuario.github.io”)
- Elegir una de las plantillas desde un menú desplegable

Selecciona “Create Project” después de elegir un nombre para la carpeta
que contendrá tu sitio. Esta carpeta contendrá dos archivos importantes:

- Un documento R Markdown con el contenido de tu sitio
- Una foto de muestra que debes reemplazar”

## Crear un nuevo proyecto

``` r
## Crearun nuevo proyecto 
usethis::create_project("Su_Usuario.github.io")
```

## Configurar Git y GitHub

Para poder guardar los cambios es necesario configurar Git y GitHub

``` r
## Configurar Git y GitHub
usethis::use_git() # Reiniciar la sesión
usethis::use_github()
```

## Elegir un templado

``` r
## Elegir solo un template (el que más te guste)
postcards::create_postcard(template = "jolla")
postcards::create_postcard(template = "jolla-blue")
postcards::create_postcard(template = "trestles")
postcards::create_postcard(template = "onofre")
```

De esta manera también se obtienen los 2 archivos importantes: - Un
documento R Markdown con el contenido de tu sitio - Una foto de muestra
que debes reemplazar”

## Editar con su información

Ahora deberán editar el documento R Markdown con su información y
reemplazar la imágen con la que elijan :)

## Desplegar la página GitHub

Para compilar el archivo HTML autocontenido para el sitio:

- En RStudio puedes utilizar el botón “Knit”

o directamente:

``` r
## Desplegar la página GitHub
rmarkdown::render("index.Rmd")
```