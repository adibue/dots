# adibue's dotfiles

This is my personal set up of configuration files, inspired by and originally forged from [haplo/dotfiles](https://github.com/haplo/dotfiles).

My main driver is macOS, with [CachyOS](https://github.com/cachyos) for gaming and [Debian](https://github.com/debian)oids for almost everything else.

Thanks to Cachy's defaults, I got quite fond of _fish_, so I recently switched to this incredibly easy and performant interactive shell 🚀.
However, scripts will still be written in `BASH` (or `ZSH`, if macOS is the only target platform).

Feel free to fork the repository, adapt it to your needs, or just copy whatever you like.

But... **Use at your own risk!**

## Dependencies

- [yadm](https://github.com/yadm-dev/yadm)
- [eza](https://github.com/eza-community/eza)
- Optional, but recommended: [fish shell](https://github.com/fish-shell/fish-shell)

## Installation

First, [install](https://yadm.io/docs/install) _yadm_, a simple dotfiles manager available for virtually every distro on the planet.

Yours isn't on the list? No biggie, as in the end it's just a single shell script.
Just download it and put it in your `PATH`.

It's _**simple**_. That's why it's _**great**_!

Once _yadm_ is up and ready, use it to clone this repo, install the files into `$HOME` and run the [bootstrap script](.config/yadm/bootstrap):

```shell
yadm clone --bootstrap -f https://github.com/adibue/dots.git
```

## Updating

```shell
yadm pull
```

## Fish plugins

I try to minimize the amount of plugins I use, but the ones I do use I decided to vendor, i.e. include in full in this repository.
This allows me to control the source code precisely, review updates manually and not to depend on an unverified external download whenever I install the dotfiles.

The vendored plugins are in [.config/fish/vendor/](.config/fish/vendor/).

To update the vendored plugins to their latest versions, in a _fish_ shell:

```fish
update-fish-vendored-plugins
```

## Thanks and inspiration

- The original version of this repository was based on [Fidel Ramos'
  dotfiles](https://github.com/haplo/dotfiles).
  Thanks to Fidel for sharing and writing an excellent guide about this and on how to [migrate over to fish](https://blog.fidelramos.net/software/fish-shell) ❤️
