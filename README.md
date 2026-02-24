# Concentrado de Reportes de Clase  
## Seguridad de Datos – Redes, Modelo OSI, TCP/IP y Hacking  
**Alumno:** Abraham CAstelan Vega  
**Asignatura:** Seguridad de Datos  
**Repositorio:** Seguridad-de-Datos2026  

---

# 📡 Modelo OSI vs TCP/IP

## 📚 Comparación de Modelos

| Capa OSI | Nombre              | TCP/IP        | Función Principal                          | Ejemplos |
|-----------|--------------------|--------------|--------------------------------------------|----------|
| 7 | Aplicación | Aplicación | Interacción con el usuario | Gmail, URLs, HTTP |
| 6 | Presentación | Aplicación | Formato, cifrado y compresión | SSL/TLS |
| 5 | Sesión | Aplicación | Control de sesiones | Active Directory, VoIP |
| 4 | Transporte | Transporte | Puertos y control de flujo | TCP, UDP |
| 3 | Red | Red | Direccionamiento lógico | IP Address |
| 2 | Enlace de Datos | Enlace de datos | Direccionamiento físico | MAC Address |
| 1 | Física | Física | Transmisión de bits | Cable, fibra |

---

# Capa 2 – Enlace de Datos

## 🔹 MAC Address
- Dirección física única del dispositivo.
- No es enrutable.
- El switch trabaja únicamente con direcciones MAC.
- Se utiliza para reenviar tráfico dentro de la red local.

### MAC Address Spoofing
Consiste en suplantar una MAC Address para:
- Evadir controles de acceso
- Interceptar tráfico
- Realizar ataques Man-in-the-Middle

### Seguridad en Switches
- El switch solo conmuta tráfico.
- No analiza direcciones IP.
- Dos MAC en distintos puertos no generan alerta.
- Con **802.1X**, el puerto intruso puede ser bloqueado.

### Ataques comunes en Capa 2
- ARP Poisoning
- DHCP Poisoning
- DNS Poisoning
- VLAN Hopping
- STP Manipulation

---

# Capa 3 – Red

## 🔹 Direcciones Lógicas (IP Address)
- Permiten identificar dispositivos en una red.
- Utilizan **notación decimal con puntos** (ejemplo: 192.168.1.1).
- El switch no trabaja con IP, solo con MAC.

### Tipos de direcciones:
- Direcciones de archivos
- Direcciones de correo electrónico
- Direcciones web
- Direcciones de telefonía IP

### Ataques en Capa 3
- IP Spoofing
- ICMP Flood
- Smurf Attack
- Routing Table Poisoning

---

# Capa 4 – Transporte

## 🔹 Puertos
Existen **65,536 puertos (2¹⁶)**.

| Puerto | Servicio |
|--------|----------|
| 80 | HTTP |
| 443 | HTTPS |
| 22 | SSH |
| 21 | FTP |
| 25 | SMTP |
| 53 | DNS |
| 110 | POP3 |
| 143 | IMAP |
| 3306 | MySQL |
| 1433 | SQL Server |
| 3389 | RDP |

---

## TCP vs UDP

| TCP | UDP |
|------|------|
| Orientado a conexión | No orientado a conexión |
| 3-Way Handshake | No requiere handshake |
| Control de errores | Sin control de errores |
| Más seguro | Más rápido |

### 3-Way Handshake
1. SYN  
2. SYN-ACK  
3. ACK  

---

# Port Scanning

Proceso para identificar puertos abiertos y servicios activos.  
Se realiza en la fase de **reconocimiento**.

### Herramientas:
- Nmap
- Netcat
- Masscan
- Tenable Nessus
- Qualys
- OpenVAS

---

# Identificación de Servicios

## Banner Grabbing
Permite obtener:
- Tipo de servicio
- Versión
- Sistema operativo

La exposición del banner incrementa el riesgo de ataque.

---

# Vulnerabilidades

## ¿Qué es una vulnerabilidad?
Debilidad o punto frágil que puede ser explotado por un atacante mediante un **exploit**.

## Conceptos Clave
- **Flaw:** falla de diseño
- **Exploit:** código que aprovecha vulnerabilidad
- **Payload:** acción ejecutada tras explotar
- **Patch:** corrección de seguridad
- **Zero-Day:** vulnerabilidad sin parche

## Evaluación de Riesgos
Frameworks:
- STRIDE
- MITRE ATT&CK

Medidas de mitigación:
- Parchar servicios
- Deshabilitar servicios innecesarios
- Firewall
- Segmentación de red
- IDS/IPS

---

# Tipos de Hackers

- 🟢 White Hat – Hackers éticos autorizados
- 🔴 Black Hat – Hackers maliciosos
- ⚪ Gray Hat – Intermedio
- 🟡 Script Kiddie – Uso de herramientas sin conocimiento profundo
- 🔵 Hacktivista – Motivación ideológica
- 🟣 Insider – Empleado con acceso legítimo

---

# Pentesting

## Tipos
- Caja Blanca
- Caja Negra
- Caja Gris

## Fases
1. Reconocimiento
2. Footprinting
3. Network Mapping
4. Identificación de servicios
5. Análisis de vulnerabilidades
6. Obtención de acceso
7. Escalada de privilegios
8. Daisy Chaining

---

# SIEM

Security Information and Event Management:

- Centraliza logs
- Detecta incidentes
- Correlación de eventos
- Respuesta ante ataques

---

# Ataques por Capa OSI

| Ataque | Capa |
|---------|------|
| MAC Spoofing | 2 |
| ARP Poisoning | 2 |
| IP Spoofing | 3 |
| Port Scanning | 4 |
| Session Hijacking | 5 |
| SSL Stripping | 6 |
| SQL Injection | 7 |

---

# Troubleshooting

Proceso de encontrar la raíz del problema.

- Falso positivo: Se detecta amenaza inexistente.
- Falso negativo: No se detecta una amenaza real.

---

# Conclusión

El modelo OSI permite clasificar los ataques según la capa en la que actúan, facilitando su análisis y mitigación. Comprender la relación entre MAC, IP, puertos y protocolos es fundamental para identificar vulnerabilidades y aplicar controles adecuados.  

La seguridad de datos no solo depende de herramientas, sino del conocimiento profundo del funcionamiento de redes, protocolos y servicios. La correcta gestión de riesgos, la segmentación de red y el monitoreo 
constante mediante SIEM son esenciales para reducir la superficie de ataque.  

Clasificar ataques por capa mejora la defensa, fortalece auditorías y permite implementar estrategias efectivas de ciberseguridad.
