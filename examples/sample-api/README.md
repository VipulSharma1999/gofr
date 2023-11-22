# SAMPLE API
A sample http app built using gofr.

## RUN
To run the app follow the below steps:

1. ` go run main.go`

This will start the server at port 9000.

## DOCKER BUILD
To Build a docker image, follow the below steps:

On non linux machines :
1. `GOOS=linux go build main.go` This will build a go binary
2. `docker build -t sample-api:$(date +%s) .`

On linux machines(Ubuntu/Mac):
1. `go build main.go` This will build a go binary
2. `docker build -t sample-api:$(date +%s) .`