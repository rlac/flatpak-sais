# Strange Adventures in Infinite Space (GPL) Flatpak

A [Flatpak](https://flatpak.org) build of [Strange Adventures in Infinite Space (GPL)](https://github.com/kuroneko/sais).

## Installation

Builds are not currently hosted anywhere. You can easily build it locally. Simply ensure flatpak-builder is installed on your system, then run:

```bash
# Add the Flathub repo for the freedesktop runtime if you haven't previously
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
# Install the Freedesktop runtime & SDK if not already installed
flatpak install flathub org.freedesktop.Platform//20.08
flatpak install flathub org.freedesktop.Sdk//20.08
# Build and install
flatpak-builder --install --user builddir com.github.kuroneko.SAIS.yml --force-clean
```
## Running

A launcher icon will be available once installed. You can also run from the command line:

```bash
flatpak run com.github.kuroneko.SAIS
```

If you want to uninstall, run:

```bash
flatapk remove com.github.kuroneko.SAIS
