Postcards
================

rnaseq_LCG-UNAM_2024

Curso introductorio de RNA-seq para LCG-UNAM Feb 2024

Actividad postcards

30/01/2024

### Create Beautiful, Simple Personal Websites

*A collection of R Markdown templates for creating simple and easy to
personalize single page websites.*

“El objetivo del paquete es facilitar que cualquier persona pueda crear
un sitio web personal de una sola página con un documento R Markdown.”

- Autor: Sean Kross \[aut, cre\]

- Maintainer: Sean Kross \<sean at seankross.com\>

- <https://CRAN.R-project.org/package=postcards>

- GitHub: <https://github.com/seankross/postcards>

- Similar a <https://pages.github.com/>

- Tu página web debe describir decir algo sobre ti, tus intereses, y tus
  proyectos además de cómo contactarte

  Algunos ejemplos:

  - <https://amy-peterson.github.io/> vía
    <https://github.com/amy-peterson/amy-peterson.github.com>
  - <http://jtleek.com/> vía
    <https://github.com/jtleek/jtleek.github.io>
  - <http://aejaffe.com/> vía
    <https://github.com/andrewejaffe/andrewejaffe.github.io>
  - <https://hadley.nz/> vía
    <https://github.com/hadley/hadley.github.com>
  - <https://emarquezz.github.io/> vía
    <https://github.com/emarquezz/emarquezz.github.io>
  - <https://bpardo99.github.io/> vía
    <https://github.com/bpardo99/bpardo99.github.io>
  - <https://daianna21.github.io/> vía
    <https://github.com/daianna21/daianna21.github.io>.

### Instalación

``` r
## Puedes instalar Postcards con el siguiente comando:
install.packages("postcards")

## O puedes instalar la última versión en desarrollo:
remotes::install_github("seankross/postcards@main")
```

### Plantillas

Postcards incluye cinco plantillas: Jolla, Jolla Blue, Trestles, Onofre
y Solana. Cada sitio está optimizado para ser visualizado tanto en
computadoras de escritorio como en dispositivos móviles. El objetivo del
paquete es facilitar que cualquier persona pueda crear un sitio web
personal de una sola página con un documento R Markdown

#### Jolla:

<figure>
<img
src="https://raw.githubusercontent.com/Melii99/rnaseq_2024_postcards/master/Templates/jolla_preview.png"
alt="Jolla" />
<figcaption aria-hidden="true">Jolla</figcaption>
</figure>

#### Jolla Blue:

<figure>
<img
src="https://raw.githubusercontent.com/Melii99/rnaseq_2024_postcards/master/Templates/jolla_blue_preview.png"
alt="Jolla Blue" />
<figcaption aria-hidden="true">Jolla Blue</figcaption>
</figure>

#### Trestles:

<figure>
<img
src="https://raw.githubusercontent.com/Melii99/rnaseq_2024_postcards/master/Templates/trestles-preview.png"
alt="Trestles" />
<figcaption aria-hidden="true">Trestles</figcaption>
</figure>

#### Onofre:

<figure>
<img
src="https://raw.githubusercontent.com/Melii99/rnaseq_2024_postcards/master/Templates/onofre-preview.png"
alt="Onofre" />
<figcaption aria-hidden="true">Onofre</figcaption>
</figure>

#### Solana:

<figure>
<img
src="https://raw.githubusercontent.com/Melii99/rnaseq_2024_postcards/master/Templates/solana-preview.png"
alt="Solana" />
<figcaption aria-hidden="true">Solana</figcaption>
</figure>

Para comenzar a personalizar una de estas plantillas, debes crear un
nuevo proyecto.

### Crear un nuevo proyecto en RStudio (selección interactiva)

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

### Crear un nuevo proyecto

``` r
## Crearun nuevo proyecto 
usethis::create_project("Su_Usuario.github.io")
```

### Configurar Git y GitHub

Para poder guardar los cambios es necesario configurar Git y GitHub

``` r
## Configurar Git y GitHub
usethis::use_git() # Reiniciar la sesión
usethis::use_github()
```

### Elegir una plantilla

``` r
## Elegir solo una plantilla (la que más te guste)
postcards::create_postcard(template = "jolla")
postcards::create_postcard(template = "jolla-blue")
postcards::create_postcard(template = "trestles")
postcards::create_postcard(template = "onofre")
postcards::create_postcard(template = "solana")
```

De esta manera también se obtienen los 2 archivos importantes:

- Un documento R Markdown con el contenido de tu sitio

- Una foto de muestra que debes reemplazar

### Editar con su información

- Ahora deberán editar el documento R Markdown con su información y
  reemplazar la imágen con la que elijan :)

- Llenen su información usando el formato `Markdown`. Por ejemplo
  <https://github.com/andrewejaffe/andrewejaffe.github.io/blob/master/index.Rmd#L17-L31>.

- Agreguen sus perfiles estilo
  <https://github.com/andrewejaffe/andrewejaffe.github.io/blob/master/index.Rmd#L7-L12>

### Desplegar la página

Para compilar el archivo HTML autocontenido para el sitio:

- En RStudio puedes utilizar el botón “Knit”

o directamente:

``` r
## Desplegar la página GitHub
rmarkdown::render("index.Rmd")
```
