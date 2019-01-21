gomod
=====

[![GoDoc](https://godoc.org/github.com/mxk/go-gomod?status.svg)](https://godoc.org/github.com/mxk/go-gomod)
[![Report card](https://goreportcard.com/badge/github.com/mxk/go-gomod)](https://goreportcard.com/report/github.com/mxk/go-gomod)

Package gomod provides information about modules compiled into the binary.

```
go get github.com/mxk/go-gomod
```

The implementation requires access to `runtime` package internals via `unsafe`
to locate the file table and parse module information from compiled file paths.
Module names extracted from file paths may not match actual package names.
