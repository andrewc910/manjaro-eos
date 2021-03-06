# Elemanjaro

This is a spin of manjaro gnome that utilizes the Pantheon DE. 

> Note: State: Alpha, I am using as a daily driver however I recommend to install it in a VM for testing.

<p align="center">
  <img src="./.images/preview.png" width="800">
</p>

## Building

Install `git` & `manjaro-tools`:

```sh
pamac install manjaro-tools-iso git
```

Create a `manjaro-tools.conf` file in `~/.config/manjaro-tools` & paste in:

```
dist_codename="Mikah-Hera"
dist_release=1.0
```

Run:

```sh
git clone https://github.com/andrewc910/manjaro-eos.git
cd manjaro-eos
buildiso -f -p eos -t ./
# Iso will be in the manjaro-eos/oem/eos/1.0 folder after building
```

## This vs Manjaro Gnome

- `Gnome-shell` completely removed as it clashes with `Gala`
- `Gdm` replaced with `lightdm` with `pantheon-greeter` theme installed
- Replaced numerous GNOME apps with the Elementary counter-part

## Current Focus

Fix bugs to make this spin more stable

## Resources

- [Manjaro Build Iso Docs](https://wiki.manjaro.org/Build_Manjaro_ISOs_with_buildiso)
- [Elementary OS](https://elementary.io/)
- [Manjaro Tools Repo](https://gitlab.manjaro.org/tools/development-tools/manjaro-tools)
