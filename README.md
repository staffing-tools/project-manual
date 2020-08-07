# Project Manual

Generates the project manual, a document defining the scope of the project.

# How to generate the manual

## Requirements

* [The Meson Build system](https://github.com/mesonbuild/meson)
* [rubygems](https://github.com/rubygems/rubygems)
* [asciidoctor](https://github.com/asciidoctor/asciidoctor)
* [asciidoctor-pdf](https://github.com/asciidoctor/asciidoctor-pdf)

## Command Line

```shell
git clone https://github.com/staffing-tools/project-manual
cd project-manual/src
meson builddir
cd builddir
meson compile
```