# Lab Pandoc

> Configure a docker image for pandoc. 


## Pandoc with Latex

```bash
docker pull pandoc/latex
```

### Running Pandoc/Latex Container

```bash
docker run --rm \
       --volume "$(pwd):/data" \
       --user $(id -u):$(id -g) \
       pandoc/latex readme.md -o outfile.pdf
```

```bash
alias pandock=\
       'docker run --rm -v "$(pwd):/data" -u $(id -u):$(id -g) pandoc/latex'      
```
