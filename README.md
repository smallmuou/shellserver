# ShellServer

> ShellServer is a server to execute shell command over http request. With it, you can operate remote pc like local pc.

## Startup

```bash
git clone https://github.com/smallmuou/shellserver
cd shellserver
./startup 1234
```
PS: default port is 8000

## Usage

```bash
curl -X POST http://serverip:port/cgi-bin/cmd.cgi -d 'your shell cmd'
```

## Example

```bash
curl -X POST  http://localhost:1234/cgi-bin/cmd.cgi -d 'ls'
curl -X POST  http://localhost:1234/cgi-bin/cmd.cgi -d 'top'
```

## When to use

* Lack of backend capability. but need to setup a http service quick.
* Control a remote pc through app.
* Put some json file to setup a json-rpc service.