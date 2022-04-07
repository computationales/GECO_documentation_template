# bgtemplate <a href=''><img src='https://raw.githubusercontent.com/computationales/CES_template/main/ces_logo.png' align="right" height="134.5" /></a>

CES_template provides a custom pkgdown template for CES
packages. Please don’t use it for your own package. This theme was
inspired by inspired by [tidytemplate](https://github.com/tidyverse/tidytemplate/),
[rotemplate](https://github.com/ropensci-org/rotemplate/) and [bgtemplate](https://github.com/khufkens/bgtemplate)

## How to use `CES_template`

Install the template as an R package
``` r
devtools::install_github("computationales/CES_template")
```

Set the package template as the override template to use when rendering
a package documentation using `pkgdown`

``` r
template <- list(package = "cestemplate")
pkgdown::build_site(devel = FALSE, override = list(template = template))
```

Everything else can be configured as usual via the `_pkgdown.yml` file
as described in the pkgdown documentation.

Alternatively, set the template in \_pkgdown.yml.

``` yaml
template:
  package: bgtemplate
```

### Mathjax

if you want to use Mathjax you’ll need to specify it in the `pkgdown`
config file like so:

``` yaml
template:
  params:
    mathjax: true
```
