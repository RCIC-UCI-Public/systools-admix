# systools-admix
System tools.

## For container build

If making builds on a singularity container need to use bindfs for bind mount.

1. need fuse module loaded on the physical host where container is running
2. start singularity with **--bind=/dev/fuse:/dev/fuse** to get the fuse device mapped into the container
