# GOSTSUM(2)
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/pedroalbanese/gostsum/blob/master/LICENSE.md) 
[![GoDoc](https://godoc.org/github.com/pedroalbanese/gostsum?status.png)](http://godoc.org/github.com/pedroalbanese/gostsum)
[![Go Report Card](https://goreportcard.com/badge/github.com/pedroalbanese/gostsum)](https://goreportcard.com/report/github.com/pedroalbanese/gostsum)
[![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/pedroalbanese/gostsum)](https://golang.org)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/pedroalbanese/gostsum)](https://github.com/pedroalbanese/gostsum/releases)
### GOST R 34.11-94 CryptoPro Recursive Hasher
<pre>
Usage of gostsum:
gostsum [-v] [-c &lt;hash.g94&gt;] [-r] &lt;file.ext&gt;
  -c string
        Check hashsum file
  -r    Process directories recursively
  -v    Verbose mode (for CHECK command)
</pre>

### Examples:

#### Generate hashsum list:
<pre>
$ ./gostsum [-r] "*.*" > hash.g94
</pre>
##### Always works in binary mode. 

#### Check hashsum file:
<pre>
$ ./gostsum [-v] -c hash.g94
</pre>
##### Exit code is always 0 in vebose mode. 

## License

This project is licensed under the ISC License.
##### Copyright (c) 2020-2021 ALBANESE Research Lab.
