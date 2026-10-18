## 2026-10-17 — SSH y logs de autenticación
- `whoami` → muestra el usuario actual
- `ssh usuario@localhost` → conexión SSH a la misma máquina (loopback, 127.0.0.1)
- Primera conexión: SSH guarda la huella del servidor en ~/.ssh/known_hosts
  (si cambia después → posible man-in-the-middle)
- `sudo grep "Failed password" /var/log/auth.log` → ver intentos fallidos de login
