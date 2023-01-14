# 证书

## Create self-signed certificate

```bash
openssl req -new -x509 -key private_key.pem -out cert.pem -days 360
```

## Covert pem to pfx

```bash
openssl pkcs12 -export -inkey private_key.pem -in cert.pem -out cert.pfx
```
