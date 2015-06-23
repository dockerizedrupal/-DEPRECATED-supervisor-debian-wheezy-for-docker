# docker-supervisor

## Build the image

    TMP="$(mktemp -d)" \
      && GIT_SSL_NO_VERIFY=true git clone https://git.beyondcloud.io/viljaste/docker-supervisor.git "${TMP}" \
      && cd "${TMP}" \
      && git checkout debian-wheezy \
      && sudo docker build -t viljaste/supervisor:debian-wheezy . \
      && cd -

## License

**MIT**
