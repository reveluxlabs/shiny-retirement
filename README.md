Dockerized Shiny App
=======================

This is a Dockerized Shiny App Retirement : simulating wealth with random returns, inflation and withdrawals.

This shiny app is based on [one](https://systematicinvestor.wordpress.com/2012/08/14/adaptive-asset-allocation/) described by Mark Kapler on the Systematic Investor blog.

## UI

![Retirement UI](https://github.com/reveluxlabs/shiny-retirement/blob/master/retirement_ui.png "Retirement UI")


## Usage:

To run this Shiny App on your computer:

```sh
docker run --rm -p 80:80 reveluxlabs/shiny-retirement
```

and it will avaliable at http://127.0.0.1/ or http://localhost

## Building your own Shiny App:

After developing your Shiny App, you will need two files for deployment: ui.R and server.R. Then:

* Remove all files from folder app (these files are from Retirement example) and put your files there, ui.R and server.R
* Build a docker image with:

docker build -t yourname/yourappname .
```


