# pumpio-snap
Snapcraft packaging for the pump.io social streaming software

To build the snap:
```
$ snapcraft
```

To install:
```
snap install pumpio-ssweeny_*_amd64.snap --dangrous
```

You can then access your pump.io instance at `http://localhost:31337`.

You'll probably want to drop a config file at `/var/snap/pumpio-ssweeny/current/pump.io.json` (see [here](https://github.com/pump-io/pump.io#configuration) for what it should contain) and restart your instance with
```
$ snap disable pumpio-ssweeny
$ snap enable pumpio-ssweeny
```
