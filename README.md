# gostsum(2)
## gostsum Parallel Implementation written in Go

### Usage:
<pre>
GOST R 34.11.94 CryptoPro Hashsum Tool - ALBANESE Lab (c) 2020-2021

Usage of gostsum:
  -c string
        Check hashsum file.
  -t string
        Target file/wildcard to generate hashsum list.
  -v    Verbose mode. (for CHECK command)
</pre>

### Generate hashsum list:
<pre>
./gostsum -t *.* > hash.txt
</pre>

### Check hashsum file:
<pre>
./gostsum [-v] -c hash.txt
</pre>

#### Exit code is 0 in vebose mode. 
