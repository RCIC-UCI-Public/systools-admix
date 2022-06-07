# systools-admix

## create pip link

There is no default pip on fresh system install.
Need to create a link to point to default python.

```bash
update-alternatives --install /usr/bin/pip pip /usr/bin/pip3 1
```
