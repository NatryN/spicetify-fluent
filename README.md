<div align=center><h1>Fluent</h1>  

  [Spicetify](https://github.com/khanhas/spicetify-cli) theme inspired by Windows 11 UI and Microsoft's Fluent Design  

</div>

<br>

![dark-1](screenshots/dark-1.png)  
<br>
![dark-2](screenshots/dark-2.png)  
<br>
![light-1](screenshots/light-1.png)  
<br>

## About


Requires Segoe UI font.

Based off [Ziro](https://github.com/schnensch0/ziro) theme by [schnensch](https://github.com/schnensch0)  
[Fluent UI System Icons](https://github.com/microsoft/fluentui-system-icons) by Microsoft Corporation  
[Phosphor Icons](https://github.com/phosphor-icons/phosphor-icons) by Phosphor Icons

## Install
Make sure spicetify >= v2.50 is installed. Run these commands:

### Windows
In **Powershell**:
```powershell
cd "$(spicetify -c | Split-Path)\Themes"
git clone https://github.com/williamckha/spicetify-fluent Fluent
Copy-Item Fluent\fluent.js ..\Extensions
spicetify config extensions fluent.js
spicetify config current_theme Fluent color_scheme dark
spicetify config inject_css 1 replace_colors 1 overwrite_assets 1
spicetify apply
```

### macOS and Linux
In **Bash**:
```bash
cd "$(dirname "$(spicetify -c)")/Themes"
git clone https://github.com/williamckha/spicetify-fluent Fluent
mkdir -p ../Extensions
cp Fluent/fluent.js ../Extensions/.
spicetify config extensions fluent.js
spicetify config current_theme Fluent color_scheme dark
spicetify config inject_css 1 replace_colors 1 overwrite_assets 1
spicetify apply
```

## Customization
Three color schemes are available: `light`, `dark` or `dracula`. Change scheme with commands:
```
spicetify config color_scheme <scheme_name>
spicetify apply
```
You can change the accent color in the theme folder's color.ini file.  
If you are using Windows, you can hide the window controls by adding the flag `--transparent-window-controls` after Spotify.exe in your Spotify shortcut.
