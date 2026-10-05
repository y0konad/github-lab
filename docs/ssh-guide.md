# Gestión de Llaves SSH y Configuración

Configuración segura y cómoda para servidores y repositorios Git.

## Generación de Llaves Seguras
Preferir siempre curvas elípticas Ed25519 sobre RSA:
`ssh-keygen -t ed25519 -C "usuario@dominio.com"`

## Archivo ~/.ssh/config
Estructurar alias para evitar recordar direcciones IP o flags:
```text
Host mi-servidor
  HostName 192.168.1.50
  User deploy
  IdentityFile ~/.ssh/id_ed25519
  Port 2222
```
