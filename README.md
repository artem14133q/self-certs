# self-certs
Self sign certificate creation tools

## 1. Create root certs (If not created)
```zsh
./create_root_certs.sh
````

## 2. Allow traget domain
```zsh
./allow_domain.sh <domain.name>
```

## 3. Create certs for domain
```zsh
./create_domain_certs.sh <domain.name>
```

## 4. Make your certificate is trusted (<domain.name>.crt)

### Linux:
```zsh
sudo mv <domain.name>.crt /usr/share/ca-certificates/
cd /usr/share/ca-certificates
sudo chmod 644 <domain.name>.crt
sudo dpkg-reconfigure ca-certificates
sudo update-ca-certificates
```

### MacOs:
Import your cert in *KeyChain* app and make it is trusted.

### Windows:
Open cert like a programm.
