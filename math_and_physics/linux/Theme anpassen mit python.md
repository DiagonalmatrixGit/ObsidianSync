[Grundlage](obsidian://open?vault=math_and_physics&file=linux%2FThemes%20anpassen%20mit%20cli)

```python

import subprocess

# Einfache Shell-Kommandos: ls -l
subprocess.run(["ls", "-l"])
```

Beispiel:
```python
  
import subprocess

subprocess.run(["gsettings", "set", "org.gnome.shell.extensions.user-theme", "name", "Obsidian-flow-gray-light"])
```


