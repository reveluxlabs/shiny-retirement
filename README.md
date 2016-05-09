Dockerized Shiny App
=======================

This is a Dockerized Shiny App Retirement : simulating wealth with random returns, inflation and withdrawals.

This Dockerfile is based on Debian "testing" and r-base image.

## Usage:

To run this Shiny App on your computer:

```sh
docker run --rm -p 80:80 reveluxlabs/shiny-retirement
```

and it will avaliable at http://127.0.0.1/ or http://localhost

```

## Building your own Shiny App:

After developing your Shiny App, you will need two files for deployment: ui.R and server.R. Then:

* Remove all files from folder app (these files are from Wordcloud example) and put your files there, ui.R and server.R
* Build a docker image with:

```sh
docker build -t yourname/yourappname .
```


