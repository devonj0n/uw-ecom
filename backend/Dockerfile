# Use the official Golang image to create a build artifact.
FROM golang:1.16 as builder
WORKDIR /src
COPY . .
RUN go mod tidy
RUN go build -o app ./cmd/app

# Use the Alpine image for a smaller footprint.
FROM alpine:3.13
COPY --from=builder /src/app /app
ENTRYPOINT ["/app"]
