# Lab Journal

## 2026-09-29 — Infraestructura inicial

```text
Provider: Hetzner Cloud
Location: Nuremberg, Germany
Instance: CPX42
Architecture: x86-64
RAM: 16 GB
Storage: 320 GB NVMe
OS: Debian GNU/Linux 13
```

- Clave SSH dedicada.
- Usuario administrativo `tpotadmin`.
- SSH restringido mediante cloud firewall.
- Sin red privada.
- Honeypots todavía no expuestos.

## 2026-09-29 — Instalación de T-Pot

```text
Version: 24.04.1
Commit: 5d95017d3ce7e8a0ecea8655cb8ac69c0d7b800f
Edition: HIVE / T-Pot Standard
SSH admin: 64295/tcp
```

## 2026-09-29 — Pre-exposure

```text
1M: 0
1H: 0
24H: 0
```

## 2026-09-29 — T0

Se habilitó Cowrie en `TCP 22` y `TCP 23`. No se guardó el segundo exacto de aplicación de la regla.

## 2026-09-29 19:47:14 — Primer evento

```text
Honeypot: Cowrie
Protocol: Telnet
Destination port: 23
Source IP geolocation: United States
T-Pot reputation: Bad Reputation
```

## 2026-09-29 ~19:57 — Actividad inicial

```text
1H: 15
24H: 15
Protocols: SSH, Telnet, HTTP, SMB
```

## 2026-09-29 — Primer análisis de Kibana

```text
36 events
Cowrie: 18
Dionaea: 9
Redis honeypot: 6
SentryPeer: 2
Tanner: 1
```

Cowrie mostraba `19 events`, `5 unique source IPs` y `1 unique hash`. Los paneles de credenciales y comandos todavía estaban vacíos.

## 2026-09-30 — Final del periodo

```text
Attack Map 24H snapshot: 105057
General dashboard: ~105k events
Cowrie: 34,745 events
Cowrie unique source IPs: 248
Cowrie unique hashes: 19
```

## 2026-09-30 — Teardown

Se guardaron resultados y vídeo, después se eliminó completamente el proyecto de Hetzner.

```text
Resources deleted:
Server
Primary IPv4
Primary IPv6
Firewall

Final usage: €3.39 VAT included
Status: LAB DESTROYED
```
