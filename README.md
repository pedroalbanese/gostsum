# GOSTSUM(2)
## gostsum Parallel Implementation written in Go

### Usage:
<pre>
GOST R 34.11-94 CryptoPro Hashsum Tool - ALBANESE Lab (c) 2020-2021

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
