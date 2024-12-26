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
<input disabled="" type="checkbox"> Agregar más alias personalizados para comandos de uso frecuente.
<input disabled="" type="checkbox"> Incluir funciones para la gestión de redes (e.g., Get-NetworkInfo, Test-InternetConnection).
<input disabled="" type="checkbox"> Crear funciones para la gestión de usuarios (e.g., Add-User, Remove-User).
<input disabled="" type="checkbox"> Implementar funciones para la gestión de servicios (e.g., Start-ServiceByName, Stop-ServiceByName).
<input disabled="" type="checkbox"> Añadir soporte para la gestión de archivos en la nube (e.g., Upload-ToCloud, Download-FromCloud).
<input disabled="" type="checkbox"> Integrar herramientas de desarrollo (e.g., Build-Project, Run-Tests).
<input disabled="" type="checkbox"> Configurar notificaciones de escritorio para eventos importantes.
<input disabled="" type="checkbox"> Crear funciones para la automatización de tareas comunes (e.g., Backup-System, Clean-TempFiles).
<input disabled="" type="checkbox"> Incluir funciones para la gestión de bases de datos (e.g., Backup-Database, Restore-Database).
<input disabled="" type="checkbox"> Añadir soporte para la gestión de contenedores Docker (e.g., Start-Container, Stop-Container).
<input disabled="" type="checkbox"> Implementar funciones para la gestión de máquinas virtuales (e.g., Start-VM, Stop-VM).
<input disabled="" type="checkbox"> Crear alias para comandos de Git (e.g., git status, git commit).
<input disabled="" type="checkbox"> Incluir funciones para la gestión de logs (e.g., Get-LogEntries, Clear-Logs).
<input disabled="" type="checkbox"> Añadir soporte para la gestión de tareas programadas (e.g., Create-ScheduledTask, Remove-ScheduledTask).
<input disabled="" type="checkbox"> Configurar un sistema de backup automático para el perfil de PowerShell.
<input disabled="" type="checkbox"> Integrar herramientas de monitoreo del sistema (e.g., Get-CPUUsage, Get-MemoryUsage).
<input disabled="" type="checkbox"> Crear funciones para la gestión de permisos de archivos y directorios.
<input disabled="" type="checkbox"> Añadir soporte para la gestión de certificados (e.g., Import-Certificate, Export-Certificate).
<input disabled="" type="checkbox"> Implementar funciones para la gestión de impresoras (e.g., Add-Printer, Remove-Printer).
<input disabled="" type="checkbox"> Incluir funciones para la gestión de dispositivos USB (e.g., List-USBDevices, Eject-USBDevice).
<input disabled="" type="checkbox"> Crear funciones para la gestión de procesos en segundo plano (e.g., Start-BackgroundProcess, Stop-BackgroundProcess).
<input disabled="" type="checkbox"> Añadir soporte para la gestión de tareas de copia de seguridad y restauración.
<input disabled="" type="checkbox"> Implementar funciones para la gestión de configuraciones del sistema (e.g., Get-SystemConfig, Set-SystemConfig).
<input disabled="" type="checkbox"> Crear alias para comandos de administración de Windows (e.g., Get-WindowsFeature, Install-WindowsFeature).
<input disabled="" type="checkbox"> Incluir funciones para la gestión de discos y particiones (e.g., Get-DiskInfo, Format-Disk).
<input disabled="" type="checkbox"> Añadir soporte para la gestión de políticas de grupo (e.g., Get-GPO, Set-GPO).
<input disabled="" type="checkbox"> Implementar funciones para la gestión de eventos del sistema (e.g., Get-EventLog, Clear-EventLog).
<input disabled="" type="checkbox"> Crear funciones para la gestión de tareas de mantenimiento del sistema (e.g., Run-DiskCleanup, Run-Defrag).

¡Disfruta de tu sesión personalizada de PowerShell! 🎉