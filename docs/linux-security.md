# Seguridad Básica en Servidores Linux

Pasos recomendados para blindar una máquina expuesta en red.

## Firewall UFW
- Política base restrictiva: `ufw default deny incoming` y `ufw default allow outgoing`.
- Habilitar SSH antes de activar el firewall: `ufw allow 22/tcp`.
- Habilitar firewall: `ufw enable`.

## Gestión de Accesos
- Deshabilitar autenticación SSH por contraseña en `/etc/ssh/sshd_config` (`PasswordAuthentication no`).
- Deshabilitar login directo de root (`PermitRootLogin no`).
- Utilizar `fail2ban` para mitigar ataques de fuerza bruta.
