# malaria-orderly-image

[![Build status](https://badge.buildkite.com/a1f54f82795e6544edc97731fd72798f33b2b2eeb3fa148a7d.svg)](https://buildkite.com/mrc-ide/malaria-orderly-image)

This is the docker container for [malaria-sites-orderly](https://github.com/mrc-ide/malaria-sites-orderly).

This repo is a fork of [`montagu-orderly`](https://github.com/vimc/montagu-orderly) with minor modifications

**Interaction with the server**.  These commands interact with the orderly server on the *same host* as you run it.  If you run these on your desktop they will not affect any other machine.

Make sure you have the most recent version of the container with with

Update the `https://github.com/mrc-ide/malaria-sites-orderly` repo on the orderly volume

```
./pull_sources
```

Run orderly commands with

```
./orderly run <name>
./orderly list names
./orderly --help
```

etc.

Get a shell on the container with

```
./shell
```

## Building the image

The image is built on [Buildkite](https://buildkite.com/mrc-ide/hiv-orderly)
