# **Instrucciones de la practica del viernes semana 1**

**configurar dos switch y dos pcss** 

---

## **comandos para los switch**

1. [Descripción](#descripción)
2. [Características](#características)
3. [Instalación](#instalación)
4. [Uso](#uso)
5. [Requisitos](#requisitos)
6. [Contribuciones](#contribuciones')
7. [Autores](#autores)
8. [Licencia](#licencia)

---

## **Configuracion de switches**


- **iniciales**:  
enable
configure terminal 

- **hostname**:  


- **hostname**:  
- **hostname**:  
- **hostname**:  
- **hostname**:  









---

## **Características**

- Gestión de usuarios y permisos (Administrador).  
- Subida y descarga de archivos.  
- Integración con Docker para despliegue fácil.  
- Autenticación segura mediante credenciales.  
- Visualización organizada de archivos por categorías.  

---

## **Instalación**

Sigue estos pasos para configurar el proyecto en tu entorno local:





1. **enable:**
   ```bash
   enable


1. **enable:**
   ```bash
   configure terminal
   
1. **nombrar:**
   ```bash
   hostname S2

1. **contrasena:**
   ```bash
   line console 0
   password cisco 
   login
   exit

1. **password a EXEC privilegiado (class es la constrasena):**
   ```bash
   enable secret class


1. **configurar las lineas**
   ```bash
   line vty 0 15
   password cisco
   login
   exit

1. **encriptar la contrasena**
   ```bash
   service password-encryption

1. **banner**
   ```bash
   banner motd #Authorized accdessss onlyyy #
 
1. **configuracion de la direccion ip (SIV (switch inteface virtual))**
   ```bash
   interface vlan 1  
   ip address 192.168.1.1 255.255.255.0
   no shutdown




1. **comando para ver las configuraciones**
   ```bash
    copy running-configur startup-config


1. **comando para ver las configuraciones**
   ```bash
   show running-config

