# Installing nord theme on windows 10

## Prerequisites
* Windows 1703 or higher(may not work on windows higher than 2004)

### Windows theme installation
* Download [UltraUxTheme](https://github.com/namazso/SecureUxTheme/releases/)
* Open UltraUxTheme and tick boxes as shown and click install
![Screenshot](https://i.imgur.com/4yPwDAM.png)
* Reboot your computer
* Download [Nord Windows 10 Theme](https://www.deviantart.com/niivu/art/Nord-Windows-10-Theme-837266272)
* Copy files from `Nord Windows 10 Theme UPDATE/Themes` to `Windows/Resources/Themes`
* Click on `Start theme tool` in SecureUxTheme
* Select Nord Darkest or your prefered nord variant and click apply, do not check any checkboxes.

### Spotify theme installation
* [Install](https://github.com/khanhas/spicetify-cli/wiki/Installation) Spicetify, use powershell method.
* Run 
  ```
    spicetify
    spicetify backup apply enable-devtool
  ```
  This will install spicetify onto your spotify installation
* Download this [repo](https://github.com/morpheusthewhite/spicetify-themes) and copy `Dribbblish` theme to `%USERPROFILE%/.spicetify/Themes`
* Launch powershell in copied `Dribbblish` folder and write: 
  ```
    cp dribbblish.js ../../Extensions
    spicetify config extensions dribbblish.js
    spicetify config current_theme Dribbblish color_scheme Nord-Dark
    spicetify config inject_css 1 replace_colors 1 overwrite_assets 1
    spicetify apply
  ```
  These commands will configure spicetify to use dribbblish.js file as extensions config, selects dribbblish as theme with Nord-Dark color scheme and configures some spicetify settings, then applies.

### Discord theme installation
* [Install](https://powercord.dev/installation) Powercord.
* Open your cloned powercord folder navigate to src/Powercord/Themes
* Put Customa folder from this repo in there
* Restart powercord

Note: if you already have an existing theme in powercord customa won't activate, open discord console and write 
```
powercord.styleManager.disable("Theme name");
powercord.styleManager.enable("Customa");
```

## Screenshots
![Task manager, explorer, spotify](https://i.imgur.com/NIOGdvm.png)
![Explorer, Visual Studio Code, Windows Terminal](https://i.imgur.com/GCE9Sbk.png)
![Spotify](https://i.imgur.com/2yZVVTf.png)
![Discord](https://i.imgur.com/zcLNCTl.png)

## Credits

### niivu - for creating Nord Windows 10 Theme
### namazso - for creating SecureUxTheme
### khanhas and all spicetify contributors - for creating spicetify and dribbblish theme
### https://powercord.dev/contributors - for creating and contributing to powercord
### Customa-Discord theme contributors - for creating customa theme