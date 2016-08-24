# npm-proxy-cache

Docker image for [npm-proxy-cache](https://github.com/runk/npm-proxy-cache). Targeting version range 0.x.x (at time of creation 0.4.2 was latest and tested).

## Image Details
* built on node:6
* exposed 8080

## Settings
* `-h 0.0.0.0` - host is set to 0.0.0.0:8080
* `-t 86400` - TTL set to 86400 (one week)
* `-f` - real module names enabled (no hashed names). 


## Usage

`npm --proxy http://npm-proxy-cache:8080 --https-proxy http://npm-proxy-cache:8080 --strict-ssl false install`

This tool is protected by the GNU General Public License v3.

Copyright Jeffrey Hann 2016
