# recalbox-utils

Acessar a página principal de Downloads
https://download.recalbox.com/pt/

# Instalação para PC

Acessar 

recalbox.conf 

Para forçar a utilização da entrada de vídeo externa (HDMI)
```
## Prefered external screen retrieved from ssh : xrandr
system.externalscreen.prefered=HDMI1
## Force selected external screen to resolution ex : 1920x1080
system.externalscreen.forceresolution=1366x768
## Force selected external screen to frequency ex: 60.00
```
```
# ------------ C - Audio ------------ #
## Set the audio device (auto, hdmi, jack)
audio.device=alsa_card.pci-0000_00_1b.0:hdmi-output-0
## Set system volume (0..100)
audio.volume=36
## Enable or disable system sounds in ES (0,1)
audio.bgmusic=1
```

Caso existam dúvidas sobre os nomes dos dispositivos de saída:

```mount -o remount,rw /```

```$ xrandr```

```$ xrandr --output LVDS1 --off --output HDMI1 --mode 1366x768```

Para acessar o Webserver do Recalbox

```
ssh root@192.168.1.XX
```

```
cd /recalbox/share/bios
```

```
cd /recalbox/share/roms
```
