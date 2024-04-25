### Snap integration

<https://snapcraft.io/>

snap link: <https://snapcraft.io/vmaalert-tool>

#### develop

Install snapcraft or docker

build snap package with command

 ```console
make build-snap
```
#### usage

installation and configuration:

```console
 # install
 snap install vmalert-tool

 # logs
 snap logs vmalert-tool

 # restart
 snap restart vmctl
```

Configuration management:

See more https://docs.victoriametrics.com/vmalert-tool/

To see the full list of supported modes run the following command:

```console
./vmctl --help
NAME:
   vmctl - VictoriaMetrics command-line tool

USAGE:
   vmctl [global options] command [command options] [arguments...]

COMMANDS:
   opentsdb    Migrate timeseries from OpenTSDB
   influx      Migrate timeseries from InfluxDB
   prometheus  Migrate timeseries from Prometheus
   vm-native   Migrate time series between VictoriaMetrics installations via native binary format
   remote-read Migrate timeseries by Prometheus remote read protocol
   verify-block  Verifies correctness of data blocks exported via VictoriaMetrics Native format. See https://docs.victoriametrics.com/#how-to-export-data-in-native-format
```