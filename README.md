# 7zip extraction tool built into Docker

# Summary

- A Docker build for [7zip](http://www.7-zip.org/)

# Requirements

- Docker :whale: - if you are on Mac, checkout the [Docker Toolbox](http://docs.docker.com/mac/step_one/)

# To build the Docker image

- Build the image using docker
```bash
$ docker build -t 7z-docker .
```
- Run the 7z container, mounting a local directory to extract or create archives
```bash
$ docker run -v $(pwd):/root/ --rm 7z-docker 7z x archive.7z
```

# Alternatively, you can use the Docker Hub automated build

[![](https://badge.imagelayers.io/danielwhatmuff/7z-docker:latest.svg)](https://imagelayers.io/?images=danielwhatmuff/7z-docker:latest 'Get your own badge on imagelayers.io')

```bash
$ docker pull danielwhatmuff/7z-docker
```

### Contributing
File issues in GitHub to report bugs or issue a pull request to contribute.
