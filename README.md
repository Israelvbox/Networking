# Fundamentos de Redes Informáticas

Este repositorio contiene conceptos clave y explicaciones detalladas sobre redes informáticas. A continuación, encontrarás los temas cubiertos:

<br>

## Propósito del Documento
Este documento tiene como objetivo servir como una guía introductoria al mundo del networking, cubriendo temas esenciales organizados en los siguientes apartados:

## Instrucciones tecnicas

- **Redes**
- **Redes de area local**
- **Modelo OSI**
- **Modelo TCP/IP**
- **Protocolos**

## Contenido

### Redes

- Interconexión de un conjunto de dispositivos capaz de comunicarse
- Dispositivo: máquina, portátil, móvil, dispositivo de interconexión (router)...
- Comunicación: intercambio de información sobre cualquier medio

<br>
<img src="https://github.com/Israelvbox/Networking/blob/main/images/redes.png" width=600px>

<br>

## Redes de area local

### **1. PAN (Personal Area Network)**
Es una red de área personal diseñada para la comunicación entre dispositivos cercanos, generalmente en un rango de pocos metros.

#### Características:
- Alcance: Pocos metros (usualmente hasta 10 metros).
- Dispositivos conectados: Teléfonos móviles, tablets, auriculares Bluetooth, smartwatches.
- Medios: Generalmente inalámbrico (Bluetooth, NFC, Zigbee).

**Ejemplo: Conexión entre un teléfono móvil y unos auriculares Bluetooth o entre un smartwatch y un smartphone.**

#### Ventajas:

- Configuración sencilla.
- Consumo de energía reducido en dispositivos.

#### Limitaciones:

- Alcance muy limitado.
- Baja velocidad de transferencia de datos en comparación con otros tipos de redes.


### **2. LAN (Local Area Network)**

Es una red de área local que conecta dispositivos en un espacio geográfico reducido, como una casa, oficina o un edificio.

#### Características:
- Alcance: Unos pocos metros hasta varios cientos (por ejemplo, una oficina o escuela).
- Dispositivos conectados: Computadoras, impresoras, servidores, cámaras IP.
- Medios: Alámbrico (cables Ethernet) o inalámbrico (Wi-Fi).
  
**Ejemplo: Red doméstica que conecta computadoras, televisores inteligentes y routers.**

#### Ventajas:

- Alta velocidad de transferencia (10 Mbps hasta varios Gbps).
- Control centralizado (por ejemplo, un router o un switch).

#### Limitaciones:

- Alcance limitado a un área específica.
- Dependencia de dispositivos específicos como switches y routers.

### **3. MAN (Metropolitan Area Network)**
Definición:
Es una red que cubre un área geográfica más grande que una LAN, típicamente una ciudad o campus universitario.

#### Características:

- Alcance: De varios kilómetros (una ciudad o campus universitario).
- Dispositivos conectados: Varias LANs interconectadas, servidores y equipos de telecomunicaciones.
- Medios: Fibra óptica, enlaces dedicados o inalámbricos (WiMAX, LTE).

**Ejemplo: Red que conecta las oficinas de una empresa distribuidas por una ciudad.**

#### Ventajas:

- Conexión más amplia que una LAN.
- Ideal para organizaciones distribuidas en una región específica.

#### Limitaciones:

- Más costosa que una LAN.
- Requiere infraestructura más compleja, como enlaces dedicados.

### **4. WAN (Wide Area Network)**

Es una red de área amplia que conecta dispositivos o redes a través de grandes distancias geográficas, como países o continentes.

#### Características:

- Alcance: Desde cientos de kilómetros hasta global (ejemplo: Internet).
- Dispositivos conectados: Routers, servidores, centros de datos, LANs y MANs.
- Medios: Enlaces satelitales, fibra óptica, cableado submarino.
- Ejemplo: Internet, que conecta millones de dispositivos a nivel mundial.

#### Ventajas:

- Permite la conexión de usuarios y dispositivos en ubicaciones remotas.
- Escalabilidad casi ilimitada.

#### Limitaciones:

- Alta latencia en comparación con LANs y MANs.
- Costos elevados para implementar y mantener.

<br>
<img src="https://github.com/Israelvbox/Networking/blob/main/images/pan-man-wan-lan.jfif" width=500px>

<br>

## **Modelo OSI**

- Aplicación: Protocolos como HTTP, FTP, DNS.
- Presentación: Codificación y cifrado.
- Sesión: Establecimiento de sesiones.
- Transporte: TCP/UDP con ejemplos de uso.
- Red: IP, routers, subnetting.
- Enlace de Datos: MAC addresses, switches.
- Física: Tipos de cables, estándares como Ethernet.

