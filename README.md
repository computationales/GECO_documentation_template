# bgtemplate <a href=''><img src='https://bluegreenlabs.org/img/logo.png' align="right" height="134.5" /></a>

cestemplate provides a custom pkgdown template for CES
packages. Please don’t use it for your own package. This theme was
inspired by inspired by BlueGreen Labs' package theme.

## How to use `cestemplate`

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
