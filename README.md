> idea come from https://github.com/lizrice/containers-from-scratch

# how to run

```bash

mkdir rootfs

docker export $(docker create ubuntu) | tar -C rootfs -xvf -

go run main.go run /bin/bash

```