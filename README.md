![terminal-logos](https://user-images.githubusercontent.com/48369326/115790869-4c852b00-a37c-11eb-97f1-f61972c7800c.png)

# Personalización de Windows Terminal

Links de instalación:

* [Windows Terminal](https://aka.ms/terminal)
* [Nerd Fonts](https://www.nerdfonts.com/font-downloads)
* [Terminal Icons](https://github.com/devblackops/Terminal-Icons)

## Instalación de fuentes

> 🔴 Nota: Puedes instalar cualquier fuente, en este caso instale Fira Code, ya que abarca mas caracteres.

![](https://i.ibb.co/0cSPLXL/firacode.png)

![](https://i.ibb.co/hfQc2sK/fonts.jpg)

---

## Configurar la fuente

* Ingresar a configuración
* Escoger fuente descargada

![](https://i.ibb.co/GMm3QG9/configuracionfuente.jpg)

---
## Instalación y ejecución de Windows Terminal

> 🔴 Nota: Windows Terminal requiere Windows 10 1903 (compilación 18362) o posterior

## Habilitar ejecución de scripts en PowerShell

`Ejecutar como administrador en windows terminal`:

```powershell
Set-ExecutionPolicy Unrestricted
```

## Instalación de oh-my-posh

Ejecutar en PowerShell:

```powershell
winget install JanDeDobbeleer.OhMyPosh
```

Listar los temas:

```powershell
Get-PoshThemes
```

Crear el scrip de configuracion powershell:

```powershell
New-Item -Path $PROFILE -Type File -Force
```
---
## Instalación terminal icons

Ejecutar en PowerShell:

```powershell
Install-Module -Name Terminal-Icons -Repository PSGallery
```
## Para tener guardado la configuración

Ejecutar en PowerShell:

```powershell
notepad $PROFILE
```

Al abrir el archivo, guardar los comandos:

```powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\cobalt2.omp.json" | Invoke-Expression
Import-Module -Name Terminal-Icons
```