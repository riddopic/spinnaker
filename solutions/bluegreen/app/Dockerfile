FROM golang:1.8-alpine
COPY . /go/src/helloworld 
WORKDIR /go/src/helloworld
RUN go install helloworld

FROM alpine:3.15.4
COPY --from=0 /go/bin/helloworld .
ENV PORT 6000
EXPOSE 6000 
ENTRYPOINT ["./helloworld"]