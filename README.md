# go-datamuse

[![Build Status](https://travis-ci.org/kostaspt/go-datamuse.svg?branch=master)](https://travis-ci.org/kostaspt/go-datamuse)
[![Coverage Status](https://coveralls.io/repos/github/kostaspt/go-datamuse/badge.svg?branch=master)](https://coveralls.io/github/kostaspt/go-datamuse?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/kostaspt/go-datamuse)](https://goreportcard.com/report/github.com/kostaspt/go-datamuse)

A [Go(lang)](https://golang.org/) library for the [Datamuse API](https://www.datamuse.com/api/).

## Installation

```
$ go get github.com/kostaspt/go-datamuse
```

## Example

```go
package main

import "github.com/kostaspt/go-datamuse/datamuse"

func main() {
	dm := datamuse.New()

	results, _ := dm.Words().MeansLike("ringing in the ears").Get()
    // Results: [{Word:tinnitus Score:51691 SyllablesCount:0 Tags:[syn n]} ...]
}
```

See this [test](https://github.com/kostaspt/go-datamuse/blob/master/datamuse/examples_test.go) for more examples.