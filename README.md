![terminal-logos](https://user-images.githubusercontent.com/48369326/115790869-4c852b00-a37c-11eb-97f1-f61972c7800c.png)

# Personalizaci贸n de Windows Terminal

Links de instalaci贸n:

* [Windows Terminal](https://aka.ms/terminal)
* [Nerd Fonts](https://www.nerdfonts.com/font-downloads)
* [Terminal Icons](https://github.com/devblackops/Terminal-Icons)

## Instalaci贸n de fuentes

> 馃敶 Nota: Puedes instalar cualquier fuente, en este caso instale Fira Code, ya que abarca mas caracteres.

![](https://i.ibb.co/0cSPLXL/firacode.png)

![](https://i.ibb.co/hfQc2sK/fonts.jpg)

---

## Configurar la fuente

* Ingresar a configuraci贸n
* Escoger fuente descargada

![](https://i.ibb.co/GMm3QG9/configuracionfuente.jpg)

---
## Instalaci贸n y ejecuci贸n de Windows Terminal

> 馃敶 Nota: Windows Terminal requiere Windows 10 1903 (compilaci贸n 18362) o posterior

## Habilitar ejecuci贸n de scripts en PowerShell

`Ejecutar como administrador en windows terminal`:

```powershell
Set-ExecutionPolicy Unrestricted
```

## Instalaci贸n de oh-my-posh

Ejecutar en PowerShell:

```powershell
Install-Module oh-my-posh -Scope CurrentUser
```

Listar los temas:

```powershell
Get-PoshThemes
```

Escoger un tema en este caso escogi blueish:

```powershell
Set-PoshPrompt -Theme blueish
```
![](https://i.ibb.co/RzDBwqm/oh-my-posh.jpg)

---
## Instalaci贸n terminal icons

Ejecutar en PowerShell:

```powershell
Install-Module -Name Terminal-Icons -Repository PSGallery
```
## Para tener guardado la configuraci贸n

Ejecutar en PowerShell:

```powershell
notepad $PROFILE
```

Al abrir el archivo, guardar los comandos:

```powershell
Import-Module -Name Terminal-Icons
Import-Module oh-my-posh
Set-PoshPrompt -Theme blueish
```
![](https://i.ibb.co/2YjsY3F/note.jpg)