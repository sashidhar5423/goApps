FROM golang:1.16.2 
WORKDIR /app
COPY go.mod, go.sum ./
RUN go.mod download
COPY . .
RUN go build -o main .
EXPOSE  9095
CMD ["./main"]


