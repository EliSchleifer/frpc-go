# fRPC-go

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Tests](https://github.com/loopholelabs/frpc-go/actions/workflows/tests.yml/badge.svg)](https://github.com/loopholelabs/frpc-go/actions/workflows/tests.yml)

This is the [Go](http://golang.org) implementation of [fRPC](https://frpc.io), a high-performance RPC framework for 
designed for performance and stability, and it uses [frisbee-go](https://github.com/loopholelabs/frisbee) messaging framework under the hood.

**This library requires Go1.18 or later.**

## Important note about releases and stability

This repository generally follows [Semantic Versioning](https://semver.org/). However, **this library is currently in
Beta** and is still considered experimental. Breaking changes of the library will _not_ trigger a new major release. The
same is true for selected other new features explicitly marked as
**EXPERIMENTAL** in CHANGELOG.md.

## Usage and Documentation

Usage instructions and documentation for fRPC is available at [https://frpc.io/](https://frpc.io/).

The fRPC Generator is still in very early **Alpha**. While it is functional and being used within other products
we're building at [Loophole Labs][loophomepage], the `proto3` spec has a myriad of edge-cases that make it difficult to
guarantee validity of generated RPC frameworks without extensive real-world use.

That being said, as the library matures and usage of fRPC grows we'll be able to increase our testing
coverage and fix any edge case bugs. One of the major benefits to the RPC framework is that reading the generated code
is extremely straight forward, making it easy to debug potential issues down the line.

### Unsupported Features

The Frisbee RPC Generator currently does not support the following features, though they are actively being worked on:

- `OneOf` Message Types
- Streaming Messages between the client and server

Example `Proto3` files can be found [here](/examples).

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/loopholelabs/frpc-go][gitrepo]. For more
contribution information check
out [the contribution guide](https://github.com/loopholelabs/frpc-go/blob/master/CONTRIBUTING.md).

## License

The Frisbee project is available as open source under the terms of
the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

## Code of Conduct

Everyone interacting in the Frisbee project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [CNCF Code of Conduct](https://github.com/cncf/foundation/blob/master/code-of-conduct.md).

## Project Managed By:

[![https://loopholelabs.io][loopholelabs]](https://loopholelabs.io)

[gitrepo]: https://github.com/loopholelabs/frpc-go
[loopholelabs]: https://cdn.loopholelabs.io/loopholelabs/LoopholeLabsLogo.svg
[loophomepage]: https://loopholelabs.io