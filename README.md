A tutorial to fix the volumes buttons not being correctly mapped on Linux on Acer PT515-52 labtops.

> **Warging** : This script use the XDG Autostart specification to launch the script automatically.

# Prerequisites
- Install [xremap](https://github.com/xremap/xremap)

# Installation
0) Clone that repository or download the files

1) Copy the `config.yml` file into `~/.config/xremap/` 
_(You can copy it into another directory but i advise this one)_

Don't forget to change the `config_path` variable in `launch_xremap.sh` if you placed the config somewhere else.

2) Make the `launch_xremap.sh` executable using the command
```chmod +x ./launch_xremap.sh```

3) Copy the launch script into a directory. For me i've copied into the Home directory.

4) Set the `Exec` field of the `launch_xremap.sh.desktop` file to the lanch script path. **The path needs to be absolute.**

5) Copy the .desktop file into `$XDG_CONFIG_HOME/autostart`. If you want it to be system-wide, copy it to `$XDG_CONFIG_DIRS/autostart` instead.

6) Restart. If your volume keys still doesn't work, please open an issue.


