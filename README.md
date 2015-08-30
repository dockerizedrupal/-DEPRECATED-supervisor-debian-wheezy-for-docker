# docker-supervisor-debian-wheezy

## Build the image

    TMP="$(mktemp -d)" \
      && git clone https://github.com/dockerizedrupal/docker-supervisor-debian-wheezy.git "${TMP}" \
      && cd "${TMP}" \
      && sudo docker build -t dockerizedrupal/supervisor-debian-wheezy:latest . \
      && cd -

## License

**MIT**
