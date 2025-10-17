# docker_labs


# Вывод history:
```
justb@Nyash-Myash:/mnt/c/Users/justb/Desktop/MOS/docker_labs/02_docker_image_lab$ docker history jbeii/image-lab:32599cf5
IMAGE          CREATED          CREATED BY                                      SIZE      COMMENT
f719cea3068b   21 minutes ago   CMD ["python" "app.py"]                         0B        buildkit.dockerfile.v0
<missing>      21 minutes ago   HEALTHCHECK &{["CMD-SHELL" "curl -f http://l…   0B        buildkit.dockerfile.v0
<missing>      21 minutes ago   ENV ROCKET_SIZE=Medium                          0B        buildkit.dockerfile.v0
<missing>      21 minutes ago   USER appuser                                    0B        buildkit.dockerfile.v0
<missing>      21 minutes ago   COPY --chown=appuser:appuser app/ ./ # build…   12.3kB    buildkit.dockerfile.v0
<missing>      21 minutes ago   RUN |2 LAB_LOGIN=jbeii LAB_TOKEN=32599cf5be3…   16.4kB    buildkit.dockerfile.v0
<missing>      21 minutes ago   COPY /usr/local/bin/python /usr/local/bin/py…   4.1kB     buildkit.dockerfile.v0
<missing>      21 minutes ago   COPY /usr/local/bin/python3 /usr/local/bin/p…   4.1kB     buildkit.dockerfile.v0
<missing>      21 minutes ago   COPY /usr/local/bin/python3.12 /usr/local/bi…   4.1kB     buildkit.dockerfile.v0
<missing>      21 minutes ago   COPY /usr/local/lib/python3.12/site-packages…   11.9MB    buildkit.dockerfile.v0
<missing>      22 minutes ago   WORKDIR /app                                    4.1kB     buildkit.dockerfile.v0
<missing>      22 minutes ago   RUN |2 LAB_LOGIN=jbeii LAB_TOKEN=32599cf5be3…   20.5kB    buildkit.dockerfile.v0
<missing>      22 minutes ago   RUN |2 LAB_LOGIN=jbeii LAB_TOKEN=32599cf5be3…   41kB      buildkit.dockerfile.v0
<missing>      22 minutes ago   LABEL org.lab.token=32599cf5be3f579b90429f9d…   0B        buildkit.dockerfile.v0
<missing>      22 minutes ago   LABEL org.lab.login=jbeii                       0B        buildkit.dockerfile.v0
<missing>      22 minutes ago   ARG LAB_TOKEN=32599cf5be3f579b90429f9de7f998…   0B        buildkit.dockerfile.v0
<missing>      22 minutes ago   ARG LAB_LOGIN=jbeii                             0B        buildkit.dockerfile.v0
<missing>      22 minutes ago   RUN /bin/sh -c apk add --no-cache curl # bui…   5.31MB    buildkit.dockerfile.v0
<missing>      3 days ago       CMD ["python3"]                                 0B        buildkit.dockerfile.v0
<missing>      3 days ago       RUN /bin/sh -c set -eux;  for src in idle3 p…   16.4kB    buildkit.dockerfile.v0
<missing>      3 days ago       RUN /bin/sh -c set -eux;   apk add --no-cach…   44MB      buildkit.dockerfile.v0
<missing>      3 days ago       ENV PYTHON_SHA256=fb85a13414b028c49ba18bbd52…   0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV PYTHON_VERSION=3.12.12                      0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV GPG_KEY=7169605F62C751356D054A26A821E680…   0B        buildkit.dockerfile.v0
<missing>      3 days ago       RUN /bin/sh -c set -eux;  apk add --no-cache…   3.02MB    buildkit.dockerfile.v0
<missing>      3 days ago       ENV LANG=C.UTF-8                                0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV PATH=/usr/local/bin:/usr/local/sbin:/usr…   0B        buildkit.dockerfile.v0
<missing>      4 days ago       CMD ["/bin/sh"]                                 0B        buildkit.dockerfile.v0
<missing>      4 days ago       ADD alpine-minirootfs-3.22.2-x86_64.tar.gz /…   8.99MB    buildkit.dockerfile.v0
```