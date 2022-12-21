# self-certs
Self sign certificate creation tools

## 1. Create root certs (If not created)
```zsh
> ./create_root_certs.sh
````

## 2. Allow traget domain
```zsh
> ./allow_domain.sh <domain.name>
```

## 3. Create certs for domain
```zsh
> ./create_domain_certs.sh <domain.name>
```

## 4. Make your certificate is trusted (<domain.name>.crt)
