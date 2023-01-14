# RSA


## 生成密钥

```bash
openssl genrsa -out private_key.pem 4096
```

## 导出公钥

```bash
openssl rsa -in private_key.pem -pubout -out public_key.pem
```

## 查看密钥信息

```bash
openssl rsa -in private_key.pem -noout -text
```


## 查看公钥信息

```bash
openssl rsa -in public_key.pem -pubin -noout -text
```


## 加密数据

```bash
openssl rsautl -encrypt -inkey public_key.pem -pubin -in plain.txt -out secret.out
```

## 解密数据

```bash
openssl rsautl -decrypt -inkey private_key.pem -in secret.out > decode.txt
```
