
### Criptografia com GPG

#### Criptografia Simétrica

```
gpg --armor --symmetric --cipher-algo AES256 <arquivo.txt>
```

#### Descriptografia Simétrica

```
gpg -o <arquivo.txt> -d <arquivo.txt.asc>
```

#### Criptografia Assimétrica

```
gpg -e -r key-id|name <arquivo.txt>
```

#### Descriptografia Assimétrica

```
gpg -o <arquivo.txt> -d <arquivo.gpg>
```

### Criptogafia com OpenSSL

#### Criptografar Arquivo

```
openssl enc -aes-256-cbc -salt -in <arquivo.txt> -out <arquivo.enc>
```

#### Descriptografar Arquivo
```
openssl enc -d -aes-256-cbc -in <arquivo.enc> -out <arquivo.txt>
```
