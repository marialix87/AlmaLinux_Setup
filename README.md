# AlmaLinux_Setup

# Instalación de AlmaLinux 9 en VirtualBox

Este repositorio documenta paso a paso cómo instalé AlmaLinux 9 en VirtualBox para construir un entorno de prácticas de administración de servidores Linux.

 🖥️ Requisitos previos

- Sistema operativo host: Windows 11
- VirtualBox instalado
- ISO de AlmaLinux 9.3 descargada (~11 GB)

🔧 Configuración de la VM

- 2 CPU
- 4096 MB de RAM
- 20 GB de disco dinámico
- Red: Adaptador en puente (Bridge)

- 📸 Proceso de instalación (con imágenes opcionales)

## 1. Crear la VM

- Omitir instalación desatendida
- Asignar nombre y recursos

## 2. Selección de ISO

- Adjuntar ISO de AlmaLinux al iniciar

## 3. Instalación

- Elegir idioma
- Configurar particionado automático
- Crear usuario administrador y root

🔐 Configuración post-instalación

## Acceso por SSH desde otra PC

  sudo systemctl enable --now sshd
Ver IP con:
ip a
Conectarse con MobaXterm o PuTTY

✅ Verificación y primeros paquetes

sudo dnf update -y
sudo dnf install -y vim git wget net-tools

Conectividad

ping -c 3 google.com



