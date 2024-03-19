# generate_cert
Original code taken from https://go.dev/src/crypto/tls/generate_cert.go and modified to suit our needs

## Build
go install

## Usage (bash)
```
generate_cert --ca --name 299m-ca --host "299m.io"
generate_cert --host "127.0.0.1,localhost" --cacert ca-cert.pem --cakey ca-key.pem

### For Golang server, concatenate the cert and ca-cert
cat cert.pem ca-cert.pem > combined-certs.pem

```
