# docker-supervisor-debian-wheezy

An intermediate base Docker image for [dockerizedrupal/base-debian-wheezy](https://github.com/dockerizedrupal/docker-base-debian-wheezy).

This project is part of the [Dockerized Drupal](https://dockerizedrupal.com/) initiative.

## Run the container

    CONTAINER="supervisor" && sudo docker run \
      --name "${CONTAINER}" \
      -h "${CONTAINER}" \
      dockerizedrupal/supervisor-debian-wheezy:1.1.0

## Build the image

    TMP="$(mktemp -d)" \
      && git clone https://github.com/dockerizedrupal/docker-supervisor-debian-wheezy.git "${TMP}" \
      && cd "${TMP}" \
      && git checkout 1.1.0 \
      && sudo docker build -t dockerizedrupal/supervisor-debian-wheezy:1.1.0 . \
      && cd -

## License

**MIT**
