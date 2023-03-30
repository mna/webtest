# webtest

[![Go Reference](https://pkg.go.dev/badge/github.com/mna/webtest.svg)](https://pkg.go.dev/github.com/mna/webtest)

This package contains a testing DSL extracted from [the website code that powers
go.dev][xwebsite].

That package is internal. This copy has been slightly cleaned up and tagged for
public consumption. It is distributed under the same license.

(The idea for this comes from https://github.com/rogpeppe/go-internal.)

This fork of https://github.com/cespare/webtest expands on the original `webtest` package in the following ways:

* Support for `PUT`, `PATCH` and `DELETE` HTTP methods (in addition to `GET`, `HEAD` and `POST`)
* Support for the `reqcookie` verb to set a cookie on the request
* Support for the `cookie` and `rawcookie` verbs to assert a cookie's value on the HTTP response
* Support for end-to-end testing, serving the handler with an HTTP server and executing requests with a client
* Better test coverage

[xwebsite]: https://pkg.go.dev/golang.org/x/website/internal/webtest
