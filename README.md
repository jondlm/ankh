# ankh

`ankh` is a CLI tool that helps manage larger, multi-tenant Kubernetes
clusters. It is currently under development.

## Installing

Eventually we will publish a set of pre-compiled binaries. For now it's best to
install go 1.9+ and install the source and binary with:

	go get github.com/appnexus/ankh

## Contributing

Here are the recommended steps for contributing to ankh:

	# Ensure you have go 1.9+ installed with `brew install go` on a Mac
	git clone <repo> $GOPATH/src/github.com/appnexus/ankh
	cd $GOPATH/src/github.com/appnexus/ankh
	go run ankh.go

### Dependencies

We use the [`dep`][dep] tool for dependency management and a checked in
`vendor` directory. Feel free to run `dep ensure` to update dependencies when
needed.

[dep]: https://github.com/golang/dep
