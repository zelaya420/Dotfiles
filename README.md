# Polybar Collection

My personal collection. Trying to make some nice themes, and show how great [Polybar](https://github.com/polybar/polybar) is. I'll keep updating the collection, and maybe create some custom scripts so you and I can have a better experience with this thing. I also recommend you to check this [adi1090x Polybar Collection](https://github.com/adi1090x/polybar-themes), has some great themes, so if you don't like my collection, you can just check the other one. Also the reason why I'm doing this is because I want you to have more options and ideas to build your own theme.

Read this README with attention.

## Getting Started

### Prerequisites

First of all, install Polybar:

[Compiling Polybar](https://github.com/polybar/polybar/wiki/Compiling)

By default the font used is `JetBrainsMono` (you can change it in the **fonts.ini** file), you can download and install from [NerdFonts](https://www.nerdfonts.com/font-downloads):

Also you'll need [MaterialIcons](https://github.com/google/material-design-icons) and [Feather](https://feathericons.com/).
You can move both **MaterialIcons** and **feather** inside **fonts** to **$HOME/.fonts/** and run:

```bash
$HOME
-> fc-cache -fv
```

or just search how to install fonts!

$HOME
-> ln -s $HOME/.config/polybar-collection $HOME/polybar-collection
```

### Running

BSPwm

```bash
$HOME/polybar-collection/launch.sh
```

I3wm

```bash
exec_always --no-startup-id $HOME/polybar-collection/launch.sh
```

Remember to keep updated:

```bash
$HOME
-> cd $HOME/polybar-collection && git pull
```

## Few changes

Now we only have one file **modules.ini** to change the modules that we like to use. I believe that's a better way to configure our Polybar themes:

```ini
modules-left = date wallz nft tor weather  i3 rofi-usb-mount
modules-center = mpd
modules-right = wired cpu memory xbacklight pulseaudio
```

The only problem with this, is that some themes don't have certain modules, for now at least! I'm planning on making this collection easier to setup, so if you have any ideas you can always share.

## Weather app

As pointed out by Dennis Perrone, my personal OpenWeather API Key is in the project as a constant, and I did this intentionally so it just works, and it's fine if you want to use it the same as me, but I'll suggest you to create your own API Key for free in the official [OpenWeather](https://openweathermap.org/api) website. There's a limit of requests you can make using the same API Key, so we both could be without the weather info if a lot of requests are made.

After you create your API Key, you can pass as an argument in the **weather.sh** script, or you can set an environment variable for **OPENWEATHER_API_KEY** with your own API Key:

## Wallz

Still thinking about this one, maybe I should add more 'backend' options, for now is only using Bing API, but I could add more options since Bing API have a 'limited', but with a really good quality, wallpapers collection. For now I'll be only using on minimal theme, but when I'm 'done' I'll add to the others.

## You might be interested

- [Rofi Collection](https://github.com/Murzchnvok/rofi-collection)
- [Wallpaper Collection](https://drive.google.com/drive/folders/1o1qjRgkJtnF_8uGB1z6MRsQUjWinHUsw?usp=sharing)
- [Pomotroid (pomodoro app)](https://github.com/Splode/pomotroid)
- [Ugly To-Do](https://github.com/Murzchnvok/ugly-todo)

_Enjoy!_

### aline

![desktop](screenshots/aline/Screenshot_2022-12-05-05-28-34_1366x768.png)
![desktop](screenshots/aline/Screenshot_2022-12-05-05-29-13_1366x768.png)



### Murz

![desktop](screenshots/murz/Screenshot_2022-10-31-02-59-45_1366x768.png)

```ini
modules-left = date weather round-right
modules-center = round-left i3 rofi-usb-mount round-right
modules-right = round-left spotify spotify-prev spotify-play-pause spotify-next battery session
```

### Chnvok

![desktop](screenshots/chnvok/Screenshot_2022-10-31-09-33-58_1366x768.png)

![desktop](screenshots/chnvok/Screenshot_2022-12-05-04-04-00_1366x768.png)


```ini
modules-left = date weather spotify spotify-prev spotify-play-pause spotify-next
modules-center = i3 rofi-usb-mount
modules-right = memory cpu xbacklight battery pulseaudio session
```

### Dracula

![desktop](screenshots/dracula/Screenshot_2022-12-05-04-15-14_1366x768.png) 
![desktop](screenshots/dracula/Screenshot_2022-12-05-04-15-35_1366x768.png )

```ini
modules-left = date margin weather margin spotify spotify-prev spotify-play-pause spotify-next
modules-center = i3 rofi-usb-mount
modules-right = memory margin cpu margin xbacklight battery margin pulseaudio margin battery margin session
```

### Gruvbox

![desktop](screenshots/gruvbox/Screenshot_2022-12-05-04-22-16_1366x768.png)
![desktop](screenshots/gruvbox/Screenshot_2022-12-05-04-24-56_1366x768.png)


```ini
modules-left = i3 rofi-usb-mount
modules-center = round-left-blue weather date round-right-blue margin round-left spotify spotify-prev spotify-play-pause spotify-next round-right
modules-right = cpu memory pulseaudio xbacklight battery
```

### Lofi

![desktop](screenshots/lofi/Screenshot_2022-12-05-04-32-39_1366x768.png)
![desktop](screenshots/lofi/Screenshot_2022-12-05-04-33-27_1366x768.png)


```ini
modules-left = i3 rofi-usb-mount
modules-center = spotify spotify-prev spotify-play-pause spotify-next
modules-right = date weather battery
```

### Material

![desktop](screenshots/material/Screenshot_2022-12-05-04-38-54_1366x768.png)

```ini
modules-left = weather margin date margin spotify spotify-prev spotify-play-pause spotify-next tri-upper-right tri-lower-left i3 rofi-usb-mount tri-upper-right
modules-center = 
modules-right = memory margin cpu margin battery xbacklight margin pulseaudio
```

### Minimal

![desktop](screenshots/minimal/Screenshot_2022-12-05-04-49-27_1366x768.png)
![desktop](screenshots/minimal/Screenshot_2022-12-05-04-49-09_1366x768.png)

```ini
modules-left = date weather i3 rofi-usb-mount
modules-center = spotify spotify-prev spotify-play-pause spotify-next
modules-right = cpu memory xbacklight battery pulseaudio session
```

### Lorena

![desktop](screenshots/lorena/IMG-20221203-WA0013.jpg)
![desktop](screenshots/lorena/Screenshot_2022-12-03-14-50-42_1366x768.png)

```ini
modules-left = launcher sep2 i3 sep2 rofi-usb-mount sep spotify sep spotify-prev spotify-play-pause spotify-next
modules-center = title
modules-right = sep2 updates sep filesystem sep backlight sep memory sep cpu sep battery sep date sep session
```

### Nord

![desktop](screenshots/nord/desktop.png)

```ini
modules-left = date margin weather margin spotify spotify-prev spotify-play-pause spotify-next round-right
modules-center = trap-left i3 rofi-usb-mount trap-right
modules-right = memory margin cpu margin xbacklight margin pulseaudio margin wallz margin session
```

### One Dark

![desktop](screenshots/onedark/desktop.png)

```ini
modules-left = i3 rofi-usb-mount margin date margin weather margin spotify spotify-prev spotify-play-pause spotify-next
modules-center =
modules-right = cpu margin memory margin pulseaudio margin xbacklight margin wallz margin session
```
