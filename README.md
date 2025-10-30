# Proyecto: Servidor Nextcloud en Ubuntu Server 22.04

## Proyecto personal de instalacion y configuración de un servidor **Nextcloud** en **Ubuntu Server 22.04** desplegado con **Docker Compose**, tambien pudiendo incluir una gesion de dominios con **Nginx**

## Tecnologías Utilizadas
 - Ubuntu Server 22-04
 - Docker & Docker Compose
 - Nextcloud
 - Nginx
 - SSH para administracion remota

## Pasos de Implementación
1. **Instalacion de Docker y Docker Compose**
  ```bash
  sudo apt update && sudo apt install docker docker-compose -y
  ```
2. **Creacion del archivo docker-compose.yml**
   (ver en repositorio el archivo completo)
3. **Configuración del entorno (.env)**
   ```bash
   MYSQL_PASSWORD=tu_contraseña_segura
   NEXTCLOUD_ADMIN_USER=admin
   NEXTCLOUD_ADMIN_PASSWORD=contraseña
   ```
4. **Levantamiento de contenedores**
   ```bash
   docker-compose up -d
   ```
5. **Acceso a la interfaz web**
   - Direccion local: **http://tu_ip_local:8080**
