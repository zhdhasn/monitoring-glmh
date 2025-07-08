# Monitoring Stack

A containerized monitoring solution using:

- **Loki** for log aggregation
- **Grafana** for visualization
- **HAProxy** for load balancing
- **MinIO** for object storage

## Getting Started

```bash
docker-compose up -d

Directory Structure:
drwxrwxr-x  5 jahid jahid 4096 Jun 25 06:43 cache/
drwxr-x---  5 jahid jahid 4096 Jun 25 06:42 data/
-rw-rw-r--  1 jahid jahid 3541 Jun 26 03:25 docker-compose.yaml
drwxrwxr-x  8 jahid jahid 4096 Jul  8 05:14 .git/
-rw-rw-r--  1 jahid jahid  220 Jul  8 04:47 .gitignore
drwxrwxr-x  3 jahid jahid 4096 Jun 25 06:42 grafana/
-rw-rw-r--  1 jahid jahid  855 Jun 25 08:31 haproxy.cfg
drwxr-xr-x  2 root  root  4096 Jun 25 10:29 loki1-cache/
drwxrwxr-x  2 jahid jahid 4096 Jun 25 10:52 loki1-wal/
drwxr-xr-x  2 root  root  4096 Jun 25 10:29 loki2-cache/
drwxrwxr-x  2 jahid jahid 4096 Jun 25 10:52 loki2-wal/
drwxr-xr-x  2 root  root  4096 Jun 25 10:29 loki3-cache/
drwxrwxr-x  2 jahid jahid 4096 Jun 25 10:52 loki3-wal/
-rw-rw-r--  1 jahid jahid  998 Jul  7 08:03 loki-config.yaml
-rw-rw-r--  1 jahid jahid  242 Jul  8 05:14 REDME.md
drwxrwxr-x  5 jahid jahid 4096 Jun 25 06:43 wal/
jahid@docker-io:~/monitoring$ tree
.
├── cache
│   ├── loki1
│   ├── loki2
│   └── loki3
├── data
│   ├── minio1
│   ├── minio2
│   └── minio3
├── docker-compose.yaml
├── grafana
│   └── storage
├── haproxy.cfg
├── loki1-cache
├── loki1-wal
├── loki2-cache
├── loki2-wal
├── loki3-cache
├── loki3-wal
├── loki-config.yaml
├── REDME.md
└── wal
    ├── loki1
    ├── loki2
    └── loki3

