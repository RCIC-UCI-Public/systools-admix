# systools-admix

## create pip link on Rocky 7/8

There is no default pip on fresh system install.
Need to create a link to point to default python.

```bash
update-alternatives --install /usr/bin/pip pip /usr/bin/pip3 1
```

## For container build

If making builds on a singularity container need to use bindfs for bind mount.

1. need fuse module loaded on the physical host where container is running
2. start singularity with **--bind=/dev/fuse:/dev/fuse** to get the fuse device mapped into the container
