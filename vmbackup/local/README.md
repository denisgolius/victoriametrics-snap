### Snap integration

<https://snapcraft.io/>

snap link: <https://snapcraft.io/vmagent>

#### develop

Install snapcraft or docker

build snap package with command

```console
make build-snap
```

It produces snap package with current git version - `vmbackup_v1.94.0+git1.1bebd021a-dirty_all.snap`.
You can install it with command: `snap install vmbackup_v1.94.0+git1.1bebd021a-dirty_all.snap --dangerous`

#### usage

installation and configuration:

```console
# install
snap install vmbackup
# logs
snap logs vmbackup
```

Configuration management:

```console
./vmbackup -storageDataPath=</path/to/victoria-metrics-data> -snapshot.createURL=http://localhost:8428/snapshot/create -dst=gs://<bucket>/<path/to/new/backup>
```

For advanced usage see https://docs.victoriametrics.com/vmbackup.html#advanced-usage