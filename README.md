[![GitHub go.mod Go version of a Go module](https://img.shields.io/github/go-mod/go-version/gomods/athens.svg)](https://github.com/KernelPryanic/goudpscan)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# **goudpscan**

Fastest UDP port scanner you've ever seen.

## Build

`go build -o bin/goudpscan`

## Install

`./install.sh`

## How to use

Run ``sudo goudpscan -f -t 1 -c 975 -p 7,19-22 -s 127.0.0-32.0/24 127.1.0.1``

Also checkout the lists of [flags](#flags) and [arguments](#arguments).

### Flags

* `    --help` - Show context-sensitive help (also try --help-long and --help-man).
* `    --print` - Print payloads.
* `-l, --payloads=PAYLOADS` - Paylaods yml config file.
* `-f, --fast` - Fast scan mode. Only "Open" or "Unknown" statuses.
* `-t, --timeout=1` - Timeout. How long to wait for response in seconds.
* `-r, --recheck=0` - Recheck. How many times to check every port.
* `-c, --maxConcurrency=768` - Maximum concurrency. How many to scan concurrently every timeout.
* `-s, --sort` - Sort results.
* `-p, --ports=7-1024 ...` - Ports to scan.

### Arguments

* `<hosts>` - Hosts to scan.
