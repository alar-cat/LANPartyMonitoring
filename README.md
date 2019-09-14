# LANPartyMonitoring
Fitxers de Docker i altres per monitorar la LAN Party

## Serveis
* Prometheus
* Alert Manager
* Grafana
* Caddy

## Instal·lar Docker
```bash
sudo apt install docker.io docker-compose
```

## Configurar correu-e
La configuració del correu-e és al fitxer `alertmanager/config.yml`. Els paràmetres a editar són `smtp_*`.

## Executar
### Executar docker-compose
```bash
ADMIN_USER=admin ADMIN_PASSWORD=password docker-compose -f docker-compose.yml -f docker-compose.exporters.yml up -d
```
