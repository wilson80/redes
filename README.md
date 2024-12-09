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
    copy running-config startup-config


1. **comando para ver las configuraciones**
   ```bash
   show running-config








Switch>enable
Switch#conf terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#hostname S2
S2(config)#line console 0
S2(config-line)#password cisco
S2(config-line)#login
S2(config-line)#exit
S2(config)#enable secret class
S2(config)#line vty 0 15
S2(config-line)#password cisco
S2(config-line)#login
S2(config-line)#exit
S2(config)#service password-encryption 
S2(config)#banner motd #Solo Acceso Autorizado#
S2(config)#interface vlan1
S2(config-if)#ip address 192.168.1.2 255.255.255.0
S2(config-if)#no shutdown 

S2(config-if)#
%LINK-5-CHANGED: Interface Vlan1, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan1, changed state to up

S2(config-if)#exit
S2(config)#exit
S2#
%SYS-5-CONFIG_I: Configured from console by console

S2#copy running-config startup-config 
Destination filename [startup-config]? 
Building configuration...
[OK]



**ping desde el swith a las pcs**

