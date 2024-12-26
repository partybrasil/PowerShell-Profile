# 🎨 PowerShell Profile Configuration

Este repositorio contiene un archivo de perfil personalizado para PowerShell 7, diseñado para optimizar y personalizar la sesión de PowerShell del usuario Party.

## 📄 Contenido del Perfil

### 🌐 Configuraciones de Entorno

- **Título de la Ventana**: Establece el título de la ventana de PowerShell a `Party's Custom PowerShell`.
- **Prompt Personalizado**: Define un prompt personalizado que muestra el nombre de usuario y el nombre del equipo.
- **Función de Bienvenida**: Limpia la pantalla y muestra un mensaje de bienvenida al iniciar la sesión.
- **Tema de Oh-My-Posh**: Carga un tema personalizado de Oh-My-Posh.

### 📝 Alias Personalizados

Define alias para comandos de uso frecuente:

- `ll` para `Get-ChildItem`
- `grep` para `Select-String`
- `vim` para `notepad`
- `la` para `Get-ChildItem -Force`
- `cls` para `Clear-Host`
- `new` para `New-Item`
- `delete` para `Confirm-Delete`

### 📦 Módulos Personalizados

Importa módulos personalizados, incluyendo:

- `Microsoft.WinGet.CommandNotFound`: Sugerencias de comandos cuando se escriben incorrectamente.

### 🔧 Funciones Personalizadas

Define varias funciones útiles:

- `Confirm-Delete`: Elimina un archivo o directorio con confirmación.
- `Get-ProcessList`: Lista procesos en un formato simplificado.
- `Backup-File`: Crea una copia de seguridad de un archivo.
- `Get-DiskUsage`: Muestra el uso del disco.
- `Update-Modules`: Actualiza los módulos de PowerShell instalados.
- `Get-SystemInfo`: Muestra información del sistema.
- `Clear-DNSCache`: Limpia la caché de DNS.
- `Restart-ServiceByName`: Reinicia un servicio por nombre.
- `Search-StringInFiles`: Busca una cadena en archivos.
- `New-DirAndCD`: Crea un nuevo directorio y navega a él.
- `New-FileAndCD`: Crea un nuevo archivo y navega a su ubicación.

### 🌱 Variables de Entorno

Define variables de entorno personalizadas (actualmente no configuradas).

### 📂 Directorio de Scripts

Define el directorio donde se almacenan los scripts para PowerShell (actualmente no configurado).

## 🚀 Uso

Para utilizar este perfil, asegúrate de que el archivo `Microsoft.PowerShell_profile.ps1` se encuentra en la ubicación correcta para ser cargado por PowerShell al iniciar la sesión.

