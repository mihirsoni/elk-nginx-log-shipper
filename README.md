#### Logshipper generator for ELK Stake

### Prerequisite

* Docker > 19

### Setup
* `git clone git@github.com:mihirsoni/elk-nginx-log-shipper.git`
*  `docker-compose build && docker-compose up`

It should bring up 3 containers :

* Nginx
* ES
* Logstash


### Request generator

Use [hey](https://github.com/rakyll/hey) for generating requests.

* `go get -u github.com/rakyll/hey`
* `cd $GOPATH/src/github.com/rakyll/hey`
* `go build`
* ` hey http://localhost:8080`
