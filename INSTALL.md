### [qutebrowser](https://www.qutebrowser.org/)

#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

    $ git clone https://github.com/makman12/pywalQute.git

#### Install manually

Download using the [GitHub .zip download](https://github.com/makman12/pywalQute.git) option and unzip.

#### Activating theme

- Find your _[qutebrowser configuration directory](https://www.qutebrowser.org/doc/help/configuring.html#configpy)_ (see e.g. `:version` in qutebrowser). This folder should be located at the "config" location listed on qute://version, which is typically ~/.config/qutebrowser/ on Linux, ~/.qutebrowser/ on macOS, and %APPDATA%/qutebrowser/config/ on Windows.
- Move the repository folder to `pywalQute` inside the configuration directory.
- In your [qutebrowser config.py file](https://www.qutebrowser.org/doc/help/configuring.html#configpy), include the following:

```python
import pywalQute.draw

config.load_autoconfig()

pywalQute.draw.color(c, {
    'spacing': {
        'vertical': 6,
        'horizontal': 8
    }
})
```
