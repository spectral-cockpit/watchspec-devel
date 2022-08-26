## Overview

Our aim here is to template a shiny app that can read and plot spectra whilst
measurements are being made.

## Principles

watchdog is a python module that features the following components:

- Watcher:
- Handler:

## Docker setup

We want run a dockerized shiny app. Therefore, we use `rocker/shiny:4.2` as
a base image. This image exposes port 3838.

To name, run and test the image:

```
export IMAGE="spectral-cockpit/watchspec-devel"
# build image
docker build -t $IMAGE .
docker run -p 8080:3838 $IMAGE
```

## Credits

- python pre-commit hooks are from opengis.ch public repos with MIT licencing.
