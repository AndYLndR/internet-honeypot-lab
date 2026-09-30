# 07 — Findings

## 1. La exposición empieza a generar actividad muy rápido

Antes de publicar Cowrie había 0 eventos. Poco después de abrir SSH/Telnet apareció la primera conexión espontánea.

## 2. Evento no significa atacante

Cowrie terminó con 34.745 eventos y 248 IPs de origen únicas.

## 3. Las credenciales básicas siguen apareciendo

Se observaron usernames y passwords extremadamente predecibles como `root`, `admin`, `password`, `1234` y `123456`.

## 4. No todo fueron simples escaneos

Cowrie también registró entradas como `config terminal`, `enable` y `linuxshell`.

## 5. La superficie de ataque importa

Los resultados dependen de los puertos y servicios publicados, así que no representan Internet completo.

## 6. La geolocalización debe interpretarse con cuidado

`Country field != nationality of attacker`.

## 7. Un laboratorio pequeño puede generar muchos datos

Con un coste de 3,39 € fue posible observar más de 105.000 eventos en menos de un día.
