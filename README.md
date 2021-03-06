![mix](https://drive.google.com/uc?export=view&id=1t9a9mZr1iQRBr4H-xE7c2yXQVV-nDTY0)


# Overview 
Mix is a tool used for interacting and editing rigged characters. Mix was developed alongside Openrig( [Openrig Release](https://github.com/squarebit-studios/openrig/releases/latest) ) and is using libraries inside of it. Currently it only works with character in Maya built using Maya's PSD system. It is best to start from scratch. If you have not built a rig using Openrig

# Links
- [Dependencies](#dependencies)
- [Running Mix](#running-mix)
- [Contributing](CONTRIBUTING.md)
- [Licensing](LICENSE)

# Dependencies 
* [Openrig Release](https://github.com/squarebit-studios/openrig/releases/latest)
* Maya 2018 and on

# Running Mix
1. Download [Openrig](https://github.com/squarebit-studios/openrig/releases/latest) and [Mix](https://github.com/squarebit-studios/mix/releases/latest).
2. Add the openrig and Mix package to your python sys.path so it is available to Maya. (See env example below)
3. Open Mix with a rig using Maya's psd system
4. Run the following code in Maya to launch the UI.

```python
import mix.ui.main_window as mix_ui
mix_ui.launch()
```

# Python env setup example
```python
import os, sys

# repo path is the directory your repo's are located. Where you cloned your repo. 
repo_path = 'C:/Users/{user}/Desktop/squarebit'
openrig_path = os.path.join(repo_path, 'openrig')
mix_path = os.path.join(repo_path, 'mix')

sys.path.append(openrig_path)
sys.path.append(mix_path)
```

