# Configuración i3wm para Debian

Esta configuración proporciona un entorno i3wm optimizado para Debian, con soporte para versiones 12 y 13.

## 📦 Paquetes necesarios

### Para Debian 12 o derivadas de Ubuntu:
```bash
sudo apt install dunst scrot imagemagick feh pamixer i3 i3blocks i3lock i3status i3-wm rofi nitrogen lxappearance fonts-font-awesome picom compton synapse flameshot policykit-1-gnome terminator numlockx neofetch diodon variety thunar mint-y-icons x11-utils xdotool wmctrl
```

### Para Debian 13:
```bash
sudo apt install dunst scrot imagemagick feh pamixer i3 i3blocks i3lock i3status i3-wm rofi nitrogen lxappearance fonts-font-awesome picom compton synapse flameshot terminator numlockx fastfetch diodon variety thunar mint-y-icons x11-utils xdotool wmctrl
```

**Nota:** En Debian 13 se utiliza el policykit de mate (incluido en XFCE) y se reemplaza neofetch por fastfetch.

## 🈯 Font Custom (Solo aplicable en la versión de Debian 12, Ubuntu y derivadas)
Para las fonts correspondientes de i3blocks es necesario copiar el archivo **ibm-plex-sans** desde el directorio en  que se descargó hasta el siguiente directorio **/usr/share/fonts/**

## 📁 Estructura de archivos

Los archivos de configuración deben ubicarse en `~/.config/`:

- `i3blocks/`
- `i3/` 
- `dunst/`

## 🚀 Instalación recomendada

Se recomienda partir de una distribución que tenga XFCE4 instalado o que venga por defecto con él.

## ⌨️ Atajos de teclado principales

### Gestión básica de ventanas
- `Mod4 + Enter` - Abrir terminal (Terminator)
- `Mod4 + q` - Cerrar ventana actual
- `Mod4 + f` - Alternar pantalla completa
- `Mod4 + Shift + Espacio` - Alternar entre flotante/tiling
- `Mod4 + Espacio` - Cambiar foco entre ventanas flotantes/tiling

### Movimiento y enfoque
- `Mod4 + j`/`←` - Enfocar ventana izquierda
- `Mod4 + k`/`↓` - Enfocar ventana inferior  
- `Mod4 + l`/`↑` - Enfocar ventana superior
- `Mod4 + ñ`/`→` - Enfocar ventana derecha
- `Mod4 + Shift + j`/`←` - Mover ventana izquierda
- `Mod4 + Shift + k`/`↓` - Mover ventana abajo
- `Mod4 + Shift + l`/`↑` - Mover ventana arriba
- `Mod4 + Shift + ñ`/`→` - Mover ventana derecha

### Disposición de ventanas
- `Mod4 + h` - Dividir horizontalmente
- `Mod4 + v` - Dividir verticalmente
- `Mod4 + s` - Cambiar a disposición apilada
- `Mod4 + w` - Cambiar a disposición en pestañas
- `Mod4 + e` - Alternar división

### Workspaces
- `Mod4 + 1-0` - Cambiar al workspace 1-10
- `Mod4 + Shift + 1-0` - Mover ventana al workspace 1-10

### Sistema
- `Mod4 + Shift + c` - Recargar configuración
- `Mod4 + Shift + r` - Reiniciar i3
- `Mod4 + Shift + e` - Salir de i3
- `Mod4 + Shift + x` - Bloquear pantalla con efecto blur
- `ImprPant` - Captura de pantalla con Flameshot

### Volumen
- `XF86AudioRaiseVolume` - Subir volumen 10%
- `XF86AudioLowerVolume` - Bajar volumen 10%
- `XF86AudioMute` - Silenciar/desilenciar
- `XF86AudioMicMute` - Silenciar micrófono

### Lanzadores
- `F12` - Abrir dmenu_run
- `Mod4 + d` - Abrir rofi
- `Mod4 + Shift + d` - Abrir synapse
- `Mod4 + t` - Abrir thunar
- `Mod4 + b` - Abrir brave browser, Para ello, instalarlo desde su página web (https://brave.com/es/download/)

### Modo Resize
- `Mod4 + r` - Entrar en modo resize
  - `j`/`←` - Reducir ancho
  - `ñ`/`→` - Aumentar ancho
  - `k`/`↓` - Aumentar alto
  - `l`/`↑` - Reducir alto
  - `Enter`/`Escape` - Salir del modo resize

**Nota:** `Mod4` corresponde a la tecla Windows/Super.
