### Snap integration

<https://snapcraft.io/>

snap link: <https://snapcraft.io/vmagent>

#### develop

Install snapcraft or docker

build snap package with command

```console
make build-snap
```

It produces snap package with current git version - `vmrestore_v1.94.0+git1.1bebd021a-dirty_all.snap`.
You can install it with command: `snap install vmrestore_v1.94.0+git1.1bebd021a-dirty_all.snap --dangerous`

#### usage

installation and configuration:

```console
# install
snap install vmrestore
# logs
snap logs vmrestore

```

Configuration management:

```console
./vmrestore -src=<storageType>://<path/to/backup> -storageDataPath=<local/path/to/restore>
```

[Advanced usage](https://docs.victoriametrics.com/vmrestore.html#advanced-usage)
[Troubleshooting](https://docs.victoriametrics.com/vmrestore.html#advanced-usage)