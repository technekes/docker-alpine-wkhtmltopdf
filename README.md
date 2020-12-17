# Alpine Wkhtmltopdf Docker Container

[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![](https://travis-ci.org/madnight/docker-alpine-wkhtmltopdf.svg)](https://travis-ci.org/madnight/docker-alpine-wkhtmltopdf)
[![](https://images.microbadger.com/badges/image/madnight/docker-alpine-wkhtmltopdf.svg)](https://microbadger.com/images/madnight/docker-alpine-wkhtmltopdf "Get your own image badge on microbadger.com")

## Usage

wkhtmltopdf with qt patches

Yes, Alpine does have a wkhtmltopdf package... but it doesn't include the qt patches ... enjoy!


```
# Docker method
docker build -t alpine-wkhtmltopdf .
docker run alpine-wkhtmltopdf google.com - > test.pdf

# Docker shortcut
docker run technekes/docker-alpine-wkhtmltopdf google.com - > test.pdf

# Mounting with a local file (e.g. test.html)
docker run --rm -v $(pwd):/data technekes/docker-alpine-wkhtmltopdf /data/test.html - > test.pdf
```

## Q&A
*Is it really the smallest html to pdf docker image on the planet?*

Yes.



