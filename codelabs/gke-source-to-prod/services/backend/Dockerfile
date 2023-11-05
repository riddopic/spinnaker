FROM golang:1-bullseye

ADD . /go/src/spinnaker.io/demo/k8s-demo

RUN go install spinnaker.io/demo/k8s-demo

ENTRYPOINT /go/bin/k8s-demo
