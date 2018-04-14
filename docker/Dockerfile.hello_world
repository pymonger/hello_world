FROM hysds/pge-base

ARG id
ARG gid

# copy job repo
COPY . /home/ops/verdi/ops/hello_world
RUN set -ex \
 && sudo chown -R ops:ops /home/ops/verdi/ops/hello_world

# set entrypoint
USER ops
WORKDIR /home/ops
CMD ["/bin/bash", "--login"]
