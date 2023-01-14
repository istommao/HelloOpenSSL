# OpenSSL Digest

## Digest List

```bash
openssl dgst -list
```

<details><summary>Show openssl help</summary>
<p>

```bash
Supported digests:
-blake2b512                -blake2s256                -md4
-md5                       -md5-sha1                  -mdc2
-ripemd                    -ripemd160                 -rmd160
-sha1                      -sha224                    -sha256
-sha3-224                  -sha3-256                  -sha3-384
-sha3-512                  -sha384                    -sha512
-sha512-224                -sha512-256                -shake128
-shake256                  -sm3                       -ssl3-md5
-ssl3-sha1                 -whirlpool
```

</p>
</details>


## Echo String

```bash
echo "Hello" | openssl dgst -sha3-224
```

## Digest file

```bash
openssl dgst -sha3-224 input.file
```
