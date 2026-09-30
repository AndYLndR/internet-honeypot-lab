# 01 — Arquitectura

Quería una arquitectura sencilla, aislada y fácil de destruir una vez terminado el experimento.

```text
Internet
   │
   ▼
Hetzner Cloud Firewall
   │
   ▼
Debian 13 VPS
   │
   ▼
T-Pot
   │
   ├── Cowrie
   ├── Dionaea
   ├── SentryPeer
   ├── Heralding
   ├── Tanner
   ├── ConPot
   ├── RDPHoneypot
   ├── Suricata
   └── otros honeypots
   │
   ▼
Elasticsearch
   │
   ├── Kibana
   └── T-Pot Attack Map
```

## VPS

```text
Provider: Hetzner Cloud
Region: Nuremberg, Germany
Instance: CPX42
Architecture: x86-64
vCPU: 8
RAM: 16 GB
Storage: 320 GB NVMe
OS: Debian GNU/Linux 13
```

El VPS no estaba conectado a una red privada, no contenía información personal ni servicios reales y estaba pensado para ser eliminado al terminar.

Los servicios administrativos `64295/tcp` y `64297/tcp` se mantuvieron restringidos mediante firewall a mi IP administrativa.