<br>
<img src="https://github.com/Israelvbox/Networking/blob/main/images/modelos-osi.webp" width=500px>

<br>

### **Modelo TCP/IP**

El protocolo **TCP/IP (Transmission Control Protocol/Internet Protocol)** es un conjunto de normas que permite la comunicación entre dispositivos en redes, como Internet. Su diseño se basa en una arquitectura de cuatro capas:


#### **1. Capa de Acceso a la Red**
- **Función:** Maneja la transmisión física de datos en la red local (LAN/WAN).  
- **Protocolos:** Ethernet, Wi-Fi.  


#### **2. Capa de Internet**
- **Función:** Gestiona el direccionamiento y el enrutamiento de paquetes entre redes.  
- **Protocolos:**  
  - **IP:** Direccionamiento lógico.  
  - **ARP:** Traducción de direcciones IP a MAC.  
  - **ICMP:** Diagnósticos de red (como `ping`).  


#### **3. Capa de Transporte**
- **Función:** Asegura la entrega confiable o rápida de datos entre dispositivos.  
- **Protocolos:**  
  - **TCP:** Confiable, orientado a conexión.  
  - **UDP:** No confiable, sin conexión, rápido.  


#### **4. Capa de Aplicación**
- **Función:** Interactúa directamente con el usuario y soporta aplicaciones.  
- **Protocolos:**  
  - **HTTP:** Navegación web.  
  - **FTP:** Transferencia de archivos.  
  - **SMTP:** Envío de correos.  
  - **DNS:** Resolución de nombres de dominio.


### **Características Clave**
- Escalabilidad: Maneja desde redes pequeñas hasta Internet.  
- Interoperabilidad: Compatible con hardware y software diverso.  
- Confiabilidad: TCP asegura la entrega correcta y ordenada.  

TCP/IP es práctico y universal, aunque menos detallado que el modelo OSI.

<br>
<img src="https://github.com/Israelvbox/Networking/blob/main/images/tcp-ip-model.png" width=500px>
<br>


## Puertos mas usados 

| **Puerto** | **Protocolo** | **Nombre**       | **Descripción**                                                                           |
|------------|---------------|------------------|-------------------------------------------------------------------------------------------|
| 20         | TCP           | FTP-Data         | Transmisión de datos FTP.                                                                 |
| 21         | TCP           | FTP              | Protocolo de transferencia de archivos.                                                   |
| 22         | TCP           | SSH              | Secure Shell para acceso remoto seguro.                                                   |
| 23         | TCP           | Telnet           | Protocolo de acceso remoto no seguro.                                                     |
| 25         | TCP           | SMTP             | Protocolo para envío de correos electrónicos.                                             |
| 53         | TCP/UDP       | DNS              | Resolución de nombres de dominio.                                                         |
| 67         | UDP           | DHCP Server      | Asignación de direcciones IP desde el servidor DHCP.                                      |
| 68         | UDP           | DHCP Client      | Recepción de direcciones IP por el cliente DHCP.                                          |
| 69         | UDP           | TFTP             | Protocolo trivial de transferencia de archivos.                                           |
| 80         | TCP           | HTTP             | Protocolo de transferencia de hipertexto (web).                                           |
| 110        | TCP           | POP3             | Protocolo para recepción de correos electrónicos (Post Office Protocol v3).               |
| 123        | UDP           | NTP              | Protocolo para sincronización de tiempo.                                                  |
| 143        | TCP           | IMAP             | Protocolo para gestión de correos electrónicos.                                           |
| 161        | UDP           | SNMP             | Protocolo de gestión de dispositivos en red.                                              |
| 162        | UDP           | SNMP             | Notificaciones SNMP para eventos en la red.                                               |
| 389        | TCP/UDP       | LDAP             | Protocolo ligero de acceso a directorios.                                                 |
| 443        | TCP           | HTTPS            | HTTP seguro mediante SSL/TLS.                                                             |
| 445        | TCP           | SMB/CIFS         | Protocolo para compartir archivos e impresoras (Windows).                                 |
| 514        | UDP           | Syslog           | Registro y recopilación de logs en sistemas Unix/Linux.                                   |
| 587        | TCP           | SMTP (Submission)| Envío de correos electrónicos con autenticación.                                          |
| 993        | TCP           | IMAPS            | IMAP seguro mediante SSL/TLS.                                                             |
| 995        | TCP           | POP3S            | POP3 seguro mediante SSL/TLS.                                                             |
| 3306       | TCP           | MySQL            | Conexión a bases de datos MySQL.                                                          |
| 3389       | TCP           | RDP              | Protocolo de escritorio remoto de Microsoft.                                              |
| 8080       | TCP           | HTTP-Alt         | Puerto alternativo para HTTP.                                                             |





   
   

