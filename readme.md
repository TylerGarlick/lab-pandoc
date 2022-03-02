# Lab Pandoc

> Configure a docker image for pandoc. 


## Pandoc with Latex

## Using Docker image

```bash 
docker pull pandoc/core
```

### Running Pandoc

```bash
docker run --rm \
       --volume "$(pwd):/data" \
       --user $(id -u):$(id -g) \
       pandoc/core README.md -o outfile.pdf
```

```bash
docker run --rm \
       --volume "$(pwd):/data" \
       --user $(id -u):$(id -g) \
       pandoc/core README.md -o outfile.pdf
```

### Notes
