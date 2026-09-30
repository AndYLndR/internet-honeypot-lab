# 06 — Análisis de datos

La observación se realizó principalmente con T-Pot Attack Map, Kibana, Cowrie Dashboard y el dashboard general de T-Pot.

Al terminar:

```text
T-Pot events: ~105,000
Attack Map 24H snapshot: 105,057
Cowrie: 34,745 events
Cowrie unique source IPs: 248
Cowrie unique hashes: 19
```

![Final dashboard](../screenshots/07-results/kibana-overview-t24h.png)

![Final Cowrie](../screenshots/07-results/cowrie-overview-t24h.png)

Entre los usernames y passwords observados aparecieron valores típicos como `root`, `admin`, `user`, `password`, `1234`, `123456` y `admin1234`.

También aparecieron comandos como `config terminal`, `enable` y `linuxshell`.

Los eventos no se interpretan como individuos: una misma IP puede producir múltiples conexiones y eventos.
