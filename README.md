#### This is just a backup of my MPV with all it's configs and shader plugins.

# REQUIREMENTS: 
   - Latest Python from https://www.python.org/downloads/
   - Latest Vapoursynth from https://github.com/vapoursynth/vapoursynth/releases

Make sure to install both system wide and available to all users, and add python to your path in the installer.

## INSTALLATION:

Once requirements are installed, open a cmd or PowerShell window and write:

```
python --version
```

To verify python is correctly installed.

Then close the window and run the Python command console from your start menu and run these two commands to import vapoursynth to python and verify the install:

```   
from vapoursynth import core
print(core.version())
```

Use "quit()" to exit the python shell.

Lastly, open and admin powershell window in "C:\Program Files\VapourSynth\vsrepo\" and run this to install mvtools:

```
vsrepo.py install mv
```

### INFO:

Configs run very well on my 7700k and GTX 1080 for the content I watch, mostly 1080p and lower content. Check the configs for the keybinds.

Make sure to disable the Anime4K shaders with `Ctrl + 0` when watching any non anime content. You won't see a difference but it will give you less processing overhead.

### BASIC KEYBINDS:

See [input.conf](input.conf) for the default keybinds. I typically use the default mode as I find it works best for 720p or 1080p content. If viewing much older 480p anime or hentai content, I tend to use A+A mode with `Cntr + 4`. A lot of how things look is up to user preference. You can clear the shaders completely using `Cntr + 0`. Use the overlay with `Shift + I` to verify the interpolation is working. FPS should be listed as 60 in front of `(estimated)`.

### PERFORMANCE:

The default config settings I have setup work very well on my GTX 1080 8GB paired with a Intel Core i7 7700k at 4.5 GHz. If you have a much newer CPU with more cores, you can enable higher quality interpolation at the cost of much more CPU usage by editing [smoothing.vpy](smoothing.vpy) by commenting out line 23 and uncommenting line 24 to switch from BlockFPS to the higher quality FlowFPS. This will give far less artifacting but I cannot use it without framedrops in some scenes with my older 7700k.

### CREDITS:

- MPV https://github.com/mpv-player/mpv
- mpv-install https://github.com/rossy/mpv-install
- Anime4K Shaders: https://github.com/bloc97/Anime4K
- Python 3.XX https://www.python.org/
- Vapoursynth https://github.com/vapoursynth/vapoursynth
- mvtools https://github.com/dubhater/vapoursynth-mvtools
