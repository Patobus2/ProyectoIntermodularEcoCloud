# ProyectoIntermodularEcoCloud
EcoCloud Industrial — Infraestructura Cloud y Green IT
Autor: Vicente Sanchis Pablo (NIA: 10899461)
Módulo: Proyecto Intermodular (2º ASIR)
Centro: IES Conselleria (València)

1. Descripción del Proyecto
EcoCloud Industrial es un Proveedor de Servicios Gestionados (MSP) local enfocado en ofrecer soluciones de Micro-Cloud privada en alta disponibilidad, ciberseguridad industrial y computación verde (Green IT) para las PYMEs del sector manufacturero y tradicional de la Comunitat Valenciana.

2. Objetivo de la Infraestructura
Diseñar, automatizar y desplegar un clúster hiperconvergente resiliente y seguro que sustituya los servidores locales obsoletos de las PYMEs industriales. Los objetivos principales son:
Garantizar la continuidad de negocio mediante Alta Disponibilidad (HA) y copias inmutables (Estrategia 3-2-1 con Proxmox Backup Server).
Aislar la red de planta (OT/SCADA) de la red administrativa (IT) mediante cortafuegos perimetral y segmentación estricta por VLANs (pfSense).
Monitorizar y optimizar la eficiencia energética en tiempo real mediante el cálculo del índice PUE (< 1,25) con Prometheus y Grafana (Green IT).
Cumplir con los estándares normativos del Esquema Nacional de Seguridad (ENS) y el Reglamento General de Protección de Datos (RGPD).

3. Tecnologías Utilizadas
Virtualización: Proxmox VE (KVM y LXC).
Sistema Operativo: Debian 12 (Bookworm).
Redes y Seguridad: pfSense (Firewall, VLANs 802.1Q, WireGuard VPN).
Almacenamiento: OpenZFS (Pools con compresión LZ4).
Copias de Seguridad: Proxmox Backup Server (PBS).
Bases de Datos: MySQL.
Servidor Web y Proxy: Nginx.
Contenedores: Docker y Docker Compose.
Automatización / IaC: Ansible y Scripts Bash.
Monitorización: Prometheus y Grafana.
Control de Versiones: Git / GitHub.

## 4. Estructura del Repositorio
ecocloud-industrial/
├── playbooks/         
├── roles/             
├── variables/        
├── plantillas/        
├── inventario/        
├── documentacion/     
└── README.md          
