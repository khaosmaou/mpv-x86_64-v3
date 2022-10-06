# REQUIREMENTS: 
   - Latest Python from https://www.python.org/downloads/
   - Latest Vapoursynth from https://github.com/vapoursynth/vapoursynth/releases

Make sure to install both system wide and available to all users, and add python to your path in the installer.

## INSTALLATION:

Once requirements are installed, open a cmd or PowerShell window and write:

   `python --version`

To verify python is correctly installed.

Then run the Python console and run these two commands to import vapoursynth to python and check version:

```   
from vapoursynth import core
print(core.version())
```

Use "quit()" to exit the shell.

Lastly, open and admin powershell window at "C:\Program Files\VapourSynth\vsrepo" and run this:

```
vsrepo.py install mv
```

### INFO:

Configs run very well on my 7700k and GTX 1080 for the content I watch, mostly 1080p and lower content. Check the configs for the keybinds.
