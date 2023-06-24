FROM golang:1.21rc2-alpine3.18 as build

WORKDIR /challenge

COPY go.mod docker_and_go.go .

RUN go build

FROM scratch

COPY --from=build /challenge/docker-and-go /bin/

CMD ["docker-and-go"]
