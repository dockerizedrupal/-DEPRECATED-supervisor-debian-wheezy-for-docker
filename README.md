# docker-supervisor-debian-wheezy

## Build the image

    TMP="$(mktemp -d)" \
      && git clone https://github.com/dockerizedrupal/docker-supervisor-debian-wheezy.git "${TMP}" \
      && cd "${TMP}" \
      && git checkout 1.0.1 \
      && sudo docker build -t dockerizedrupal/supervisor-debian-wheezy:1.0.1 . \
      && cd -

## License

**MIT**
