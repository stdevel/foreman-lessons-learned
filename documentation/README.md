# documentation

This folder contains the AsciiDoc-based documentation.

You can build it like this:

```command
$ cd Asciidoc
$ docker run -it --rm -v "$(pwd)":/documents/ asciidoctor/docker-asciidoctor:1.17 asciidoctor-pdf -d book \
   -a pdf-stylesdir=stylesheets/ \
   -a pdf-theme=sz \
   -a pdf-fontsdir=stylesheets/ttf/ \
   *.adoc
```

When running on Red Hat-like distributions, don't forget adding the `:Z` postfix to the volume definition: `-v "$(pwd)":/documents/:Z`.