```powershell
# Verifica la ubicación del perfil
$PROFILE

# Copia el archivo a la ubicación del perfil
Copy-Item -Path .\Microsoft.PowerShell_profile.ps1 -Destination $PROFILE
```
---
📝 TODO
```markdown
- [ ] Agregar más alias personalizados para comandos de uso frecuente.
- [ ] Incluir funciones para la gestión de redes (e.g., Get-NetworkInfo, Test-InternetConnection).
- [ ] Crear funciones para la gestión de usuarios (e.g., Add-User, Remove-User).
- [ ] Implementar funciones para la gestión de servicios (e.g., Start-ServiceByName, Stop-ServiceByName).
- [ ] Añadir soporte para la gestión de archivos en la nube (e.g., Upload-ToCloud, Download-FromCloud).
- [ ] Integrar herramientas de desarrollo (e.g., Build-Project, Run-Tests).
- [ ] Configurar notificaciones de escritorio para eventos importantes.
- [ ] Crear funciones para la automatización de tareas comunes (e.g., Backup-System, Clean-TempFiles).
- [ ] Incluir funciones para la gestión de bases de datos (e.g., Backup-Database, Restore-Database).
- [ ] Añadir soporte para la gestión de contenedores Docker (e.g., Start-Container, Stop-Container).
- [ ] Implementar funciones para la gestión de máquinas virtuales (e.g., Start-VM, Stop-VM).
- [ ] Crear alias para comandos de Git (e.g., git status, git commit).
- [ ] Incluir funciones para la gestión de logs (e.g., Get-LogEntries, Clear-Logs).
- [ ] Añadir soporte para la gestión de tareas programadas (e.g., Create-ScheduledTask, Remove-ScheduledTask).
- [ ] Configurar un sistema de backup automático para el perfil de PowerShell.
- [ ] Integrar herramientas de monitoreo del sistema (e.g., Get-CPUUsage, Get-MemoryUsage).
- [ ] Crear funciones para la gestión de permisos de archivos y directorios.
- [ ] Añadir soporte para la gestión de certificados (e.g., Import-Certificate, Export-Certificate).
- [ ] Implementar funciones para la gestión de impresoras (e.g., Add-Printer, Remove-Printer).
- [ ] Incluir funciones para la gestión de dispositivos USB (e.g., List-USBDevices, Eject-USBDevice).
- [ ] Crear funciones para la gestión de procesos en segundo plano (e.g., Start-BackgroundProcess, Stop-BackgroundProcess).
- [ ] Añadir soporte para la gestión de tareas de copia de seguridad y restauración.
- [ ] Implementar funciones para la gestión de configuraciones del sistema (e.g., Get-SystemConfig, Set-SystemConfig).
- [ ] Crear alias para comandos de administración de Windows (e.g., Get-WindowsFeature, Install-WindowsFeature).
- [ ] Incluir funciones para la gestión de discos y particiones (e.g., Get-DiskInfo, Format-Disk).
- [ ] Añadir soporte para la gestión de políticas de grupo (e.g., Get-GPO, Set-GPO).
- [ ] Implementar funciones para la gestión de eventos del sistema (e.g., Get-EventLog, Clear-EventLog).
- [ ] Crear funciones para la gestión de tareas de mantenimiento del sistema (e.g., Run-DiskCleanup, Run-Defrag).
- [ ] Añadir soporte para la gestión de tareas de impresión (e.g., Print-Document, Cancel-PrintJob).
- [ ] Implementar funciones para la gestión de perfiles de usuario (e.g., Export-UserProfile, Import-UserProfile).
- [ ] Crear funciones para la gestión de configuraciones de red (e.g., Set-NetworkConfig, Get-NetworkConfig).
- [ ] Incluir funciones para la gestión de sesiones remotas (e.g., Start-RemoteSession, Stop-RemoteSession).
- [ ] Añadir soporte para la gestión de dispositivos Bluetooth (e.g., Pair-BluetoothDevice, Remove-BluetoothDevice).
- [ ] Implementar funciones para la gestión de energía del sistema (e.g., Get-PowerPlan, Set-PowerPlan).
- [ ] Crear alias para comandos de administración de Active Directory (e.g., Get-ADUser, New-ADUser).
- [ ] Incluir funciones para la gestión de configuraciones de seguridad (e.g., Get-SecurityConfig, Set-SecurityConfig).
- [ ] Añadir soporte para la gestión de configuraciones de firewall (e.g., Get-FirewallRule, Set-FirewallRule).
- [ ] Implementar funciones para la gestión de configuraciones de proxy (e.g., Get-ProxyConfig, Set-ProxyConfig).
- [ ] Crear funciones para la gestión de configuraciones de DNS (e.g., Get-DNSConfig, Set-DNSConfig).
- [ ] Incluir funciones para la gestión de configuraciones de DHCP (e.g., Get-DHCPConfig, Set-DHCPConfig).
- [ ] Añadir soporte para la gestión de configuraciones de VPN (e.g., Get-VPNConfig, Set-VPNConfig).
- [ ] Implementar funciones para la gestión de configuraciones de Wi-Fi (e.g., Get-WiFiConfig, Set-WiFiConfig).
- [ ] Crear alias para comandos de administración de IIS (e.g., Get-IISSite, Start-IISSite).
- [ ] Incluir funciones para la gestión de configuraciones de correo electrónico (e.g., Get-EmailConfig, Set-EmailConfig).
- [ ] Añadir soporte para la gestión de configuraciones de backup (e.g., Get-BackupConfig, Set-BackupConfig).
- [ ] Implementar funciones para la gestión de configuraciones de restauración (e.g., Get-RestoreConfig, Set-RestoreConfig).
- [ ] Crear funciones para la gestión de configuraciones de actualización del sistema (e.g., Get-UpdateConfig, Set-UpdateConfig).
- [ ] Incluir funciones para la gestión de configuraciones de aplicaciones (e.g., Get-AppConfig, Set-AppConfig).
```

¡Disfruta de tu sesión personalizada de PowerShell! 🎉