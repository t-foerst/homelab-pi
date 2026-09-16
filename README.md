# homelab-pi

Docker-Compose-Setups für einen Raspberry Pi im Homelab.

## Services

| Ordner | Dienst | Zweck |
|---|---|---|
| `adguard/` | AdGuard Home | DNS-Server & Werbeblocker |
| `monitoring/` | Prometheus, Grafana, node-exporter, pve-exporter | Metriken & Dashboards (u.a. Proxmox) |
| `netbird/` | Netbird | WireGuard-basiertes VPN |
| `uptime-kuma/` | Uptime Kuma | Verfügbarkeits-Monitoring |

## Nutzung

In den jeweiligen Ordner wechseln und starten:

```sh
cd <service>
docker compose up -d
```

`monitoring/` benötigt eine `.env` (siehe `.env.example`).
