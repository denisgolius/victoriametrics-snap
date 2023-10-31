### Snap integration

<https://snapcraft.io/>

snap link: <https://snapcraft.io/vmauth>

#### develop

Install snapcraft or docker

build snap package with command

```console
make build-snap
```

It produces snap package with current git version - `vmauth_v1.94.0+git1.1bebd021a-dirty_all.snap`.
You can install it with command: `snap install vmauth_v1.94.0+git1.1bebd021a-dirty_all.snap --dangerous`

#### usage

installation and configuration:

```console
# install
snap install vmauth
# logs
snap logs vmauth
# restart
snap restart vmauth
```

**Auth config**

See https://docs.victoriametrics.com/vmauth.html#auth-config

`/path/to/vmauth -auth.config=/path/to/auth/config.yml`

For advanced usage see https://docs.victoriametrics.com/vmauth.html#advanced-usage