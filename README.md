# GOSTSUM(2)
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/pedroalbanese/gostsum/blob/master/LICENSE.md) 
[![GoDoc](https://godoc.org/github.com/pedroalbanese/gostsum?status.png)](http://godoc.org/github.com/pedroalbanese/gostsum)
[![Go Report Card](https://goreportcard.com/badge/github.com/pedroalbanese/gostsum)](https://goreportcard.com/report/github.com/pedroalbanese/gostsum)
### GOST R 34.11-94 CryptoPro Hashsum Tool
<pre>
Usage of gostsum:
gostsum [-v] [-c &lt;hash.g94&gt;] [-r] -t &lt;file.ext&gt;

  -c string
        Check hashsum file.
  -r    Process directories recursively.
  -t string
        Target file/wildcard to generate hashsum list.
  -v    Verbose mode. (The exit code is always 0 in this mode)

</pre>

### Examples:

#### Generate hashsum list:
<pre>
$ ./gostsum [-r] -t "*.*" > hash.g94
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
