## Requirements

[Go](http://golang.org) 1.16 or newer.

## Installation



#### Linux/BSD/MacOSX/POSIX - Build from Source

- Install Go according to the installation instructions here:
  http://golang.org/doc/install

- Ensure Go was installed properly and is a supported version:

```bash
$ go version
$ go env GOROOT GOPATH
```

NOTE: The `GOROOT` and `GOPATH` above must not be the same path.  It is
recommended that `GOPATH` is set to a directory in your home directory such as
`~/goprojects` to avoid write permission issues.  It is also recommended to add
`$GOPATH/bin` to your `PATH` at this point.

- Run the following commands to obtain brond, all dependencies, and install it:

```bash
$ cd $GOPATH/src/github.com/bronsuite/brond
$ GO111MODULE=on go install -v . ./cmd/...
```

- brond (and utilities) will now be installed in ```$GOPATH/bin```.  If you did
  not already add the bin directory to your system path during Go installation,
  we recommend you do so now.

## Updating

#### Linux/BSD/MacOSX/POSIX - Build from Source

- Run the following commands to update brond, all dependencies, and install it:

```bash
$ cd $GOPATH/src/github.com/bronsuite/brond
$ git pull
$ GO111MODULE=on go install -v . ./cmd/...
```

## Getting Started

brond has several configuration options available to tweak how it runs, but all
of the basic operations described in the intro section work with zero
configuration.

#### Linux/BSD/POSIX/Source

```bash
$ ./brond
```

## IRC

- irc.libera.chat
- channel #btcd
- [webchat](https://web.libera.chat/gamja/?channels=btcd)

## Issue Tracker

The [integrated github issue tracker](https://github.com/bronsuite/brond/issues)
is used for this project.

## Documentation

The documentation is a work-in-progress.  It is located in the [docs](https://github.com/bronsuite/brond/tree/master/docs) folder.

## Release Verification

Please see our [documentation on the current build/verification
process](https://github.com/bronsuite/brond/tree/master/release) for all our
releases for information on how to verify the integrity of published releases
using our reproducible build system.

## License

brond is licensed under the [copyfree](http://copyfree.org) ISC License.
