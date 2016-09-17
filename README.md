# WARNING

> **Notice:** *This project is deprecated. Read more about the reason why [here](https://github.com/dockerizedrupal/base-debian-wheezy-for-docker/issues/3).*

# -DEPRECATED-supervisor-debian-wheezy-for-docker

A base Docker image for [dockerizedrupal/base-debian-wheezy](https://github.com/dockerizedrupal/base-debian-wheezy-for-docker).

## Run the container

    CONTAINER="supervisor" && sudo docker run \
      --name "${CONTAINER}" \
      -h "${CONTAINER}" \
      dockerizedrupal/supervisor-debian-wheezy:1.1.2

## Build the image

    TMP="$(mktemp -d)" \
      && git clone https://github.com/dockerizedrupal/-DEPRECATED-supervisor-debian-wheezy-for-docker.git "${TMP}" \
      && cd "${TMP}" \
      && git checkout 1.1.2 \
      && sudo docker build -t dockerizedrupal/supervisor-debian-wheezy:1.1.2 . \
      && cd -

## License

**MIT**
