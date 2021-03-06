# twemproxy-exporter

Expose twemproxy stats to prometheus

## Building

### Mac/Linux

0) set GOROOT environment variable
1) Install Go and Make
2) make

### Docker

0) set GOROOT environment variable
1) Install Docker, Go and Make
2) make docker


## Running

### Mac/Linux

```
./twemproxy-exporter
```

### Docker

```
docker pull maguec/twemproxy-exporter:latest
docker run -i -t -p 9119:9119 maguec/twemproxy-exporter
```

## Testing

run either the docker container or the raw application binary

```
curl http://localhost:9119/health
```

---
Copyright © 2018, Chris Mague
