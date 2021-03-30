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

## Examples:

### Generate hashsum list:
<pre>
./gostsum -t "*.*" > hash.txt
</pre>

### Check hashsum file:
<pre>
./gostsum [-v] -c hash.txt
</pre>
#### Exit code is 0 in vebose mode. 

### Generate recursive hashsum list:
$ find . -type f -name "*.*" -exec ./gostsum -t '{}' \; 

### Recusive Hash in Bash:
<pre>
#/bin/bash
find . -type f \( -name "$1" -o -name "$2" -o -name "$3" \) -exec ./gostsum -t '{}' \;
</pre>
#### Evocation:
<pre>
sh recusive.sh *.txt *.csv *.ldj
</pre>
### Recusive Hash in Batch:
<pre>
@ECHO OFF

set stdin=%*
setlocal enabledelayedexpansion
for /r %%a in (%stdin%) do (
  set "x=%%a"
  tool\gostsum-t ".!x:%cd%\=\!"
)</pre>
#### Evocation:
<pre>
recusive.bat *.txt *.csv *.ldj
</pre>
